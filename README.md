# aws_whitepapers

run below to start downloading latest documents

```bash
curl "https://aws.amazon.com/whitepapers/" | grep -e '.*\.pdf.*' | sed -e 's/.*href="\(.*\)\.pdf.*/http:\1.pdf/g' | sort | uniq | xargs wget 
```
