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
     - ngx_packages:
       - nginx=1.24.0
     - ngx_sites_available_create: true
     - ngx_sites_available_path: /etc/nginx/sites-available
     - ngx_sites_enabled_create: true
     - ngx_sites_enabled_path: /etc/nginx/sites-enabled
     
  roles: 
    - pastir.nginx
```