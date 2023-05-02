[2188801.github.io](2188801.github.io)
=======================================

프로젝트명 : Dream of PyoungSick jo
===================================
블로그 업데이트 중

[목차]
----
1. [\[컨셉\]](#컨셉)
    - [메인컨셉 : 트라우마](#메인컨셉--트라우마)
    - [서브컨셉 1 : 탈출](#서브컨셉-1--탈출)
    - [서브컨셉 2 : 공포감](#서브컨셉-2--공포감)
    - [서브컨셉 3 : 학교](#서브컨셉-3--학교)
    - [서브컨셉 4 : 성취감](#서브컨셉-4--성취감)

<br>

2. [\[대표 이미지\]](#대표-이미지)

<br>

3. [\[컨셉 & 대표이미지 기반 작품묘사\]](#컨셉-대표이미지-기반-작품묘사)

<br>

4. [\[구성 요소\]](#구성-요소)

<br>

5. [\[게임 시스템 디자인\]](#게임-시스템-디자인)

<br>

6. [\[개발 요구사항 현황\]](#개발-요구사항-현황)

<br>

7. [\[개발 요구사항\]](#개발-요구사항)

<br>

### [컨셉]
---

### 메인컨셉 : 트라우마
- 플레이어는 캐릭터의 상황에 몰입하여 캐릭터가 트라우마를 극복해 히키코모리 생활을 청산하는 계기가 될수 있도록 도와야합니다.

### 서브컨셉 1 : 탈출
- 한정된 공간에서 플레이어는 탈출하기 위해 공포감 속에서도 지성을 발휘해야 합니다.

### 서브컨셉 2 : 공포감
- 공포감을 조성하는 분위기(배경, BGM)와 이를 더 극대화 할 수 있는 Enemy를 통해 긴장감을 부여합니다.

### 서브컨셉 3 : 학교
- 주 플레이어 연령층을 10대로 겨냥한 만큼 학생들의 공감대를 형성합니다.

### 서브컨셉 4 : 성취감
- 플레이어가 힌트를 통해 문제를 해결했을 때 성취감을 느끼고 다음 스토리로 넘어갈 수 있는 원동력을 제공합니다.

<br>

### [대표 이미지]
---
![Alt text](/gallery/game.png)

<br>

### [컨셉 대표이미지 기반 작품묘사]
---
시작 화면 :

    - 전체적으로 화면을 어둡게 구성하고, 무서운 BGM을 추가해 플레이어가 느끼는 공포감을 극대화 해줍니다.
    - Enemy의 스토리를 통해 긴장감을 부여합니다.

![Alt text](/gallery/enemy1.png)
![Alt text](/gallery/enemy2.png)

게임 화면 :

    - 중앙 하단에 현재 플레이어가 소지한 아이템이 표시됩니다. 
    - 왼쪽 하단에는 플레이어의 체력을 나타내주는 HP바와 이동속도를 제한해주는 SP바가 표시됩니다.
    - 마우스를 이동하여 플레이어의 시야를 변경할 수 있습니다.

![Alt text](/gallery/school1.png)

<br>

### [구성 요소]
---

1. 스토리

- 조평식(23세/男)은 고등학교 시절 학교폭력을 당해 그 트라우마로 히키코모리 생활을 이어가고 있었던 어느 날 그가 눈을 뜨고 일어나보니 어느 교실에 있었다. 혼란에 빠진 조평식은 주변의 공기와 모습들이 자신이 다니던 고등학교라는 것을 알게 되고 우선 주변의 도움을 청하고자 한다. 그때 학교의 이상한 사람 형태를 한 괴물을 마주하게 된다. 조평식은 우선 그것을 피해 도망쳐 물품 보관실에 숨어 그 괴물의 추적을 피한다. 조평식은 자신의 학창 시절에는 존재하지 않던 괴물의 존재에 이 상황이 꿈이라고 추측하게 되고, 꿈에서 깨기 위해 벽에 머리도 박고, 수많은 방법을 시도하던 중 물품 보관실에 우연히 떨어진 쪽지를 발견하게 된다. 쪽지에는 알 수 없는 수수께끼 같은 말이 적혀있었다. 이 쪽지가 이 꿈을 꾸는 이유나 꿈에서 벗어날 수 있게 도움을 주는 것이라는 생각을 하게 된 조평식은 물품 보관실에 있던 손전등을 챙겨 이곳을 탈출하기 위해 움직인다. 그렇게 탈출을 위해 움직이던 조평식은 학교의 괴물들이 자신의 트라우마가 만들어 낸 공포의 집합체라는 것을 알게 된다. 자신의 트라우마를 극복하기 위해 조평식은 학교에 있는 자신에게 트라우마가 있는 물건을 없애려고 한다.

<br>

2. 디자인
- 평범해 보이지만 불규칙적인 식사와 운동을 통해 건강이 나빠보이는 20대 남성의 모델 사용
- 학창시절 학교에서 사용했던 책상, 사물함, 교탁, 칠판같은 익숙한 모델 사용
- 공포감을 극대화 시켜줄 수 있는 으스스한 BGM 사용

<br>

3. 기술
- 물체의 상호작용에 물리엔진을 적용하여 현실적인 물체의 움직임을 구현
- Player, Enemy의 모션과 음향의 싱크를 맞춰 현실성을 부여함

<br>

### [게임 시스템 디자인]
---

![Alt text](/gallery/school2.png)
![Alt text](/gallery/school3.png)
![Alt text](/gallery/school4.png)
![Alt text](/gallery/school5.png)
![Alt text](/gallery/school6.png)
![Alt text](/gallery/school7.png)

<br>

### [개발 요구사항 현황]
---

### **1주차**
 - 제작할 게임에 대한 전체적인 주제를 설정
 - 이 게임 내에서 구현할 기능 및 기능에 따른 각 팀원의 역할을 분담
 - 이를 토대로 Zoom 수업에서 발표를 통한 교수님의 피드백 수용

 ### **2주차**
  - 1주차 교수님의 피드백을 수용하여, 제작할 게임에 대한 세부적인 역할 분담
  - 플레이어(조평식)에 대한 스토리 구현
  - 게임 속 상황을 지루하지 않도록 여러 가지(Enemy 중점) 구현을 보완

 ### **3주차**
  - 게임의 배경과 Player 이동, Enemy 웨이포인트 구현
  - 게임 속 긴장감을 조성하는 사운드를 넣어 공포감을 더욱 극대화

 ### **4주차**
  - 스타트 씬 제작 및 캐릭터 소개창 및 BGM 추가
  -Player와 문 오브젝트의 상호작용 구현

 ### **5주차**
  - Player의 체력, 스태미나 UI 추가
  - Player가 스태미나를 모두 소모한 경우 Player의 속도에 제한을 주는 상호작용 구현

 ### **6주차**
  - 게임 속 배겨이 어두워지는 오류 및 메인 카메라가 흔들리는 오류 수정
  - Player와 Enemy가 서로 상호작용하는 것을 구현 중

 ### **7주차**
  - 게임 내 과학실, 미술실, 교무실, 화장실을 손수 제작하여 추가 에셋 구매 없이 실제 학교의 모습을 구현하고 현실 고증을 이룸
  - Player와 Enemy가 충돌 시 Player의 HP바가 감소하는 상호작용 구현

<br>

### [개발 요구사항]
---
 ### **8주차**
  - Player와 Enemy의 상호작용 구현 예정
  - Player가 흭득할 수 있는 아이템(힌트)에 대한 상호작용 구현 예정

 ### **9주차**
  - Player 인벤토리 구현 예정
  - Enemy가 Player를 인식 후 추적 이동 구현 예정
  - 손전등 구현 예정

 ### **10주차**
  - 새로운 Enemy(교사) 추가 예정
  - Enemy(교사)의 새로운 공격 패턴 및 디버프 구현

 ### **11주차**
  - 새로운 Enemy(학생) 추가 예정
  - Enemy(학생생)의 새로운 공격 패턴 및 디버프 구현

 ### **12주차**
  - 게임 클리어 조건 구현 예정
   - 엔딩씬 구현 예정

 ### **13주차**
  - 게임 테스트 및 버그 수정

 ### **14주차**
  - 게임 테스트 및 버그 수정

 ### **15주차**
  - 결과 발표