# logstash_pipelines

This repository contains a few logstash pipelines created for specific situation.

in order to use this pipelines you need to configure listening ports, elastic search credentials and certificates.

## gelf_logs

This pipeline is to get docker logs using gelf over UDP conection.

docker example
```
        logging:
          driver: gelf
          options:
             gelf-address: "udp://logstash_ip:12201"
             tag: "my_container_neme"
```
