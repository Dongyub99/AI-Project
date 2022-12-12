# AI-Project
## 마스크 착용 유무 판별기
---
## 주제
* ##### 웹캠을 이용하여 사람의 마스크 착용 유무를 판단하는 모델 실현
---
### 주제선정
* ##### 코로나 팬데믹 사태로 인해 현재까지도 마스크 착용이 의무화 되고 있다.
* ##### 마스크 착용유무를 사람이 일일이 확인할려면 번거롭고 비효율적이기 때문에 사람들이 마스크를 착용하였는지 안하였는지 판단하는 마스크 식별 모델을 만들어서 카메라로 자동으로 인식하는 시스템을 만들었다.
---
### 라이브러리
- TensorFlow 2+
- OpenCV
- numpy
- matplotlib
---
### 작동 방식
- 웹캠에 얼굴을 보이면 마스크 착용 유무를 확인함
- 마스크 착용시 라임색 박스와 확률이 출력되고, 미착용시 빨갠색 박스와 확률이 출력됨
- 2명 이상의 인원이 있어도 각각의 착용유무가 출력이 됨
- 마스크의 색깔 상관없이 유무 판별 가능
---
### 만드는 과정
<img src="https://user-images.githubusercontent.com/112042668/207055062-83553c82-92d9-4692-ab05-800cfd918058.png" width="200px" height="200px" title="11" alt="11"></img>
##### 일반적인 사람의 사진을 구한다
<img src="https://user-images.githubusercontent.com/112042668/207055076-3499039f-579d-4334-9aed-21ce86f54c10.png" width="200px" height="200px" title="11" alt="11"></img>
##### OpenCV의 딥 러닝 방식으로 사진속의 얼굴을 검출
<img src="https://user-images.githubusercontent.com/112042668/207056343-5215bac3-9805-4504-bfe3-518eabbe3ed8.png" width="200px" height="200px" title="11" alt="11"></img>
<img src="https://user-images.githubusercontent.com/112042668/207056360-6756fe12-54b9-47ec-8244-e587ee8590c6.png" width="200px" height="200px" title="11" alt="11"></img>
##### 검출된 얼굴사진을 facial landmark detection을 통해 검출 후 마스크 이미지를 검출된 landmark에 씌워 데이터셋을 만든후 학습을 시켜 마스크 인식 판별기를 만든다
---
<img src="https://user-images.githubusercontent.com/112042668/207058286-cd1b1c47-aa1b-44d9-84f4-f0870ae80665.png" width="800px" height="400px" title="11" alt="11"></img>
---
<img src="https://user-images.githubusercontent.com/112042668/207058661-9e1d5ae8-a44f-40d8-ba8d-739b1c4e8377.png" width="800px" height="400px" title="11" alt="11"></img>
---
<img src="https://user-images.githubusercontent.com/112042668/207058816-86850771-6a41-49b2-9638-f5c0ac2eed98.png" width="800px" height="400px" title="11" alt="11"></img>
---
<img src="https://user-images.githubusercontent.com/112042668/207058971-9691f280-995d-4610-8023-2f435cbb29fe.png" width="800px" height="400px" title="11" alt="11"></img>
### 작동영상
[:video_camera:혼자일때](https://youtu.be/DoUi6i3doAg)
[:video_camera:2명일때](https://youtu.be/oPvfWP84s1U)
---
