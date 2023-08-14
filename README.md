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


Upload a folder:

```bash
aws s3 cp SOURCE_DIR s3://DEST_BUCKET/ --recursive
```
or sync:

```bash
aws s3 sync SOURCE_DIR s3://DEST_BUCKET/
```
