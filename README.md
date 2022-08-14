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
- 화면공유 필수 (웹 RTC만 가능하다고 함.)
- 판매하고자 하는 제품의 3D 모델링을 화면에 표현
- 번역프로그램 (파파고, 구글) 를 이용해 실시간 번역이 가능 / 실시간 채팅번역
- 웹RTC 혹은 Agora.io를 이용해서 화상, 음성 띄우기
- Photon Server에 대한 이해
## 3. 부가적 기술
- FBX 파일을 배치시키기 (전시회)
- Open CV를 이용한 얼굴인식  (캐릭터에 얼굴을 입히는 방식) / 자기만의 캐릭터 만들기
- 각 Room에 맞는 분위기 조성

## 4. 진행사항
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
 - 가상키보드 만들기!
