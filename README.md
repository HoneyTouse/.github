# 🐝꿀단집 (HoneyTouse)

> **"당신의 감성을 흔드는 인테리어 꿀템이 가득한 꿀단집"**

> "특별한 감성을 담은 소품과 가구를 원하는 당신을 위한 꿀템이 가득!<br>
> 저희 꿀단집에서 만나보세요.” 🍯🏠

> <b>https://www.honeytouse.com</b>

<center>

![logo_with_animation](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/5f8233de-177e-46a3-8b78-861024c6d34b)

![리드미최상단](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/6374c883-fad2-40ad-bec2-01fcf71cac01)

</center>

<details>
<summary><b>유튜브 시연 영상</b></summary>
<div markdown="1">

[![Video Label](http://img.youtube.com/vi/5DiQ-FD5xv8/0.jpg)](https://youtu.be/5DiQ-FD5xv8)

</div>
</details>

---

## 바로가기

- [서비스 소개](#서비스-소개)<br>
- [프로젝트 개요](#프로젝트-개요)<br>
- [스토리보드](#스토리보드)<br>
- [페이지 구성](#페이지-구성)<br>
- [주요 구현 내용](#주요-구현-내용)<br>
- [기능 설명](#기능-설명)<br>
- [참고 링크](#참고-링크)<br>

---

## 서비스 소개

- <b>요약</b> : 기능성과 스타일을 모두 갖춘 인테리어 소품 및 생활용품을 판매하는 쇼핑몰

- <b>기획 의도</b> :

  - 1인가구의 증가와 워라벨에 대한 높아진 인식으로 집에 있는 시간이 늘어남에 따라 휴식공간인 집의 인테리어에도 많은 관심이 몰리고 있음.
  - 여성의 인테리어 관심도가 높기에 여성유저를 타겟으로 예쁜색상과 귀여운 디자인을 채택하여 접속하는 유저들의 머릿 속에 '인테리어 = 꿀단집'이라는 기억이 남을 수 있게 디자인한 쇼핑몰을 런칭함.

- <b>서비스 명칭</b> :

  - **꿀단집(HoneyTouse)**
    - 꿀단지<u>(HoneyPot)</u> + 집<u>(House)</u>의 합성어
    - 꿀같은 휴식과 안락함을 즐길 수 있는 다양한 제품들을 제공하는 서비스의 이미지를 연상하도록 하며, 따뜻하고 아늑한 느낌을 줌.

- <b>페르소나</b> :
  - <b>권 나리 / 20대 여성 / 서울 거주 자취생 (1인가구)</b>
    - 저렴하면서도 세련되게 자취방을 꾸밀 수 있는 아기자기한 감성 가구 및 소품을 원함.
    - 자취방에서 사용할 수 있는 심플한 생활용품 구매를 희망함.
    - 실용성이 뛰어나면서도 본인의 감성을 채워줄 물건을 찾고 있음.

<details>
<summary><b>페르소나 이미지 파일</b></summary>
<div markdown="1">

![image](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/732522c3-ea12-4d43-9b32-4dfc4b765ec6)

</div>
</details>

---

## 프로젝트 개요

- ### 진행 기간 <br>

  - <b>1차</b> : 기획 및 개발 (24.02.19 ~ 24.03.01) [2주]<br>
  - <b>2차</b> : 리팩토링 (24.03.08 ~ ) [자율] <br>
    - (주)엘리스가 보유하고 있는 프라이빗 GitLab 저장소에서 1차 개발을 마침.<br> 이후 개별적으로 Github Organization 생성하여 2차 리팩토링을 자율적으로 진행함.

- ### 진행 인원 및 역할 <br>

  - 7명 (프론트엔드 4명, 백엔드 3명)<br>
    | 팀원 이름 | FrontEnd | BackEnd | 배포/발표/영상 |
    |----------------------------|---------------------------|---------------------------|--------------------------|
    | <b>김지윤</b> | • 상품 상세 페이지<br>• 장바구니 페이지 | - | • 시연 영상 제작 |
    | <b>문채영</b> | - | • Admin API(관리자 기능)<br>• Order API (회원/비회원 주문 CRUD) | • PPT 제작 |
    | <b>신창건</b> | • 마이페이지 프로필 관리 부분 | - | • PPT 제작 |
    | <b>이가린</b> | • 마이페이지 프로필 이미지 업로드 부분 | • User API (로그인, 회원가입, 이메일 인증, 개인정보 CRUD) | • 발표<br>• 2차 배포 (AWS, Github Actions) |
    | <b>이승철</b> | • 메인페이지<br>• 로그인 및 회원가입 페이지 | - | • PPT 제작<br>• 1차 배포(Nginx) |
    | <b>이보미</b> | • 주문 및 결제 페이지<br>• 마이페이지 주문내역 부분 | - | • 시연영상 제작 |
    | <b>최정민</b> | • 관리자 페이지 | • Category API (카테고리 CRUD)<br>• Product API (상품 CRUD) | • PPT 제작 |

- ### 관련 링크

  - <b>노션 페이지</b> : https://holy-mailbox-d99.notion.site/HONEY_TOUSE-3-24dfdd1b9bb64d00bac395e1a56c0093?pvs=4<br>
  - <b>피그마</b> : https://www.figma.com/design/3Knu77CbkAbGge2jrBXQds/honey-touse?node-id=0-1&t=w161YF54HWFuTJ1F-1
  - <b>포지션별 Github</b>
    - 프론트엔드 : https://github.com/HoneyTouse/HoneyTouse_FE
    - 백엔드 : https://github.com/HoneyTouse/HoneyTouse_BE

- ### 기술 스택
  - <b>프론트엔드</b> : HTML, CSS, JavaScript, Vite
  - <b>백엔드</b> : Node.js, Express, MongoDB, JavaScript
  - <b>배포</b> : AWS S3, Route53, Cloudfront, EC2, Github actions appleboy/ssh-action

---

## 스토리보드

![image](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/9d4fee41-ac09-437d-9576-40bd5e581113)

---

## 페이지 구성

|                                                                          메인 페이지                                                                          |                                                                       카테고리별 페이지                                                                       |
| :-----------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------------------: |
|    <div style="text-align: center;">![메인페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/ea31d850-53d9-4c8d-a906-119861baeb77)</div>    | <div style="text-align: center;">![카테고리별페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/09e5bb0f-38fa-467c-9b81-0acbb01f55e8)</div> |
|                                               <b><div style="text-align: center;">상품별 상세 페이지</div></b>                                                |                                                 <b><div style="text-align: center;">장바구니 페이지</div></b>                                                 |
| <div style="text-align: center;">![상품별상세페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/c680f57c-2ae3-4b04-80c4-f62edcfa9391)</div> |  <div style="text-align: center;">![장바구니페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/095b3366-ac62-42b7-b290-b5ef2d1ff3d9)</div>  |
|                                                <b><div style="text-align: center;">주문/결제 페이지</div></b>                                                 |                                                 <b><div style="text-align: center;">주문내역 페이지</div></b>                                                 |
|  <div style="text-align: center;">![주문결제페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/9911657a-4fd4-4696-b1cf-e72aae781b23)</div>  |  <div style="text-align: center;">![주문내역페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/40a07b7b-b38c-4d77-9489-031859f5811f)</div>  |
|                                                   <b><div style="text-align: center;">마이페이지</div></b>                                                    |                                                     <b><div style="text-align: center;">관리자 페이지</b>                                                     |
|    <div style="text-align: center;">![마이페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/11d56aac-64f7-4d68-ac6a-4886a88bff26)</div>    |   <div style="text-align: center;">![관리자페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/ce92ae5c-3590-4948-9a1c-9e031ee7c949)</div>   |
|                                                  <b><div style="text-align: center;">로그인 페이지</div></b>                                                  |                                                    <b><div style="text-align: center;">회원가입 페이지</b>                                                    |
|   <div style="text-align: center;">![로그인페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/d15483eb-7e3a-4d8a-baa0-48d4117bece2)</div>   |  <div style="text-align: center;">![회원가입페이지](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/5b6f5c5c-e763-4c9b-9122-9a22ab9c97f7)</div>  |

---

## 주요 구현 내용

| 프론트엔드                                           | 백엔드                                      |
| ---------------------------------------------------- | ------------------------------------------- |
| • 깔끔한 UI와 산뜻한 디자인, 페이지마다 대표 파비콘 연결                          | • 유지 보수성을 향상시키는 모듈화 구조 설계 |
| • 외부 라이브러리를 거의 사용하지 않은 순수 CSS 구현 | • 회원과 비회원의 주문 내역이 구분되어 관리 |
| • 검색 SEO를 위한 메타태그 및 사이트맵 등록                   | • jwt, 구글 OAuth를 통한 간편한 로그인              |
| • 장바구니 및 최근 검색어 저장 기능 구현             | • 이메일 인증을 통한 보안 강화               |
| • 관리자 페이지 구현             | • multer를 활용한 이미지 처리               |

---

## 기능 설명

### ✅ 상품 탐색을 즐겁게 만드는 메인페이지 UI

- 귀여운 분위기의 사용자 친화적인 디자인
- 화면 상단에서 최신 입고된 상품 확인 가능
- 화면 하단에서 MD가 추천 상품을 카테고리별로 클릭하여 조회 가능
- 상품에 마우스를 올리면 상품 이미지가 확대되어 사용자의 시선을 주목시킴
- 최근 검색 내역을 저장하여 재방문시 검색 내역 확인 가능 **_(Local Storage)_**
<details>
<summary><b>메인 페이지 - 접속</b> (시연 GIF)</summary>
<div markdown="1">

![메인페이지-접속](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/448bfe7f-9dab-4573-9fb2-be274684379a)

</div>
</details>
<details>
<summary><b>메인 페이지 - 카테고리 선택 후 상품 둘러보기</b> (시연 GIF)</summary>
<div markdown="1">

![메인페이지-카테고리](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/4bf52dc4-fd6c-45e7-bc94-ff9e5e9d4ddb)

</div>
</details>
<br>

### ✅ 상품 선택과 구매가 쉬운 상세 페이지 UI

- 상품별 옵션 지정 가능
- 옵션을 선택 시 장바구니 담기 및 바로구매 가능
- 상품 개수를 버튼으로 조절할 때마다 자동으로 주문금액이 계산되어 화면에 표시
- 개별 상품에 대한 상세 정보는 이미지로 확인 가능
<details>
<summary><b>상세 페이지 - 접속</b> (시연 GIF)</summary>
<div markdown="1">

![상세페이지-접속](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/16a849e7-59da-408d-912e-8fe629047ec3)

</div>
</details>
<details>
<summary><b>상세 페이지 - 장바구니 담기</b> (시연 GIF)</summary>
<div markdown="1">

![상세페이지-장바구니담기](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/76691d7a-2c72-49bd-a879-a54c8f8bda3b)

</div>
</details>
<br>

### ✅ 마이페이지 서비스

- 회원 정보를 확인하고 프로필 관리<i>(프로필 이미지, 비밀번호)</i> 가능
- 배송 상태별 주문 수량을 확인 가능
- 최근 주문 정보 확인 가능
<details>
<summary><b>마이 페이지 - 주문내역 조회</b> (시연 GIF)</summary>
<div markdown="1">

![마이페이지-주문내역조회](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/56fb027e-9a76-4dac-bec8-bdc1d07f6a69)

</div>
</details>
<details>
<summary><b>마이 페이지 - 비밀번호 변경</b> (시연 GIF)</summary>
<div markdown="1">

![마이페이지-정보변경](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/b82c7bc7-ad1d-42eb-9daf-67450bd66922)

</div>
</details>
<details>
<summary><b>마이 페이지 - 프로필 이미지 변경</b> (시연 GIF)</summary>
<div markdown="1">

![프로필이미지변경](https://github.com/HoneyTouse/HoneyTouse_FE/assets/127278410/7a544949-4ea9-410d-a30e-3e69ffd7537d)

</div>
</details>
<br>

### ✅ 관리자 권한

- 일반 사용자와 구분되는 관리자 계정을 이용하여 관리자 페이지로 접속 가능
- 모든 회원 정보와 상품 주문 내역 조회 가능
- 상품은 배송 상태별로 분류하여 조회 가능
- 상품 및 카테고리 관리 기능 (추가, 수정, 삭제)
<details>
<summary><b>관리자 페이지 - 비회원 또는 일반 회원 접속</b> (시연 GIF)</summary>
<div markdown="1">

![관리자페이지-비회원(배)](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/920f276c-a6f4-43eb-9721-974382ba3138)

</div>
</details>
<details>
<summary><b>관리자 페이지 - 회원 정보 조회</b> (시연 GIF)</summary>
<div markdown="1">

![관리자페이지-회원정보조회](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/0666bf95-7d90-4d97-b5fe-1ae0e85b8a27)

</div>
</details>
<details>
<summary><b>관리자 페이지 - 배송상태별 주문조회</b> (시연 GIF)</summary>
<div markdown="1">

![관리자페이지-상품배송상태조회](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/baa538cd-b4ba-42c9-86e9-8bf104592bb0)

</div>
</details>
<details>
<summary><b>관리자 페이지 - 상품 배송상태 변경</b> (시연 GIF)</summary>
<div markdown="1">

![관리자페이지-상품배송상태변경](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/f37b0820-bdd4-41fa-a680-66526ff78768)

</div>
</details>
<details>
<summary><b>관리자 페이지 - 카테고리 관리</b> (시연 GIF)</summary>
<div markdown="1">

![관리자페이지-카테고리관리](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/967fddae-92f6-440d-94e4-84b4f4a8f07d)

</div>
</details>
<br>

### ✅ 주문/결제

- 장바구니에 상품 담아두기 가능 **_(Local Storage)_**
- 장바구니 리스트 중 선택적으로 구매 가능
- 비회원도 장바구니, 쇼핑 및 결제 가능
- 결제금액 확인, 개인정보 약관 동의해야만 주문 가능
- 회원은 가입 정보와 연동하여 결제 정보를 저장
- 비회원은 주문 시 입력한 정보를 기반으로 결제 정보를 저장
<details>
<summary><b>주문/결제 - 비회원</b> (시연 GIF)</summary>
<div markdown="1">

![주문-비회원](https://github.com/TripTeller-repository/.github/assets/127278410/a052027c-6fc5-4350-aebc-e3a6e15fbe78)

</div>
</details>
<details>
<summary><b>주문/결제 - 회원</b> (시연 GIF)</summary>
<div markdown="1">

![주문-회원](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/f97eb00f-f2b1-4792-9100-5b2742562bb6)

</div>
</details>
<br>

### ✅ 회원가입

- 고유한 이메일 주소를 활용한 회원가입
- 회원정보(이메일, 비밀번호 등)에 대한 유효성 검사 실시
- 입력한 이메일로 인증번호 발송 및 확인 가능 (구글, 네이버 등) **_(Node mailer)_**
- 인증번호는 5분 이내에만 유효하도록 하여 보안 강화
<details>
<summary><b>회원가입 - 폼 입력부터 메일 인증, 로그인까지</b> (시연 GIF)</summary>
<div markdown="1">

![회원가입-정상](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/b75f0f91-f138-4a03-b569-2344ff4a5fc8)

</div>
</details>
<details>
<summary><b>회원가입 - 이메일 미인증 5분 경과시 인증번호 무효</b> (시연 GIF)</summary>
<div markdown="1">

![회원가입-5분이상경과1](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/056e6798-619d-4799-bb7f-9d91aa37f835)
<br>

5분 이상 경과시 인증번호가 무효가 됨.
<br>

![회원가입-5분이상경과2](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/ab05af26-8397-4d12-a2a7-a496c217b268)

</div>
</details>
<br>

### ✅ 로그인

- JSON Web Token 라이브러리를 이용하여 토큰 기반의 인증을 수행
- 구글 OAuth를 활용한 소셜 로그인 구현 <br>
  (액세스 토큰을 쿠키에 저장하고 SSL 인증을 처리함)
<details>
<summary><b>로그인</b> (시연 GIF)</summary>
<div markdown="1">

![로그인](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/2aa5b8a0-4d14-432f-9630-8da9817ebd42)

</div>
</details>
<details>
<summary><b>구글 소셜 로그인</b> (시연 GIF)</summary>
<div markdown="1">

![구글소셜로그인](https://github.com/user-attachments/assets/b6bb8707-4538-4a43-bdd5-d37a5a6c7256)

</div>
</details>
<details>
<summary><b>로그아웃</b> (시연 GIF)</summary>
<div markdown="1">

![로그아웃](https://github.com/HoneyTouse/HoneyTouse_BE/assets/127278410/1e03cb9b-a8ed-462d-b502-db2c7510d575)

</div>
</details>

---

## 참고 링크

- <b>사이트 제작에 참고한 레퍼런스 사이트</b>
  - KREAM 크림 : https://kream.co.kr/
  - 오늘의집 : https://ohou.se/
- <b>Google Cloud API Console</b>
  - OAuth를 활용한 소셜로그인 구현을 위함.
  - https://console.cloud.google.com/apis/dashboard?pli=1
- <b>Google Cloud Search Console</b>
  - 제작한 사이트의 구글 검색 노출을 위함.
  - https://search.google.com/search-console/about
