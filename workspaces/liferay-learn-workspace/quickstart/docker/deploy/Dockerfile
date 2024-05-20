FROM liferay/jar-runner:latest

COPY resources/ /

ENTRYPOINT ["tini", "-v", "--", "/usr/local/bin/liferay_deploy_entrypoint.sh"]

ENV JAVA_VERSION=zulu11

USER root

RUN apt-get update && apt-get install --yes git mysql-client p7zip-full rsync

WORKDIR /mnt/liferay-learn-workspace