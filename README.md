# ansible-nginx
* Description:

  Install nginx


* Distribution support: 
  - Ubuntu: 20,22,24
  
* Example:
```
---
- hosts: 'localhost'
  vars:
     - nginx_version: latest
     - nginx_sites_available_create: true
     - nginx_sites_available_path: /etc/nginx/sites-available
     - nginx_sites_enabled_create: true
     - nginx_sites_enabled_path: /etc/nginx/sites-enabled
     
  roles: 
    - pastir.nginx
```