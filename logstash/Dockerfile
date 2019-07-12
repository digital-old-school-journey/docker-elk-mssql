FROM docker.elastic.co/logstash/logstash:7.2.0

RUN rm -f /usr/share/logstash/pipeline/logstash.conf
# ADD config/ /usr/share/logstash/config/

RUN logstash-plugin install logstash-filter-jdbc_streaming
RUN logstash-plugin install logstash-filter-aggregate
RUN logstash-plugin install logstash-input-jdbc
RUN logstash-plugin install logstash-filter-translate

COPY ./jars /logstash/jars/