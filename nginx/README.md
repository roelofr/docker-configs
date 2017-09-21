# Nginx configs

This directory contains the configurations for Nginx.

This is relative to the `/etc/nginx` path on Debian-based systems.

**WARNING** Please, please don't blindly copy TLS-related information. It might
cause needless risk to your server and it's just a Really Bad Idea™.

You may want to use [Mozilla's TLS config generator][tls-config] with the best
settings.

[tls-config]: https://mozilla.github.io/server-side-tls/ssl-config-generator/?server=nginx-1.10.1&openssl=1.0.1e&hsts=yes&profile=modern
