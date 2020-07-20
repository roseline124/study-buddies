# study buddies

두 개의 submodule 로 이루어져 있습니다.

- [server](https://github.com/roseline124/study-buddies-server)
- [client](https://github.com/roseline124/study-buddies-client)

한꺼번에 다운로드 받기 위해서는 아래 명령어를 이용합니다.

```
git clone --recurse-submodules git@github.com:roseline124/study-buddies.git
or
git clone --recurse-submodules https://github.com/roseline124/study-buddies.git
```

submodule에 name 또는 path를 주고 싶은 경우, 아래 명령어를 이용합니다.
path 끝의 `/`를 잊지 마세요!

```
git submodule add --name {name} {repository-url} {path}/

like this

git submodule add --name server https://github.com/roseline124/study-buddies-server.git server/
git submodule add --name client https://github.com/roseline124/study-buddies-client.git client/
```

## 개발

- typescript
- server: [apollo-server](https://www.apollographql.com/docs/apollo-server/), `node`, `sequelize`
- client: [apollo-client](https://www.apollographql.com/docs/react), `react`, `materializecss`
- database: mysql (AWS RDS)
- deployment: via [ainize](https://ainize.ai)

## 주요 기능

주요 기능은 매일매일 게시물을 등록하여 `연속 학습 일 수`를 쌓는 기능과
다른 사용자의 게시물을 (내가 올린 게시물을 기반으로) `추천`해 주는 기능 입니다.

추천 받은 게시물을 통해 다음에 뭘 공부하면 좋을지 학습 대상을 찾게 되고 꾸준히 공부한 내용을 업로드 하여 자신만의 컨텐츠를 쌓아갑니다.

`google login` 을 이용하여 사용자가 편리하게 서비스를 이용 할 수 있도록 하였고
등록한 url 로 부터 `og tag 를 추출`하여 내용을 보기 쉽게 하였습니다.

`좋아요` 와 `follow` 기능을 추가하여 인기 컨텐츠를 파악 할 수 있게 하였고
추후 `인기 컨텐츠`와 카테고리에 대해 관리자가 featured 로 지정 하는 방식으로 교육 과정 제작과 연계 될 수 있을 것으로 기대 합니다.

### 프로필 조회

![profile](images/profile.png)

### 게시물 등록

![post](images/post.png)

### 게시물 조회 및 연속 학습 일 수

![daily-posting](images/daily-posting.png)

### 팔로우

![follow](images/follow.png)

### 추천

![recommendation](images/recommendation.png)
