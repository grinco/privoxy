# privoxy

A privoxy docker image based on Alpine Linux. This image also incoperates AdBlock lists which is from https://projects.zubr.me/wiki/adblock2privoxy

Has socks5 forwarding to 172.17.0.1:9151 enabled by default.

```
docker run -d --restart unless-stopped --name privoxy -p 8118:8118 grinco/privoxy
```
Once the proxy started and set your browser goes through the proxy, you can edit the proxy config at http://config.privoxy.org/
