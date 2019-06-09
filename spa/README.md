# SPA vs MPA <br> 단일 페이지 어플리케이션 vs 다중 페이지 어플리케이션
<br><br>
## Single Page Application

[SPA](https://ko.wikipedia.org/wiki/%EC%8B%B1%EA%B8%80_%ED%8E%98%EC%9D%B4%EC%A7%80_%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98)(Single Page Application)는 현재 웹개발의 트랜드가 되는 차세대 패러다임입니다.<br>
기존의 새로고침 방식의 MPA과는 달리 필요한 CSS, JS 등의 정적파일을 한 번에(나눠서도 가능하다) 모두 다운로드받고, 이후 사용자와의 상호작용 가운데 필요한 데이터만 서버로부터 받게 하여 트래픽의 총량을 줄이고, 네이티브 앱과 유사한 사용자 경험을 제공하여 사용자를 편리한 웹 공간에 머무를 수 있게 도와주는 애플리케이션 형태입니다.
<br>
> 대부분의 모던 프론트엔드 프레임워크(angular, react, vue)는 SPA를 권장합니다.

<br><br><br><br>

### SPA 장점
 * 기존 웹보다 더 좋은 사용자 경험을 제공할 수 있습니다.
 * 사용자 친화적인 웹을 만들수 있습니다.(빠른 반응성, 화면전환 에니메이션 등)
 * 서버 요청이 적기 때문에 서버의 부하가 줄어듭니다.(REST API를 통한 데이터 송수신)
 
### SPA 단점
 * 초기 구동 속도가 느립니다.
 * 검색엔진 최적화(SEO) 적용이 어렵고 까다롭습니다.([prerender.io](https://prerender.io/)같은 솔루션을 이용할수있다.)
 * IE용 대안을 별도로 마련해야 됩니다.
 * JS 위에서 작동하기 때문에 JS가 차단돼있으면 장애가 발생하기 때문에 대안을 별도로 마련해야 합니다.

<br><br>
 
### SPA 예시
 * Gmail
 * 구글 맵스
 * Facebook
 * Youtube
 * 모던 프론트엔드 프레임워크(react, vuew, algular) 공식 홈페이지
 <br><br>
![spa example](https://cdn-images-1.medium.com/max/1500/1*r1vmH5n7cYKJwYZq2fXKpw.gif)

<br><br><br><br><br><br>

## Multi Page Application

MPA는 __고전적인__ 방식으로 동작합니다. <br>
데이터를 보여주거나 서버로 요청을 보내는 등 변경사항이 발생하면 브라우저에서 서버로부터 새로운 페이지를 렌더링하게 합니다. 하지만 AJAX를 사용하여 서버와 브라우저 사이의 데이터 전달이 어느정도 해소되어, 페이지의 특정 부분만 바꿀 수 있도록 발전했습니다.<br>
그리고 MPA는 많은 콘텐츠의 양과 많은 UI 계층 때문에 SPA보다 거대합니다. <br>

<br><br><br>

### MPA 장점
 * 쉽고 정확한 검색엔진 최적화(SEO)를 제공합니다. 페이지당 하나의 키워드가 적용되기 때문에 다른 키워드들과의 순위를 매기는데 더 유리합니다.
 * JS가 차단돼있어도 정상적으로 작동할수 있습니다.
 * 다양한 브라우저를 지원합니다.
 
### MPA 단점
 * 프론트와 백엔드가 상당히 결합되있습니다. 예를 들어 상품 별점 같은 경우 db에서 뿌려주기 때문에 style로 width를 넣는다.
 * 프론트와 백엔드 각각의 프레임워크를 사용해야하고 개발과정이 길어지는 결과를 낳기 때문에 개발이 복잡해집니다.
 
 <br>
 
### MPA 예시
 * 네이버, 네이트같은 포털 사이트
 * 대부분의 쇼핑몰
 
 <br><br><br><br>
 
![MPA, SPA](https://www.e-nor.com/wp-content/uploads/2018/10/spa-architecture-1-822x1024.png)

## SPA or MPA
 
  1. 페이지의 목적을 고려해볼 필요가 있습니다. 다양한 카테고리가 필요하다면 (ex: 온라인 쇼핑몰, 네이버 같은 포털 사이트) MPA! <br> Pinterest, Facebook, Twitter 같은 하나의 애플리케이션 형태라면 SPA 사용을 추천 드립니다.
  2. 프로젝트에서 사용자 경험이 전략적으로 중요하다면 SPA!!
  3. 편리한 SEO, URL 공유를 원한다면 MPA!!
  4. SPA는 MPA보다 더 많은 수고가 필요하기 때문에 쉬운 길로 가고 싶다면 MPA!!
  
