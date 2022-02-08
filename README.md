### DockerHub
[`metabase/spark`](https://hub.docker.com/r/metabase/spark)
[![](https://images.microbadger.com/badges/version/metabase/spark.svg)](https://microbadger.com/images/metabase/spark)

### Available versions

* `metabase/spark:2.1.1`
* `metabase/spark:3.2.1`

### Build It

```bash
docker build -t metabase/spark:3.2.1 .
```

### Use It

```bash
docker run -p 10000:10000 \
       --name sparksql-3.2.1 \
       --rm \
       -d metabase/spark:3.2.1
```

#### Run Metabase Tests

```bash
DRIVERS=sparksql clojure-X:dev:ee:ee-dev:drivers:drivers-dev:test
```

No additional env vars are needed.

### Push It

```bash
docker push metabase/spark:3.2.1
```
