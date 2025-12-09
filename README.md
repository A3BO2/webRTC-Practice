# webRTC-Practice
webRTC의 동작원리를 알기위한 프로젝트

### 1. 모듈설치

```
npm i
```

### 2. cloudflared 설치

```
Windows
winget install cloudflare.cloudflared
```

```
macOS
brew install cloudflared
```

```
Linux
sudo apt install cloudflared
```

### 3. server.mjs에서 서버 실행

```
cmd
npm run dev
```

### 4. cloudflared로 터널 열기

```
cmd
cloudflared tunnel --url http://localhost:3000
```

그럼 아래처럼 출력됨:

Your tunnel has started!
https://small-panda-xyz.trycloudflare.com

여기서 나온 https://something.trycloudflare.com로 접속

두명의 접속자가 call버튼과 remote버튼을 각자 누르면 연결됨

