<!-- TITLE: Commands -->
<!-- SUBTITLE: A quick summary of Commands -->

# Commands
## Secure Copy between computers using ssh

```text
scp -rv /path/to/file username@a:/path/to/destination
```

## Unzip Multiple Zips to Different Dicrectories
```text
find -name '*.zip' -exec sh -c 'unzip -d "${1%.*}" "$1"' _ {} \;
```
## Find out what disk a particular directory is mounted on
```text
df -P file/goes/here | tail -1 | cut -d' ' -f 1
```
