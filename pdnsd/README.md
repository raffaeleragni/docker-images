
## Steps

- `docker build -t pdnsd .`
- `docker run -d --restart=always -p 53:53/tcp -p 53:53/udp --name pdnsd -v pdns.conf:/etc/pdns.conf pdnsd`
- set localhost for resolving DNS
- profit
