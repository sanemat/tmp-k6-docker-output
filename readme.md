# k6 docker integration with artifacts
## works well
```
docker run -i -v $(pwd):/ci/ loadimpact/k6:latest run /ci/performance-test.js
```

## error

```
docker run -i -v $(pwd):/ci/ loadimpact/k6:latest run --out json=/ci/result.json /ci/performance-test.js
```

`time="2021-04-03T04:09:20Z" level=error msg="open /ci/result.json: permission denied"`
