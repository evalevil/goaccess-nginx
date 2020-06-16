## Dockerized Goaccess + GeoIP + Nginx ##

### Installation ###

1. Create empty access.log file:

    ```
    $ touch log/nginx/access.log
    ```

2. Run docker-compose:
    
    ```
    $ docker-compose up -d
    ```

3. Browse

    - your Application on `http://127.0.0.1:80`
    - GoAccess on `http://127.0.0.1:7890/goaccess/report.html`

--------

### Optionally ###

1. Edit access file for goaccess:
   
   ```
   $ vim config/nginx/access.conf
   ```

2. Change GeoIP library to enterprise version in `data`.

    example：`data/GeoLite2-City.mmdb`

### Ref
Fork from https://github.com/icamys/docker-goaccess-nginx
