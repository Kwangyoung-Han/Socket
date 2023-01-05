# Socket

## NLP
### 프로그램
```
Socekt 통신을 위해 `Client`, `Server`에서 string을 주고 받는 코드입니다.
`NLP`를 위해 프로젝트를 했을 때 만들었습니다.
```

`Client.py`는 client 파일로 Mic, Speaker와 연결하여 Mic를 입력으로 받고 Server로 encoding 후 보내거나, Server로부터 받은 정보를 decoding 후 사용합니다.
`Server.py`는 server 파일로 Client로 받은 정보를 이용하여 미리 학습시킨 모델에 예측함수를 사용하여 예측 결과를 얻은 후, Client로 다시 보냅니다(소리방출 위해)

### 실행방법
1. Server에서 `python Server.py`를 실행 후, Client의 통신 대기
2. Client에서 `python Client.py`를 실행 후, Server와 통신
3. 통신 완료
