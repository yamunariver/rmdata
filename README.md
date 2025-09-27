# rmdata

## To list top 10 large files

```
sudo find / -type f -exec du -h {} + 2>/dev/null | sort -hr | head -n 10
```
