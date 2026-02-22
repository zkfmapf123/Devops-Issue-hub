# docker desktop 말고 colima 쓰기

- docker desktop 은 제한이있고 유료임 (Rate Limit)
- 무료버전인 colima를 쓰자

## 설치

```sh
brew install colima docker
colima start
```

## 부팅할때 colima 띄우기

```sh
# ~/.zshrc

if ! colima status &> /dev/null; then
    echo "Starting Colima..."
    colima start --cpu 2 --memory 4 --disk 60
fi
```

## .docker/config.json 내 desktop 삭제하기

```sh
cat ~/.docker/config.json

{
  "credsStore": "desktop"  // Docker Desktop의 credential helper <- 이거삭제해야 함
}
```
