# DNS-TEST
Test the behavior of zone management 

The env is based on [pdns docker-compose](https://github.com/PowerDNS/pdns/blob/master/docker-compose.yml).


## Enable the Env
```
docker-compose up
```

## Create Zone and record:
Inside of pdns container
```
pdnsutil --config-dir /etc/powerdns/ create-zone test
pdnsutil --config-dir /etc/powerdns/ add-record test aa A 192.168.1.1

```
Test dig 
```
dig -p 1053 aa.test @localhost
```
