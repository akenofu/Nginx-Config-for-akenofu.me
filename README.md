# Nginx-Config-for-akenofu.me
Overview
1. Redirects HTTP to HTTPs
2. VHost routing for akenofu.me , notes.akenofu.me and blog.akenofu.me
3. Uses the lets encrypt generated certificate for each of the three subdomains

To generate a lets encrypt certificate:
1. follow the following guide to Install Let's Encrypt's certbot <br>
https://www.inmotionhosting.com/support/website/ssl/lets-encrypt-ssl-ubuntu-with-certbot/

2. Generate the certificate using Certbot
```bash
sudo certbot certonly --nginx -d 'akenofu.me'
```
> Make sure port 8080 allows inbound and outbound traffic; Let's encrypt magic requires inbound and outbound access from&to port 8080
