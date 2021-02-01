### Before you start

1. Install [nginx-cache-purge](https://crates.io/crates/nginx-cache-purge)
```
sudo apt install cargo

cargo install nginx-cache-purge

```
2. Rebuild your nginx with ngx_http_lua_module ([link](https://github.com/openresty/lua-nginx-module#installation))

### Start
```
sudo nginx -c $PWD/nginx.conf -g "pid /var/run/nginx.pid;"
```
### Reload
```
sudo nginx -s reload -c $PWD/nginx.conf -g "pid /var/run/nginx.pid;"
```
### Test config
```
sudo nginx -t -c $PWD/nginx.conf
```
