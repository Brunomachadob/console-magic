# console-magics
Useful list of console magics

#### Recursively find unique matches in files

```bash
find . -name '*.java' -exec grep -Eohr "com\.amazonaws.+Request" {} \; | sort -u
```

#### Query for an API server certificates

```bash
openssl s_client -showcerts -connect gnupg.org:443
```

#### Delete docker images by name

```bash
docker rmi $(docker images |grep '<NAME_HERE>')
```
