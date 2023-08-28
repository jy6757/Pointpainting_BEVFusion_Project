# JoJoOne[Team1]
# Pointpainting+BEVFusion Project
 Draft for fusion of two models and heading extraction of BEV Fusion model result

---

## BEV Fusion with PointPainting & Heading Extract

발표자 : 김정민, 임지연

---

## 목표

⭐ Sensor Fusion을 통한 **3D Object Detection, Segmentation**

⭐ BEV Fusion 앞단 부분의 Fusion 방식 변경

⭐ PointPainting 모델을 활용하여 LiDAR Point Cloud Painting

⭐ 그 결과 나온 LiDAR Painting을 BEV로 변환

⭐ BEV로 변환된 LiDAR Point를 BEV Fusion Shared-BEV Encoder 형태로 Encoding

⭐ **Heading** 시각화

---

1. **BEV Fusion을 main으로 진행 → Feature Extractor를 변경해보며 성능 비교**
    - BEVFusion : Multi-Task Multi-Sensor Fusion with Unified Bird’s-Eye View Representation
    - PointPainting: Sequential Fusion for 3D Object Detection
2. BEV Fusion의 결과물에 추가적인 알고리즘 개발
    - 장애물의 위치, 크기, Heading, 예상되는 움직임
  
## 역할 분배
1. 논문 및 코드 분석 
    - BEV Fusion → [김정민](https://www.notion.so/ad5c97f9c6d540a1ba6d56802210863d?pvs=21), [허정은](https://www.notion.so/1d9da9c2e8e040f0833d92a3854016ca?pvs=21)
    - Frustum PointNets → [김민지](https://www.notion.so/29d90ef4b671431b8f2b3631bb3a3793?pvs=21), [임지연](https://www.notion.so/454c60072b6643a6925af1ef5b3dc81d?pvs=21)
    - Pointpainting → [임지연](https://www.notion.so/454c60072b6643a6925af1ef5b3dc81d?pvs=21)
2. 모델 개선 및 구현 →[임지연](https://www.notion.so/454c60072b6643a6925af1ef5b3dc81d?pvs=21)
3. 환경 구축 및 디버깅 / 프로세스 실행 및 수정  →[김정민](https://www.notion.so/ad5c97f9c6d540a1ba6d56802210863d?pvs=21)
4. Heading 추출 구현→ [김민지](https://www.notion.so/29d90ef4b671431b8f2b3631bb3a3793?pvs=21),[허정은](https://www.notion.so/1d9da9c2e8e040f0833d92a3854016ca?pvs=21)


## 기술 스택

`Python` `pytorch` `cuda` `Docker`
