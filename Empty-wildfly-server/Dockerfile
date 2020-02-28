FROM jboss/wildfly

ENV USERNAME=admin

ENV PASSWD=Admin#0000

RUN /opt/jboss/wildfly/bin/add-user.sh ${USERNAME} ${PASSWD} --silent

EXPOSE 9990 8080

CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]