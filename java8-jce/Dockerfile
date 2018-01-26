FROM java:8
MAINTAINER Pablo Castelo <pablo@castelo.com.ar>
RUN curl -q -L -C - -b "oraclelicense=accept-securebackup-cookie" -o /tmp/jce_policy-8.zip -O http://download.oracle.com/otn-pub/java/jce/8/jce_policy-8.zip 
RUN unzip -jo -d ${JAVA_HOME}/jre/lib/security /tmp/jce_policy-8.zip \/\.jar
RUN rm /tmp/jce_policy-8.zip