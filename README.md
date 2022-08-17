# VRProject
## 0. 프로젝트 구성원 (최미수, 왕성민, 정현기, 이서희)
 - 기술 총괄 : 이서희
 - 기획 총괄 : 최미수
 - 운영 총괄 : 정현기
## 1. 계획 일정
 - 8월 전체적인 프로토타입 완성
 - 9월 수정 및 구체화
 - 10월 완성시키기
## 2. 필요한 중요한 기술
### 2-1. 주 사업이 번역이 있으면 효율이 좋은 산업에 활용하라. 
### 2-2. 자기 회사제품을 3D화 해서 소개할 수 있는 산업에 활용하라.
### 2-3. 전시회 같은 것으로 활용하라.
- 화면공유 필
- 판매하고자 하는 제품의 3D 모델링을 화면에 표현
- 번역프로그램 (파파고, 구글) 를 이용해 실시간 번역이 가능 / 실시간 채팅번역
- 웹RTC 혹은 Agora.io를 이용해서 화상, 음성 띄우기
- Photon Server에 대한 이해
## 3. 부가적 기술
- FBX 파일을 배치시키기 (전시회)
- Open CV를 이용한 얼굴인식  (캐릭터에 얼굴을 입히는 방식) / 자기만의 캐릭터 만들기
- 각 Room에 맞는 분위기 조성
## 4. Scene 구성 및 필요 기능
 ### 01.Intro : Concept 주위를 구경할 수 있게하고 입구에 UI구성 
 - 로그인/회원가입/입장, 가상키보드 구현 / 주요 스크립트 : Intro Manager.cs 
 ### 02.Server : Concept 복도를 걷다가 각 기업의 매장을 구성 
 - ( A / B / C Company ) 원하는 기업 선택 후 Join Room 클릭시 다음 03 Scene 이동 / 주요 스크립트 : Server Manager.cs
 ### 03.Lobby : 각 기업의 특성에 따라 카테고리(방 제목) 분류 한 룸 생성 (최대 인원 설정 필요)
 - BackGround에 깔끔한 이미지 혹은 기업이미지 / 주요 스크립트 : Lobby Manager.cs, Information.cs, LobbyCount.cs, Data.cs
 ### 04.Show : Concept 기업의 전시회장 및 회의장
 - 회의공간에서 화면공유 및 번역 구현하기 / 전시장에서 제품 상세 설명페이지로 이동, 구매 구현하기 
 - 주요 스크립트 : PlayerMove.cs, GameManager.cs, DetailManager.cs, ButtonManager.cs, ~
 ### 05.Detail : Concept 제품의 상세 모델링 Scene
 - 제품을 상하좌우 늘리기 줄이기를 할 수 있게 하기
 - 주요 스크립트 : SizeManager.cs
 - 모든 Scene에는 뒤로가기 버튼 UI 필요 (LeaveManager.cs)
## 5. 진행사항
### 8월 1주차 목표 : 방을 구성, 보이스챗 가능하게 하기, 캐럭터 움직이기, 화면공유
#### 1주차 발표 내용 : 개론, 2주 뒤의 결과, 핵심기술, 게임성 컨텐츠 요소
#### Day 1-1
- Photon Setting을 통해 회원가입 / 로그인 로그인 시 Lobby로 이동
- Photon Lobby 구현 / 이름, 지역 입력 후 Room 이동
- Photon Room 구현 / 방 생성, 최대 인원, 방파괴 설정 Game 이동
- Photon Game 구현 / 대면 할 수 있는 공간마련
- 추가해야 할 과제 : Photon Game에서 나가기 기능
- 앞으로 해야할 과제 : Photon server 심화, 파파고 API 공부, 웹RTC에 대한 공부
#### Day 1-2 (2022/ 7/ 31) (수정해야 할 사항 있음.) 
- Photon Game Scene에 Window Screen 화면 공유 구현 (다른 스크린 공유도 가능 / 활용 방안 생각해보기)
- Photon Game Scene에 Exit 버튼 (수정 해야할 부분 : Master가 없어지는지 재접속시 화면공유가 없어짐.)
- Photon Game Scene의 채팅창 글씨크가 해상도 강제 조절 후 이상해짐 (수정 요망)
- 기존 UI 조금 수정
- 디스코드 회의 내용
- 1. Photon 서버 기능, Script에 적용되는 명령어 이해하기
- 2. 파파고 API 기능 적용하기
- 3. 3D 제품 업로드 가능하게 하기
- 4. PC, 모바일, VR 연동 가능하게 하기 (현재 Zoom은 PC와 모바일이 연동이 가능하다.)
- 5. 플랫폼에 대한 해상도 적용하기
- 6. 방 구성을 좀 더 다양하게 하기
- 7. 현재 나와있는 Zoom(성민), Google 미팅(서희), 디스코드(미수), 팀뷰어, MicroSoft Teams(현기)에 대해서 조사해보기
#### Day 1-3 (2022 /8 /1)
 - 프로젝트 시작
 - 추가했으면 하는 사항 : 채팅방에 입장/퇴장 표시 (색을 이용해서 눈에 띄게), 현재 인원 보이게 하기
 - 사용자 간의 최적화가 필요하다 (매우 중요)
 - 모르는 사람이 접근을 해도 UI/UX 부분에서 충분히 설명이 필요하다
 - 다른 플랫폼이 가지지 않은 차별점을 비교 분석하면 더 좋을 것이다
