FROM docker.elastic.co/logstash/logstash:6.5.4

ENV LS_JAVA_OPTS -Xms200m -Xmx200m
COPY Gemfile.lock /usr/share/logstash/Gemfile.lock
RUN logstash-plugin install logstash-input-jdbc logstash-input-beats logstash-output-elasticsearch logstash-output-stdout logstash-filter-grok logstash-filter-date logstash-filter-kv logstash-filter-urldecode


