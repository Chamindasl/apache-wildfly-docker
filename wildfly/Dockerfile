FROM jboss/wildfly
USER root
RUN yum clean all && yum install -y lsof tcpdump net-tools
RUN passwd --delete root
USER jboss
RUN  /opt/jboss/wildfly/bin/add-user.sh admin admin --silent
CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-c", "standalone-ha.xml", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]
