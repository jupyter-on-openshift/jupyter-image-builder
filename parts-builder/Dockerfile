FROM centos/python-35-centos7:latest

COPY assemble /usr/libexec/s2i/assemble
COPY run /usr/libexec/s2i/run
COPY save-artifacts /usr/libexec/s2i/save-artifacts
COPY usage /usr/libexec/s2i/usage

RUN . /opt/app-root/etc/scl_enable && \
    pip install -U pip setuptools wheel && \
    pip install zc.buildout
