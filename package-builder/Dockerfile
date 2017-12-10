FROM centos/s2i-base-centos7:latest

COPY assemble /usr/libexec/s2i/assemble
COPY run /usr/libexec/s2i/run
COPY save-artifacts /usr/libexec/s2i/save-artifacts
COPY usage /usr/libexec/s2i/usage

USER 1001
