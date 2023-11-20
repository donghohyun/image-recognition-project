# image-recognition-project
자동차 번호판 인식 프로젝트

## 프로젝트 목표
* 이미지에서 자동차 번호판 영역을 검출하고 번호판을 인식하고자 한다.
---
## 데이터 수집
데이터 분석을 위해 크롤링과 AIHub 데이터를 이용하였으며 자체제작한 번호판 3가지를 사용하였다.
<p align="center">
  <img src="https://github.com/donghohyun/image-recognition-project/assets/139213175/7fdebf5c-c688-41c3-8767-c9ea02f17188">
</p>

---

## 이미지 전처리
이미지에서 번호판 영역 추출과 번호를 구분하기 위해 전처리를 거쳐 주었다.
전처리를 크게 N 단계를 거쳤다.
1. 이미지 그레이 스케일 변환
2. 이미지 블러처리
3. 외각선 구하기
4. 문자로 추정되는 contour 찾기

---
## 사전 학습된 모델인 Tesseract OCR 모델을 사용하여 텍스트 추출

