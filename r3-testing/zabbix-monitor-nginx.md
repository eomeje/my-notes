Verify the Nginx http_stub_status module was installed

```
nginx -V 2>&1 | grep -o with-http_stub_status_module
```

Add the following to the `server` block of /etc/nginx/sites-available/default
```
        # allow Zabbix server to access the nginx status page
        location = /basic_status {
                stub_status;
                allow 159.203.36.31/24;
                deny all;
        }
```

Restart nginx

```
service nginx restart
```