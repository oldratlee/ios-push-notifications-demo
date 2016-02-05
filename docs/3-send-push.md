给`App`发推送（服务端）
=============================================

通过[`houston`](https://github.com/nomad/houston)工具可以比较方便给`App`发送推送。

```bash
openssl pkcs12 -in PushHelloDemo.p12 -out PushHelloDemo.pem -nodes -clcerts
```

```bash
$ apn push 670388fb848f86ad738b6c3728c289d90db8191c6efc1df3eeef8fb5b36e06fd -e development -c PushHelloDemo.pem -m 'Hello Push Demo' 
push notification sent successfully
```
