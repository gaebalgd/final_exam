# final_exam
## 서울대학교, 벤처창업웹프로그래밍 2, 2016년 1학기 기말고사


• accounts  앱을 생성하여, 회원가입/로그인/로그아웃 구현
◦ django.contrib.auth  앱을 최대한 활용하기
◦회원가입 뷰에서 next 파라미터 처리
◦회원가입/로그인/로그아웃 링크를 템플릿에 출력하고,  next  인자를  현재 페이지 로 필히 지정


•템플릿 상속


•템플릿 스타일은 추가 스타일이 없더라도, 깔끔하게 정리가 되어야 합니다.


•모델
◦아래 모델에 대해 admin 및 view/form 을 통해 추가/조회/수정이 이뤄져야합니다.
◦Category 모델 ◾분류명 필드
◾생성일시
◾수정일시

◦Shop 모델 ◾가게명 필드
◾가게 전화번호 필드
◾가게 주소 필드
◾가게 설명 필드
◾가게 사진1 필드
◾가게 사진2 필드 : 옵션 필드
◾가게 사진3 필드 : 옵션 필드
◾생성일시
◾수정일시

◦Review 모델 ◾관련 Shop
◾리뷰쓴 유저
◾남긴 말 필드
◾인증샷 필드 : 옵션 필드
◾생성일시
◾수정일시

◦모델간의 관계 ◾Category : Shop = 1 : N
◾Shop : Review = 1 : N



•구현해야할 뷰
◦index 뷰 ◾Category 별 목록 Shop List 노출
◾각 Category 별 링크
◾최근 Review List 노출
◾Category/Shop 생성/수정 링크

◦category_new ◾새로운 Category 생성

◦category_edit ◾기존 Category 수정

◦category_detail ◾해당 Category 내 Shop List 노출

◦shop_new ◾새 Shop 생성

◦shop_edit ◾기존 Shop 수정

◦shop_detail ◾Shop 자세히 보기
◾Review 목록
◾Review 쓰기/수정 링크

◦review_new ◾새 리뷰 생성

◦review_edit ◾기존 리뷰 수정



•Azure WebApp 배포에 필요한 파일들을 모두 생성해야합니다. 시험기간 중에 Azure WebApp 사이트에 배포를 하지 않아도 되지만, Azure WebApp 배포가 가능한 상태여야합니다.


가산점 포인트
•위 모델필드 외에 필요하다고 생각되는 필드가 있으면 더 추가하셔도 됩니다. 적절하다고 판단이 될 경우  가산점 이 있습니다. 추가된 필드는 템플릿 내에 적절히 노출되어야합니다.
•추가 스타일을 지정하실 경우 ◦bootstrap-theme 를 적용하셔도 됩니다.

•접근제한 ◦Category : superuser에 한해서
◦Shop : 소유자 User에 한해서
◦Review : 리뷰 쓴 User에 한해서

•각 Category/Shop/Review 별 삭제
