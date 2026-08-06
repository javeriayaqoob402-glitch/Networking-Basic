# Linux TAR and ZIP Notes

# TAR (Tape Archive)

## What is TAR?
TAR (Tape Archive) is a Linux command used to combine multiple files and folders into a single archive file. It is commonly used for backup, sharing files, and storing data. TAR itself does not compress files unless it is used with gzip (`-z`).

## Syntax
```bash
tar [options] archive_name files_or_folder
```

## Commands

### Create an archive
```bash
tar -cvf backup.tar MyFolder/
```
- c = Create
- v = Verbose (show process)
- f = Archive file name

### Extract an archive
```bash
tar -xvf backup.tar
```
- x = Extract
- v = Verbose
- f = Archive file

### List archive contents
```bash
tar -tvf backup.tar
```
- t = List files inside archive

### Create compressed archive
```bash
tar -czvf backup.tar.gz MyFolder/
```
- z = Compress using gzip

### Extract compressed archive
```bash
tar -xzvf backup.tar.gz
```

---

# ZIP

## What is ZIP?
ZIP is a Linux command used to compress files and folders into a `.zip` file. It reduces file size and makes files easier to share.

## Syntax
```bash
zip [options] zip_file file_or_folder
```

## Commands

### Compress one file
```bash
zip notes.zip notes.txt
```

### Compress a folder
```bash
zip -r myfolder.zip MyFolder
```
- r = Include all files and subfolders

### List ZIP contents
```bash
unzip -l myfolder.zip
```
- l = List files only

### Extract ZIP file
```bash
unzip myfolder.zip
```

---

# Difference

| TAR | ZIP |
|------|-----|
| Creates an archive | Compresses files/folders |
| .tar or .tar.gz | .zip |
| Mostly used in Linux | Used in Windows and Linux |

## Interview Definitions

**TAR:** A Linux command used to create, extract, and manage archive files.

**ZIP:** A Linux command used to compress files and folders into a ZIP archive.
