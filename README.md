## 최상윤 (Choi Sangyun)

숭실대학교 AI소프트웨어학부 3학년

**관심 분야:** Vision-Language-Action(VLA) 모델 · 로봇 정책 학습 · Open-World Manipulation

📫 sean2373@soongsil.ac.kr

---

### Projects

**NAFNet 기반 스마트폰 렌즈 오염 복원** (2026.03 – 06)
딥러닝프로그래밍 · 개인 프로젝트 · PyTorch (BasicSR)

- NAFNet에 학습 기법 7가지를 차례로 적용하고, 통제 실험으로 SSIM 향상의 원인이 FFT 손실이 아닌 AMP였음을 바로잡음
- 대형 패치는 쉬운 샘플에서, 교차 태스크 사전학습은 어려운 샘플에서 효과가 큼을 관찰하고 5모델 앙상블로 PSNR 23.70 dB 달성 (가장 어려운 구간은 미개선, 원인 분석 포함)
- 🔗 [프로젝트 정리와 보고서](https://github.com/sean237333/nafnet-dirty-lens-restoration)

**QuantPrune-X: 모델 경량화가 백도어를 활성화하는 조건 분석** (2026.10 – 진행 중)
온디바이스 AI 수업 · 5인 팀 · 실험 파이프라인과 ResNet-18 분석 담당 · PyTorch

- 양자화 후에만 작동하도록 백도어가 삽입된 공개 모델(QCB)에 양자화·프루닝을 여러 순서로 적용해, 경량화가 백도어를 활성화하거나 막는 조건을 분석
- 5개 경로(FP32·양자화·프루닝·양자화→프루닝·프루닝→양자화)를 자동 실행하는 파이프라인을 구현해 모델 4개 172건 실행
- ResNet-18에서 프루닝만으로도 백도어가 활성화되고(65% → 70%에서 공격 성공률 27.5% → 95.5%), layer2를 먼저 프루닝하면 INT4 양자화 백도어가 막힘을 확인
- 🔗 [ResNet-18 분석 리포트](https://github.com/zobbo0408/QuantPrune-X/tree/feat/experiment-pipeline/analysis/resnet18/report) · [팀 저장소](https://github.com/zobbo0408/QuantPrune-X)

**ROS 2 로봇 프로그래밍 실습** (2026.03 – 06)
로봇프로그래밍 · ROS 2 Jazzy, Python (rclpy), Webots

- Topic·Parameter·Launch·Service 통신 패키지 6개를 직접 구현 (사용자 정의 서비스 타입, 실행 중 파라미터 변경)
- 수업 제공 Webots 차동구동 로봇 위에서 odom 피드백 360° 회전, LiDAR 장애물 감지 후 후진, 토픽 실시간 검증 노드 작성
- Cartographer로 지도를 작성하고, 저장한 지도로 Nav2 자율 주행 수행
- 🔗 [ros2-robot-programming](https://github.com/sean237333/ros2-robot-programming)

**Amazon 상품 Top-20 추천** (2026.11 – 진행 중)
데이터사이언스 수업 Kaggle 대회 · 4인 팀 · Python, XGBoost, CatBoost, PyTorch

- 팀의 후보 생성 + 랭커 2단계 시스템을 이어받아 개선 실험 수행, 개인 최고 Recall@20 0.08466 (베이스라인 0.04187 대비 약 2배)
- 멀티모달 추천 논문 FREEDOM(ACM MM 2023)의 핵심 구조를 대회 데이터에 맞게 경량 구현해 랭커 feature로 적용
- 대회 규칙에 따라 코드는 마감(2026.12.04) 이후 공개 예정

---

### Skills

Python · PyTorch · ROS 2 · Webots · XGBoost · CatBoost · Git
