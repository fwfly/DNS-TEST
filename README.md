# DNS-TEST
Test the behavior of zone management 

Qick setup from pdns docker-compose

https://github.com/PowerDNS/pdns/blob/master/docker-compose.yml

The env is based on pdns docker-compose.


# Create Zone and record:
```
pdnsutil --config-dir /etc/powerdns/ create-zone test
pdnsutil --config-dir /etc/powerdns/ add-record test aa A 192.168.1.1
```
