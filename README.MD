### Wordpress Docker Best Performance Pack

---

✅ Wordpress latest<br>
✅ PHP 7.4<br>
✅ PHP-FPM<br>
✅ Redis (Redis cache available)<br>
✅ Mysql 8.0<br>
✅ Nginx 1.18<br>
✅ Reverse Proxy (Caching && Connection Limiting && GZIP Compression)<br>

---

#### Google PageSpeed Results

![PageSpeed Results](/pagespeed.png)

#### 1. Clone project

```bash
git clone https://github.com/haliloncen/wordpress-docker.git
cd wordpress-docker
```

#### 2. Configure Environment Variables: `docker-compose.yml`

- WORDPRESS_DB_NAME: **wp-db-name**
- WORDPRESS_DB_USER: **wp-db-user**
- WORDPRESS_DB_PASSWORD: **wp-db-user-pass**

#### 3. Add Your SSL Certificates To `/config/nginx/ssl/`

- Generate SSL certificate with [Let's Encrypt](https://letsencrypt.org/) or other Certificate Authority

#### 4. Configure Nginx: `/config/nginx/nginx.conf`

- ssl_certificate /etc/ssl/**your-ssl-certificate-file**;
- ssl_certificate_key /etc/ssl/**your-ssl-certificate-key-file**;

#### 5. Build & Run

```bash
docker-compose up
```

#### 6. Go `http://localhost` On The Browser

#### Happy Coding 😎
