FROM bharatht08/ccw-consul-agent:latest
ADD ./config /config/
ENTRYPOINT ["/bin/consul", "agent", "-server", "-config-dir=/config"]
