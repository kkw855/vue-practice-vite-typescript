## npm 의존성 관리  

현재 버전을 npm 레지스트리의 최신 버전과 비교합니다. 사용 가능한 버전을 요약한 표로 인쇄합니다.
```sh
npm outdated
```
![img.png](docs/img.png)

모든 패키지를 업데이트합니다. 메이저 버전을 업데이트하지는 않습니다.
```sh
npm update
```

메이저 버전을 업데이트하려면 아래 명령을 실행합니다.
```sh
npm install -D lint-staged@latest
```
