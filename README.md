### [2runo님의 프로젝트(욕설 감지기)](https://github.com/2runo/Curse-detection)에 일부 수정 및 실행파일 추가버전


### 주의
구형 버전으로 구현되었으므로 tensorflow, keras, numpy의 버전 호환 고려해야함

```tensorflow==2.4.1```

```keras==2.2.5```

버전 추천 

numpy와 버전 호환 오류 있을시,

```pip uninstall numpy```

```conda install numpy=1.19.5 -c conda-forge```



## 사용 방법
pretrained weight file -> ```src/model/ 경로에 다운```

[링크](https://drive.google.com/file/d/1gO_5Pltn9vEVVyOW3gTTR4e7_DdjKPrL/view)

src 파일로 경로 옮김

``` cd ./src ```

``` python filtering --text "욕설 분류를 위한 텍스트 입력"```


## 출력
욕설이 존재하면 ```return 1``` 및 ```print {욕설이 포함되었을 확률}``` 존재하지 않으면 ```return 0``` 및 ```print {욕설이 포함되었을 확률}```

### 출력 예시
``` python filtering.py --text "고현준 팀플 모임도 안나오고 시~~발롬임" ```

```return 1```, ```print 0.9865211```
