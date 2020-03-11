# docker-letsencrypt-envoy

- `git clone https://github.com/herpiko/docker-letsencrypt-envoy.git && cd docker-letsencrypt-envoy`
- `sed -i '' 's/example.org/yourdomain.com/g' envoy.yaml`
- `sed -i '' 's/example.org/yourdomain.com/g' docker-compose.yaml`
- `sed -i '' 's/hello@example.org/yourname@domain.com/g' docker-compose.yaml`
- `docker-compose up certbot`
- `docker-compose up -d envoy`
- Fire up your own service.
