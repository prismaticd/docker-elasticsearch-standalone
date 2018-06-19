# docker-elasticsearch-standalone

Elasticsearch for dev/test usage.  `prismaticd/elasticsearch-standalone/` on [Docker Hub](https://hub.docker.com/r/prismaticd/elasticsearch-standalone/).

* Using latest docker.elastic.co version as base image
* Tags:
  * 6.2
  * 6.3
  * latest
* Defaults to these envs:
   * `ES_JAVA_OPTS=-Xms512m -Xmx512m`
   * `discovery.type=single-node`
   * `bootstrap.memory_lock=true`

Useful to get around constraints on environment variables containing '.'s


## Example Docker Pull Command

E.g. to get the latest 6.2 release:

    docker pull prismaticd/elasticsearch-standalone:6.2

Run with:

    docker run prismaticd/elasticsearch-standalone:6.2 -p 9200:9200 -p 9300:9300

## Links

* [prismaticd/elasticsearch-standalone on Docker Hub](https://hub.docker.com/r/prismaticd/elasticsearch-standalone/)
* [elastic.co docker image documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html)
