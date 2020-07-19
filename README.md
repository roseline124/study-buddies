# study buddies

두 개의 submodule 로 이루어져 있습니다.

- [server](https://github.com/angelhack-study-buddies/study-buddies-server)
- [client](https://github.com/angelhack-study-buddies/study-buddies-client)

한꺼번에 다운로드 받기 위해서는 아래 명령어를 이용합니다.

```
git clone --recurse-submodules git@github.com:angelhack-study-buddies/study-buddies.git
or
git clone --recurse-submodules https://github.com/angelhack-study-buddies/study-buddies.git
```

개발은 [graphql](https://graphql.org) 을 이용 하였고
서버는 [apollo](http://apollographql.com), 웹은 [react](https://www.apollographql.com/docs/react) 를 사용 하였습니다.

Database 는 MySQL (Amazon RDS) 를 사용하였고
배포는 docker image 를 만들어 [ainize](https://ainize.ai) 를 통해 배포하였습니다.

주요 기능은 매일매일 게시물을 등록하여 `연속 학습 일 수`를 쌓는 기능과
다른 사용자의 게시물을 (내가 올린 게시물을 기반으로) `추천`해 주는 기능 입니다.

추천 받은 게시물을 통해 다음에 뭘 공부하면 좋을지 학습 대상을 찾게 되고 꾸준히 공부한 내용을 업로드 하여 자신만의 컨텐츠를 쌓아갑니다.
