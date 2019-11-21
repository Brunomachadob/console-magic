# console-magic
Useful list of console magics

### Recursively find unique matches in files

```bash
find . -name '*.java' -exec grep -Eohr "com\.amazonaws.+Request" {} \; | sort -u
```
