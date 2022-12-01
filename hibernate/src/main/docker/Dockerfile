FROM jboss/wildfly

ENV LANG='en_US.UTF-8' LANGUAGE='en_US:en'

#Copy oracle module jdbc
COPY ./wildfly/modules/ /opt/jboss/wildfly/modules/

#Copy wildfly Configuration
COPY ./wildfly/standalone.xml /opt/jboss/wildfly/standalone/configuration/

#Copy artifact to Wildfly deployment folder
COPY target/*.war /opt/jboss/wildfly/standalone/deployments/