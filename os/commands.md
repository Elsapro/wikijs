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