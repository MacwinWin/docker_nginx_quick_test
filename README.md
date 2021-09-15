# docker_nginx_quick_test
Test your nginx conf file quickly with docker

# How to use
```bash
# up your container
>>> docker-compose up -d
# edit your own configer
>>> vim nginx/nginx.conf
>>> vim nginx/conf.d/server.conf
# enter your container
>>> docker exec -it nginx_test sh
# reload the configer
/ $ nginx -s reload
/ $ exit
# test your configer
>>> ab -c 300 -n 300 'http://0.0.0.0:8080/test' 
```

![](./ScreenFlow.gif)
