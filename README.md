# 1. Camera Calibration  
OpenCV를 이용한 카메라 캘리브레이션 도구입니다.  
체스보드 패턴이 포함된 영상을 통해 내부 카메라 파라미터와 왜곡 계수를 추정할 수 있습니다.

## 🎯 주요 기능  
- 영상 프레임에서 체스보드 코너 자동 검출
- 서브픽셀 정밀도 보정을 통한 코너 정확도 향상
- 카메라 파라미터 추정:
  - 내부 파라미터 행렬 (K)
  - 왜곡 계수 (방사/접선 왜곡)
  - 재투영 오차 (RMS)
- 이미지 선택 시 실시간 시각화
- 이후 왜곡 보정이나 증강현실, 3D 비전 작업에 활용 가능

---

## 🛠️ 출력 예시 (결과)

![image](https://github.com/user-attachments/assets/95f75d4a-8c9d-42a7-8439-b081cfd2e8fc)


![image](https://github.com/user-attachments/assets/314ba48b-468d-4671-97c1-e5358b31785a)


# 2. distortion correction

## 🎯 주요 기능

- 캘리브레이션 결과(K, 왜곡 계수)를 이용한 왜곡 보정
- `cv.initUndistortRectifyMap()`과 `cv.remap()`을 이용한 실시간 보정 처리
- `Tab` 키를 이용한 원본/보정 영상 전환
- 영상 스트림 형태의 입력에 대응

---

## 🛠️ 결과
![image](https://github.com/user-attachments/assets/52213cd4-80fc-414e-beb4-1cc00192e456)
