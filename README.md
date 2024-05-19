<!-- 프로젝트명 -->
# Netflix Clone Coding


<!-- 프로젝트 요약 설명 -->
`Netflix 메인과 상세 페이지를 JavaScript와 React를 사용하여 클론 코딩하는 프로젝트`


<!-- 프로젝트 로고 이미지 -->
<div align="center">
  <a href="">
    <img src="https://github.com/front01team/our-netflix/assets/111291076/c4879cab-a6a2-433c-9df7-c5dcad76aeb0" width="300px"/>
  </a>
</div>


<!-- 프로젝트 기술스택 뱃지 -->
<div align="center">
  <img src="https://img.shields.io/badge/javascript-F7DF1E.svg?style=flat&logo=javascript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB.svg?style=flat&logo=React&logoColor=white" />
  <img src="https://img.shields.io/badge/styled components-DB7093.svg?style=flat&logo=styled-components&logoColor=white" />
</div>


<!-- Demo/메인 이미지 -->
# Main Screen
`데모영상`  https://youtu.be/Y9TaMagiEJ4

<div align="center">
  <img src="https://github.com/front01team/our-netflix/assets/111291076/66f54ad0-a993-4ff8-b863-d6264cf3d7ab" width="100%"/>
</div>


<!-- 프로젝트 개요 -->
# Overview
> **1. 프로젝트 기획 이유**  
: 넷플릭스 메인 페이지와 상세 페이지를 클론 코딩해보면서 React, JavaScript, styled-components 이해를 높이고, 영상과 이미지 다루는 연습 수행  
>  
> **2. 프로젝트 기간** : 2024. 03. 04 ~ 2024. 03. 08 (5일)  
>  
> **3. 프로젝트 수행 인원** : 프론트엔드 3명
>   
> **4. 개발환경**  
> * FrontEnd : JavaScript, React, styled-components  
> * 버전 관리 및 협업 : Git & Github, Notion, Figma  
> * 배포 : Vercel
>
> **5. Branch 전략** : Git-Flow (main, develop)
> 
> **6. 프로젝트 특징** : 메인화면 영상 자동재생, Modal로 상세 페이지 구현, React Custom Hook 사용, 크롤링으로 Mock 데이터 수집 & TMDB API 이용
> 
> **7. 프로젝트 배포 링크** : https://our-netflix.vercel.app


<!-- 프로젝트 세부 내용 -->
# Detail


<div align="center">
<table>
  <tr>
    <td><img src="https://github.com/front01team/our-netflix/assets/111291076/a6a3d817-b2b2-490c-b727-6c023476bd94" alt="Image 1" height="300" /></td>
    <td><img src="https://github.com/front01team/our-netflix/assets/111291076/695b4e10-8bdd-44a5-a965-c236dbc0ab6a" alt="Image 2" height="300" /></td>
  </tr>
</table>
</div>


1. Header & Footer  
   * useNavigate를 이용해 메뉴 링크  
   * DropDown Menu 구현  
2. Main Page  
   * TOP 영화 목록 별도 구현  
   * 컨텐츠 목록 슬라이드 구현  
   * 유투브 영상 Path와 iframe 태그를 이용해 영상 재생 구현  
   * 컨텐츠 Click 시, useNavigate로 해당 영상을 볼 수 있는 페이지로 이동시키면서 state값으로 영상 제목 텍스트 전달  
   * 컨텐츠 Hover 시, 해당 영상의 제목으로 TMDB API를 통해 유투브 영상 Path를 찾아서 영상 자동 재생 구현, 이때 useSearchVideo라는 Custom Hook 이용함
   * TMDB API에서 데이터를 받아올 땐, async/await과 fetch 사용
3. Detail Page  
   * Main Page처럼 해당 컨텐츠와 연관된 영상 자동 재생  
   * ReactDOM.createPortal을 이용해 Modal로 구현(모달 외 영역 클릭시 닫힘 구현)  



<!-- 프로젝트 회고 -->
# Retrospective
1. 개선하고 싶은 점
   * 주석 작성, 부분 CSS 코드를 styled-components로 작성
   * 메인 페이지 슬라이드, 컨텐츠 hover시 부드러운 효과 적용, TOP 시리즈, width 조정
   * 상세 페이지 width를 반응형으로 좀 더 상세히 구현
   * 내가 찜한 리스트 페이지 구현
   * Header 검색 기능
2. 회고
   * 적극적인 팀 협업으로 짧은 기간과 처음 해보는 프로젝트였음에도 불구하고 기획부터 구현과 발표까지 완료
   * 백엔드가 없는 상황이었지만 데이터 확보를 다양한 방법으로 해결
   * 초기 기획 단계의 중요성 실감 - 완벽하진 않았어도 초기 기획 단계에서 피그마로 플로우 차트와 폴더구조 등을 미리 정한 것이 큰 도움이 됨
   * React, JavaScript, styled-components, Git & Github(특히 Git-Flow)에 대한 더 깊은 이해와 숙련도 향상
