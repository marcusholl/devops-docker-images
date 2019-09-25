FROM ppiper/mta-archive-builder

USER root

RUN apt-get update && \
    apt-get install curl -y && \
    mkdir -p /opt/sap/piper/bin && \
    curl --insecure --fail -o /opt/sap/piper/bin/piper https://nexussnap.wdf.sap.corp:8443/nexus/content/repositories/deploy.snapshots/com/sap/de/marcusholl/go/go/0.0.1-SNAPSHOT/go-0.0.1-20190925.075502-1-amd64.jar && \
    chmod +x /opt/sap/piper/bin/piper

USER mta
