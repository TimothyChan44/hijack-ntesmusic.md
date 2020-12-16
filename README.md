# hijack-ntesmusic.md

# what u need
## mac OS
## git
```
git clone https://github.com/nondanee/UnblockNeteaseMusic.git
cd UnblockNeteaseMusic
```

## install pm2
```
npm install pm2 -g
ping music.163.com // to get IP
pm2 start app.js --name unblockMusic -- -f <IP> -p 8000:8043
```

## install Proxifier

```
ADD Proxy: HTTPS 127.0.0.1 8000
ADD Rules:
  - Name: NeteaseMusic
  - Applications: NeteaseMusic;com.apple.WebKit.Networking
  - Target Hosts: .music.163.com;.music.126.net;
  - Action: Proxy HTTPS 127.0.0.1 8000

￼Change DNS settings:
  - [x] Resolve hostnames through proxy
```

## install crt
```
double click file named 'ca.crt' in UnblockNeteaseMusic
double click 'UnblockNeteaseMusic Root CA' and set 'Always trust' at all
```


## install 700 以下的 NeteaseMusic

```
http://d1.music.126.net/dmusic/NeteaseMusic_2.0.0_700_web.dmg
```
