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

## CSS 임포트
임포트 방법  
첫 번째
```vue
<script setup>
import './assets/main.css'  
</script>
```
두 번째  
scoped로 설정하거나 미디어 쿼리를 사용할 수 있다.
```vue
<style scoped>
@import './assets/main.css' (max-width: 800px);  
</style>
```
세 번째
CSS 파일에서 다른 CSS 파일을 임포트 할 수 있다.
```css
@import './assets/main.css';
```

## PostCSS 플러그인
.scss, .sass, .less, .styl, .stylus 등을 사용하는 것보다는  
PostCSS 플러그인과 함께 네이티브 CSS 변수를 사용하여 미래 표준을 준수하는 CSS를 작성하도록 권고하고 있습니다.

## CSS Module
클래스 이름이 충돌하는 걸 막아줍니다. ```<style scoped>```와 비슷합니다.
Random Hash가 추가된 클래스 이름을 사용하기 때문에 클래스 이름 충돌을 피할 수 있습니다.
```
{example: '_example_1mlos_1'}
```
```vue
<script setup>
import styles from './assets/example.module.css'
</script>
<template>
  <p :class="styles.example">Hello CSS Modules</p>
</template>
```
