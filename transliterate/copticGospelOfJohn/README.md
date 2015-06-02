Used this to generate word frequencies

```sh
cat * | sed 's/[0-9]//g' | sed 's/\[//g' | sed 's/\]//g' | egrep -o '[^ ]*' | sort | uniq -c | sort -rn > wordFreq.txt
```
