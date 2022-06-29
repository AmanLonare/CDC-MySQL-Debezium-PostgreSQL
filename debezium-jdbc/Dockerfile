FROM quay.io/debezium/connect:1.9

ENV KAFKA_CONNECT_JDBC_DIR=$KAFKA_CONNECT_PLUGINS_DIR/kafka-connect-jdbc

ARG POSTGRES_VERSION=42.2.8
ARG KAFKA_JDBC_VERSION=5.3.2

COPY postgresql-42.2.8.jar /kafka/libs

RUN mkdir $KAFKA_CONNECT_JDBC_DIR

COPY kafka-connect-jdbc-5.3.2.jar $KAFKA_CONNECT_JDBC_DIR
