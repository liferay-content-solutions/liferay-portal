FROM liferay/jar-runner:latest

COPY resources/ /

ENTRYPOINT ["tini", "-v", "--", "/usr/local/bin/liferay_build_entrypoint.sh"]

ENV JAVA_VERSION=zulu11

USER root

WORKDIR /mnt/liferay-learn-workspace