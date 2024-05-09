# FreeDuckDuckGo

### Docker Compose

#### FreeDuckDuckGo Service

```bash
git clone https://github.com/louisje/FreeDuckDuckGo.git && cd FreeDuckDuckGo
docker compose up -d --build
```

### Test FreeDuckDuckGo

```bash
curl http://127.0.0.1:3456/v1/chat/completions \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-3.5-turbo",
    "messages": [
      {
        "role": "user",
        "content": "Hello!"
      }
    ],
    "stream": true
    }'
```
