# This script no longer works for every Zippyshare url.
### Zippyshare requires better javascript handling than this script is intended to offer. There are other command-line downloaders with broader dependencies that do support all Zippyshare javascript shenanigans.

## zippyshare.sh
### bash script for downloading zippyshare files

##### Download single file from zippyshare

```bash
./zippyshare.sh url
```

##### Batch-download files from URL list (url-list.txt must contain one zippyshare.com url per line)

```bash
./zippyshare.sh url-list.txt
```

##### Example:

```bash
./zippyshare.sh https://www3.zippyshare.com/v/CDCi2wVT/file.html
```

zippyshare.sh uses `wget` with the `-C` flag, which skips over completed files and attempts to resume partially downloaded files.

### Requirements: `coreutils`, `grep`, `sed`, **`wget`**
