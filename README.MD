# javascript Plugin
## 공통 주의사항
* 각 플러그인 사용시 해당 플러그인의 필수 연결파일 먼저 확이나기
* css,js 파일확장자가 서로 다른경우 있으니 이름과 함께 확장자 반드시 확인!
## Swiper
* swiper, swiper-wrapper, swiper-slide
* 위 3개의 클래스명은 swiper 적용의 기본명칭으로 반드시 수정없이 그대로 작성하기!
* 위 공통 명칭회에 각 swiper 구분용으로 `div class= "swiper main_slide"` 시작테그에  한칸 띄고 별도의 구분용 클래서 적용하기 ex) `div class="swiper main_slide"`
* swiper플러그인 적용대상에 nth관련 수열선택자 사용하지 않기
* `swiper_slide`를 개별로 구문하고 싶다면? nth 수열선택자 사용하지 않고 개별 클래스 적용해서 디자인 또는 동적결과사용하기 ex) `div class= "swiper-slide slide1"`
* swiper 적용 대상에 원하는 태그추가는 swiper-slide 안에서만 사용하기(태그제한없음)
### swiper css 주의사항
* swiper, swiper-wrapper, swiper-slide 
* 위 기본클래스명 기준 swiper, swiper-wrapper 기본 css가 내장되어 있기 때문에 반드시 그점을 체크하고 원하는 css를 설정해야 한다
* 공통 swiper 클래서 대상기준사용가능한 css list: `width, margin, padding, position, transform, 꾸미는속성(background, color, font...)`
* 공통 swiper, swiper-wrapper클래스 flex 설정금지
* 공통 swiper-wrapper 금지속성 : 레이아웃 관련한 속성들(position, flex, float, width, height, margin(padding만 가능))

### Swiper option css 주의사항
* prev, next, pagination, scroll-bar
* 위 옵션들은 필요한 경우에만 선택적으로 작성한다
* swiper 시작태그의 바깥쪽 위치로 디자인하고 싶은 경우만 swiper 바깥쪽 위치에 태그를 구성하고 해당 위치의 새로운 부모대상에 position:relation를 설정한다.(swiper 옵션들에 absolute가 내장되어있기때문)