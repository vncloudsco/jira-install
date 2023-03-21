FROM atlassian/jira-software:9.7.0-ubuntu-jdk11
LABEL maintainer="vouu <sale@tinyactive.net>" version="9.7.0"
RUN mkdir -p /var/agent
ADD agent.jar /var/agent/atlassian-agent.jar
ENV JAVA_OPTS="-javaagent:/var/agent/atlassian-agent.jar ${JAVA_OPTS}"
EXPOSE 8080