# 🥇🥈🥉 스마트 올림픽 (Smart Olympic)
**교실과 가정을 뒤집어 놓을 100% 온디바이스(On-device) AI 모션 인식 체육 웹앱**

![스마트 올림픽 썸네일](media/logo.png) ## 🚀 서비스 링크 (Demo)
👉 **[스마트 올림픽 바로가기](https://smart-olympic.vercel.app/)**

---

## 📖 프로젝트 소개
**스마트 올림픽**은 초등학교 체육 수업(건강 및 도전 영역)을 위해 개발된 웹 기반 AI 모션 인식 프로그램입니다. 코로나 이후 줄어든 학생들의 신체 활동량을 늘리고, 자기주도적인 체력 단련을 독려하기 위해 기획되었습니다. 

별도의 앱 설치나 회원가입 없이, 노트북이나 스마트패드의 **웹 브라우저와 웹캠**만 있으면 누구나 즉시 6가지 다채로운 체육 종목에 참여할 수 있습니다.

---

## ✨ 주요 기능 및 특징

### 1. 🛡️ 100% 온디바이스(On-device) 개인정보 보호
* **No Server, No DB:** 학생의 카메라 영상 및 이름 데이터는 외부 서버로 1바이트도 전송되지 않습니다.
* **Privacy by Design:** 오직 웹 브라우저 메모리 내에서만 실시간으로 연산되며, 브라우저 종료 시 영구 파기되어 학교 현장에서 개인정보 유출 걱정 없이 안전하게 사용할 수 있습니다.

### 2. 🏃‍♂️ 6대 체력 요소를 반영한 맞춤형 종목
* **100m 달리기 (순발력):** 발구름 속도를 스마트하게 계산하여 전진
* **50m 수영 (심폐지구력):** 양팔을 끝까지 저어주는 동작 인식
* **30초 체조 (근지구력):** 팔벌려뛰기 4박자(옆-차렷-위-차렷) 정확도 판정
* **30초 복싱 (민첩성):** 뻗어 나가는 주먹의 가속도를 인식하여 타겟 타격
* **송판 격파 (유연성):** 하이킥 모션을 인식하여 송판 격파 파티클 효과 제공
* **서핑 밸런스 (평형성):** 어깨의 무게 중심 이동을 통한 아케이드 미니 게임

### 3. 🎥 오디오가 포함된 영상 기록증 발급
* Canvas API를 이용한 실시간 화면 렌더링에 Web Audio API 기반의 **오디오 라우팅 기술**을 결합했습니다.
* 플레이 종료 후, 신나는 BGM과 효과음이 그대로 담긴 **'나만의 플레이 영상'** 및 **'기록증 이미지'**를 로컬 기기로 다운로드할 수 있습니다.

---

## 🛠️ 기술 스택 (Tech Stack)
* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **AI Model:** [Google MediaPipe Pose](https://google.github.io/mediapipe/solutions/pose.html) (인체 뼈대 랜드마크 실시간 추출)
* **Media & Graphics:** HTML5 `<canvas>`, Web Audio API, `MediaRecorder` API
* **Deployment:** Vercel

---

## 📂 프로젝트 구조 (Directory Structure)
📦 smart-olympic
 ┣ 📜 index.html        # 메인 대시보드 및 종목 선택 화면
 ┣ 📜 sprint.html       # 100m 달리기
 ┣ 📜 swim.html         # 50m 자유형 수영
 ┣ 📜 gymnastics.html   # 30초 체조 (팔벌려뛰기)
 ┣ 📜 boxing.html       # 30초 복싱
 ┣ 📜 taekwondo.html    # 송판 격파
 ┣ 📜 surfing.html      # 서핑 밸런스
 ┗ 📂 media             # BGM, 효과음, 로고 이미지 폴더

## 💻 로컬 실행 방법 (Getting Started)
이 프로젝트를 로컬 환경에서 실행하고 테스트하려면 다음 단계를 따르세요.

1. 저장소를 클론(Clone)합니다.
```bash
git clone [https://github.com/Kimmahone/smart-olympic.git](https://github.com/Kimmahone/smart-olympic.git)
```
2.프로젝트 폴더로 이동합니다.
```bash
cd smart-olympic
```
3. 웹 서버 환경에서 실행합니다. (카메라 권한을 얻기 위해 로컬 서버가 필요합니다.)
VS Code 사용자: Live Server 익스텐션을 사용하여 index.html을 엽니다.
Python 사용자: python -m http.server 8000 실행 후 브라우저에서 localhost:8000 접속

🧑‍🏫 개발자 및 라이선스
기획 및 개발: 5학년 담임교사 김정준
문의: kimjj0709@gmail.com
개인정보 처리방침: 본 앱은 상업적 목적이 없는 교육용 소프트웨어이며, 개인정보를 수집하지 않습니다. (메인 페이지 하단 참조)
