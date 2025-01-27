# serv00-xray

## serv00 一键部署三协议

 ssh登陆后执行

1.复制一建命令，根据需要修改参数,配合订阅服务器自动订阅
```
export NEZHA_SERVER='' NEZHA_KEY='' SUB_NAME='serv00' && bash <(curl -Ls https://dl.argo.nyc.mn/ser.sh)
```
可选参数:TOK 隧道key ，ARGO_DOMAIN 隧道域名 ，UUID ，SUB_NAME 节点名称，

TMP_ARGO 节点类型，可选vls,vms，tuic,hy2,3x等,默认为3x，即vmess.tuic,hy2三协议

2.重新部署
```
pkill -kill -u $(whoami) && export NEZHA_SERVER='' NEZHA_KEY='' SUB_NAME='serv00' && bash <(curl -Ls https://dl.argo.nyc.mn/ser.sh)
```

推荐一个抱脸保活项目:

https://github.com/dsadsadsss/serv00-baohuo.git
