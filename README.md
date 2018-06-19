# docker-elasticsearch-standalone

Elasticsearch for dev/test usage

* Using latest docker.elastic.co version as base image
* Tag 6.2, 6.3 for latest point release of each
* Defaults to these envs:
   * `ES_JAVA_OPTS=-Xms512m -Xmx512m`
   * `discovery.type=single-node`
   * `bootstrap.memory_lock=true`

Useful to get around constraints on environment variables containing '.'s