#### Day 1-4 (~2022/ 8 /5)
 - Google Translate API 적용해보기 (~작업중) 
#### Day 2-1 (2022/ 8/ 8)
 - Unity version 다운 후에 Room에서 Game이 안들어가는 버그 발생 (~수정중)
 - API 적용시 너무많은 UI들이 존재 줄일 방안 검토
 - 컴퓨터, 안드로이드 버전 / VR 버전을 나누어 만든 후에 만나지게 하기 (공부 중)
### 8월 2주차 : 3,4주차 목표 VR를 중점으로 한 ShowRoom 새로만들기 / Scene 구성, Photon 연동, 3D 모델링 업로드 하기 (PPT 자료)
#### Day 2-2 (2022/ 8/10)
 - 팀원과 상의 후 현재 프로젝트를 갈아 엎고 VR로 가상 전시회 구성하기
 - 참고 : VR CHAT 전시, XR interaction, ShowRoom 구성, Photon Server
 - 구현 할 기술 : 결제 시스템, Charactor 번역, 가상공간에서의 3D modeling 보여주기 
 - ![01  첫 구성](https://user-images.githubusercontent.com/102361334/183945710-ef438c4a-fd73-4e64-8e83-541b6357951b.png)
 - ![02  Main ShowRoom](https://user-images.githubusercontent.com/102361334/183945738-28309fb5-7865-480b-8095-4770b7ddfbca.png)
 - ![03  3D 상세보기](https://user-images.githubusercontent.com/102361334/183945780-d09e106a-51bd-485d-98cc-d6b27cec3a18.png)
 - ![04  결제 시스템](https://user-images.githubusercontent.com/102361334/183945816-e6142cf9-9a2e-4f17-97bc-401931910743.png)
 - ![05  캐릭터 번역](https://user-images.githubusercontent.com/102361334/183945850-0eb8b6c6-9766-45ac-ba89-66e95c149598.png)
#### Day 2-3 (2022/ 8/ 13~14)
 - Android, Oculus Quest2 세팅으로 새롭게 만들기
 - 01.Intro Playfab으로 회원가입, 로그인 하게 하기 / Photon 연동
 - 02.Server A B C Company를 선택하고 접속하게 하기
 - 03.Lobby 각 Company의 로비에 접속
 - 04.Show 메인 전시장/회의실이 있는 ShowRoom에 접속
 - Canvas 를 WorldSpace로 구성, UI 맞춰넣기 (쉽지 않음.)
 - Blender로 각 Scene에 맞는 모델링 하기
#### Day 2-4 (2022/8/15)
 - 04.Show Scene에 Charactor 만들기 (완료) / 제품 설명 UI 띄우기 / 05.Detail Scene Load 필요
 - 05.Detail Scene 필요 (제품 상세 모델링)
### 8월 3-4주차 토론, 해결해야하는 내용 Scene 별로
 - 전체적 문제 : Scene UI배치, Prefab Modeling, VR Controller 띄우기
 - 01.Intro : 로그인 UI를 클릭시 나타나게 하기
 - 02.Server : UI 위치에 따른 마우스 클릭 위치가 다름. UI 위치 조정 필요
 - 03.Lobby : UI를 두개로 구성? 1. 방 리스트 UI 2. Join, Create UI
 - 04.Show : 캐릭터가 VR로 움직여지는지 / 사진들 마다 UI 배치, 버튼 클릭시 다음 Scene로 넘어가기, 결제 UI 띄우기 / 제품 상세 설명 UI 만들기
 - 05.Detail(1~5) : 제품 3D 모습을 볼 수 있게 배치하기

