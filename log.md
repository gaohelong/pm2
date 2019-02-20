### pm2执行npm
```javascript
# pm2
$ pm2 start npm -- start

# npm
$ npm run start
```

### pm2添加至node.js项目
```javascript
$ npm install pm2
```

### pm2命令
```javascript
$ pm2 start app.js

# pm2进程停止、重启、删除
$ pm2 stop     <app_name|id|'all'|json_conf>
$ pm2 restart  <app_name|id|'all'|json_conf>
$ pm2 delete   <app_name|id|'all'|json_conf>

# 查看pm2详情
$ pm2 desc

# 所有进程监控
$ pm2 monit

# 所有进程日志
$ pm2 log

# 清空所有进程日志
$ pm2 flush

# 启动一个进程并把它命名为 prod
$ pm2 start npm --name prod -- start

# 开启集群(开启3个进程)
$ pm2 start server/prod.js -i 3
```
