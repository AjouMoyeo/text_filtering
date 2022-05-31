### 2runo님의 프로젝트(욕설 감지기)에 일부 수정 및 실행파일 추가버전
https://github.com/2runo/Curse-detection\
### 주의
구형 버전으로 구현되었으므로 tensorflow, keras, numpy의 버전 호환 고려해야함

## 사용 방법
src 파일로 경로 옮김

``` cd ./src ```

``` python filtering --text "욕설 분류를 위한 텍스트 입력"```


## 출력
욕설이 존재하면 return 1 및 print {욕설일 확률} 존재하지 않으면 return 0 및 print {욕설이 아닐 확률}

### 출력 예시
``` python filtering.py --text "고현준 팀플 모임도 안나오고 시~~발롬임" ```

return 1, print 0.9865211
