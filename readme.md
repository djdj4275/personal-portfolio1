# 0. 목차

1. 프로젝트 주제
2. 프로젝트 사용된 스택
3. 프로젝트 기능
4. 프로젝트 작업시 난점 (어려웠던 점)
5. 프로젝트 제한점 (추가해야할 부분)

---

# 1. 프로젝트 주제

### **- Artical -**

평소에 갔던 전시회나 카페의 느낌을 살려 표현해 전시회 소개 느낌의 웹사이트 구현

---

# 2. 프로젝트 사용된 스택

  * HTML
  * CSS
  * Java Script
  * Vue,Vuetify

---

# 3. 프로젝트 기능
1. **마우스 디자인 & 특정 링크 호버시 트랜지션**
![1](https://user-images.githubusercontent.com/99634816/170812394-735a3d0b-4b93-491e-8b3b-f56a43e03a3e.PNG))
2. **상단 네브바 구현**
![2](https://user-images.githubusercontent.com/99634816/170812731-a5d6be96-3a4c-4a12-b8e3-8e49210c59bb.PNG)
3. **특정 컨텐츠 클릭시 모달창 구현**
![3](https://user-images.githubusercontent.com/99634816/170812922-520aa4d3-65eb-49b0-b525-f5d3f64912c7.PNG)
4. **스크롤 이벤트 구현(컨텐츠들 나타남)**
![4](https://user-images.githubusercontent.com/99634816/170812928-22b19c13-4aaa-4bdb-948e-fab863b1d945.jpg)
5. **컨텐츠 설명 타이핑 이벤트 구현**
![5](https://user-images.githubusercontent.com/99634816/170812941-d6738167-41b7-4310-be4e-267a7de1fffa.PNG)
6. **슬라이드쇼 구현**
![6](https://user-images.githubusercontent.com/99634816/170813155-aede02b4-e4f5-487e-b8dc-61ebb29505a3.PNG)
7. **768px 화면에서 사이드 네브바 구현 (트랜지션)**
![7](https://user-images.githubusercontent.com/99634816/170813945-828f12d9-9aad-44c4-9b07-5fffe0177eb5.PNG)


___

# 4. 프로젝트 작업시 난점 (어려웠던 점)
### (1) 타이핑 이벤트 작성시에 줄바꿈시에 문자열 취급으로서 넣어주기때문에 <br> 태그를 먹이기 힘들었던 점**
  * 문자열로 넣어줄때에 <br> 대신 |n (역슬래쉬 n)을 작성하여주고 삼항연산자를 이용하여 타이핑 진행중에 |n이 나오게되면 <br/> 태그를 넣어주도록 하여서 줄바꿈 구현.
### (2) 슬라이드쇼 구현에서 넘기는 모션이 아닌 자동으로 사진이 자연스레 사라졌다 나타나는 애니메이션 구현**
  * 사진들에 공통적인 클래스를 주고 그 클래스를 for문으로 반복하며 display:none으로 해둔다음 setinterval로서 정해둔 시간이 지날때마다 해당되는 index의 슬라이드 사진에만 display속성을 바꾸어 주어 슬라이드 쇼를 구현.
### (3) 마우스 이벤트에서 x,y 좌표를 받을시에 window.addEventListener 에서 scroll 이벤트로 받을시에 좌표의 계산이 올바르게 진행되지 않는점**
 * 현재로는 스크롤로는 계산이 잘되지않는 이유를 찾지 못했습니다. 이 부분에서는 콘솔로 계산되기전 들어오는 좌표값을 찍었을때에 값도 잘 들어왔습니다. 또한 스크롤이벤트가 아닌 mousemove 이벤트의 계산에서는 값이 계산되어서 잘 들어왔습니다. 지금 현재로는 scroll대신에 wheel 이벤트로서 대신하였습니다.

___

# 5. 프로젝트 제한점 (추가해야할 부분)
1. 마우스 이벤트를 스크롤이 아닌 휠로 값을 계산하기에 스크롤시 화면에서 마우스포인터가 살짝씩 밀리는 현상 발생
2. 반응형에서 768px뿐 아니라 사이사이 규격에서도 레이아웃 변경점을 두어 화면이 점차 줄어들때에 레이아웃이 겹치는 부분이 없도록 추가
