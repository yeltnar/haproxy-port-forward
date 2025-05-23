the haproxy/haproxy.cfg binds on `:::8888 v4v6`

This binds to all ipv4 and ipv6 addresses on port 8888

### port summary 

port exposed from podman must be the real port from the incoming request

port exposed within podman can be whatever, as long as it is the sampe with `-p` and on the haproxy listen line

port leaving haproxy can be anything as long as it hits caddy

port inside caddy should match the port on the physical machine aka the podman exposed port 

