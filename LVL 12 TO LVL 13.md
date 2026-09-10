## Level 12 → 13

### Goal

The file `data.txt` contains a hexdump of a repeatedly compressed file. The task is to decompress it until the password is obtained.

### Steps

First, create a temporary directory and copy the file: using these commands
```bash
mkdir /tmp/b12
cp data.txt /tmp/b12
cd /tmp/b12
```

<img width="286" height="44" alt="image" src="https://github.com/user-attachments/assets/4218b1cb-8db7-4a7e-bf4b-a6696c82c45b" />


Convert the hexdump back into its original binary form:

```bash
xxd -r data.txt data
```

<img width="353" height="16" alt="image" src="https://github.com/user-attachments/assets/3e8e5cb5-e7a2-4520-a18c-3c3954c98ddc" />

Check the file type:

```bash
file data
```

<img width="953" height="47" alt="image" src="https://github.com/user-attachments/assets/e8e66850-b4e7-48e1-ae0f-7fb3faff45d9" />


It shows that the file is **gzip compressed**.

Decompress it:

```bash
gzip -dc data > data2.bin
```

Check again:

```bash
file data2.bin
```

It is **bzip2 compressed**.

```bash
bzip2 -d data2.bin
file data2.bin.out
```

It is **gzip compressed** again:

```bash
gzip -dc data2.bin.out > data4.bin
file data4.bin
```

It is a **tar archive**:

```bash
tar -xf data4.bin
file data5.bin
```

Again, it is a **tar archive**:

```bash
tar -xf data5.bin
file data6.bin
```

It is **bzip2 compressed**:

```bash
bzip2 -d data6.bin
file data6.bin.out
```

It is a **tar archive**:

```bash
tar -xf data6.bin.out
file data8.bin
```

It is **gzip compressed**:

```bash
gzip -dc data8.bin > data9.bin
```

Finally, read the password:

```bash
cat data9.bin
```
<img width="462" height="32" alt="image" src="https://github.com/user-attachments/assets/712f9bb9-33de-4595-a896-a9de16a8c263" />

The output contains the **password for Bandit Level 13**.
