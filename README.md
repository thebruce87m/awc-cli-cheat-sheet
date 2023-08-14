# awc-cli-cheat-sheet

Find version:

```bash
aws --version
```

Find out who is logged in:

```bash
aws sts get-caller-identity
```


Download specific folders using a file with the folder names:

```bash
cat file-with-folders.txt | xargs -I % aws s3 cp s3://bucket-name/% download/% --recursive
```
