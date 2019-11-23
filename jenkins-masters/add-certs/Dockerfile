FROM quay.io/openshift/origin-jenkins:4.1
ARG ca_cert
USER root
RUN echo ${ca_cert} > /etc/pki/ca-trust/source/anchors/ca-chain.cert.perm
RUN chmod 644 /etc/pki/ca-trust/source/anchors/ca-chain.cert.perm && update-ca-trust

USER 1001
