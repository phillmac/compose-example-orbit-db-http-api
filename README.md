# compose-example-orbit-db-http-api
An example docker compose project for the orbit-db-http-api using certbot, nginx, and go-ipfs

### **NOTE** ###

**Replace** `domain.io` **with your real domain in:**
 - **config/domains/list.txt**
 - **config/reverse-proxy/conf.d.available/api.ipfs.domain.io.conf**
 - **config/reverse-proxy/conf.d.available/gw.ipfs.domain.io.conf**
 - **config/reverse-proxy/conf.d.available/api.orbitdb.domain.io.conf**
 
 **Rename all the** `config/reverse-proxy/conf.d.available/*io.conf` **files to match the new domain name**

### How To Run ###

```
docker-compose up -d
docker-compose exec certbot sh run.sh
docker-compose restart reverse-proxy
```
