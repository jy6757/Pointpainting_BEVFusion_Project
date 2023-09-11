# JoJoOne[Team1]


 Draft for fusion of two models and heading extraction of BEV Fusion model result

---

발표자 : 김정민, 임지연

---

## 목표

⭐ Sensor Fusion을 통한 **3D Object Detection, Segmentation**

⭐ BEV Fusion 앞단 부분의 Fusion 방식 변경

⭐ PointPainting 모델을 활용하여 LiDAR Point Cloud Painting

⭐ 그 결과 나온 LiDAR Painting을 BEV로 변환 

⭐ Pointpainting된 point cloud를 이용하여 원하는 클래스에 해당하는 point만 남기고 복셀화 진행

⭐ BEV로 변환된 LiDAR Point를 BEV Fusion Shared-BEV Encoder 형태로 Encoding

⭐ **Heading** 시각화

---

1. **BEV Fusion을 main으로 진행 → SensorFusion 방법을 변경해보며 성능 비교**
    - BEVFusion : Multi-Task Multi-Sensor Fusion with Unified Bird’s-Eye View Representation
    - PointPainting: Sequential Fusion for 3D Object Detection

     [모델을 변경함으로써 확인해보고자 한 것]


    1. 복셀화 범위를 줄임으로써 계산량 측면에서 효율성을 갖게 되는지, 불필요한 포인트까지 복셀화가 되지 않으므로 원하는 객체를 가리는 부분이 줄어듦으로써 성능 향상에 영향을 미치는지?
    2. 이미지를 BEV Tranform시키지 않기 때문에 이미지 정보의 변형이나 손실 없이 사용함으로써 성능 향상에 영향을 주는지?
    3. 기존 Pointpainting 모델의 성능과 Pointpainting된 Point Cloud들을 BEV로 변환시켰을 때를 비교하여 World 좌표계 정보를 훨씬 더 많이 담고있는 BEV를 사용하는 것이 더 좋은지?
    4. 결론적으로 Pointpainting의 장점과 BEV Fusion의 장점들을 결합할 수 있는 모델인지?

       
1. BEV Fusion의 결과물에 추가적인 알고리즘 개발
    - 장애물의 위치, 크기, Heading, 예상되는 움직임
  
## 역할 분배
1. 논문 및 코드 분석 
    - BEV Fusion → [김정민](https://www.notion.so/ad5c97f9c6d540a1ba6d56802210863d?pvs=21), [허정은](https://www.notion.so/1d9da9c2e8e040f0833d92a3854016ca?pvs=21)
    - Frustum PointNets → [김민지](https://www.notion.so/29d90ef4b671431b8f2b3631bb3a3793?pvs=21), [임지연](https://www.notion.so/454c60072b6643a6925af1ef5b3dc81d?pvs=21)
    - Pointpainting → [임지연](https://www.notion.so/454c60072b6643a6925af1ef5b3dc81d?pvs=21)
2. 모델 개선 방법론 제안 및 구현 →[임지연](https://www.notion.so/454c60072b6643a6925af1ef5b3dc81d?pvs=21)
3. 환경 구축 및 디버깅 / 프로세스 실행 및 수정  →[김정민](https://www.notion.so/ad5c97f9c6d540a1ba6d56802210863d?pvs=21)
4. Heading 추출 구현→ [김민지](https://www.notion.so/29d90ef4b671431b8f2b3631bb3a3793?pvs=21),[허정은](https://www.notion.so/1d9da9c2e8e040f0833d92a3854016ca?pvs=21)


## 기술 스택

`Python` `pytorch` `cuda` `Docker`
