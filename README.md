# profacto_nginx_proxy
nginx profacto proxy config and docker-compose file to use the profacto API with HTTPS.

## Usage

**Replace the following placeholders in `docker-compose.yml`:**

- `<certificate-folder-path>` path on the host system where the certificate files are stored
- `<static-site-content-path>` path on the host system where the web content files are stored

**Replace the following placeholders in `nginx.conf`**

- `<domainname.tld>` domain name (e.g. example.com)
- `<profacto-API-url>` profacto API server url (e.g. http://profactoserver.domain.local:8080/4DAction)

- `<certificate.crt>` ssl certificate name
- `<certificate-key.rsa>` ssl certificate key name
- `<trusted-intermediate-certificate.cer>` ssl intermediated trusted certificate (CA authorithority trusted certificate)

- `<dns-resolver-1>` DNS resolver (e.g. 1.1.1.1)
- `<dns-resolver-2>` DNS resolver (e.g. 8.8.8.8)