<h1 align="center">이해권 (Haegwon Lee)</h1>
<p align="center">
  AI/ML 엔지니어 · 하드웨어 제약 환경 최적화(On-device AI)<br/>
  <a href="mailto:gwon99065@naver.com">gwon99065@naver.com</a> ·
  <a href="https://github.com/gwon9906">GitHub</a> ·
  <a href="https://gwon9906.github.io">Portfolio</a> ·
  <a href="https://latetime.tistory.com">Blog</a>
</p>

---

## 👋 소개
- 동의대학교 컴퓨터공학과 학사 졸업 (2026.02)
- 전력·연산·노이즈 등 **물리적 제약 환경에서 AI 성능을 최적화하는 문제**에 집중
- 결과를 그대로 믿지 않고, **왜 그런 결과가 나왔는지 설명될 때까지 검증**하는 방식으로 일함
- 실험 기반 개선과 **정량 지표(MSE, MAPE 등) 및 실환경 측정**을 통한 검증을 강점으로 함

---

## 🔧 핵심 역량
- **프로그래밍:** Python, C/C++
- **AI/ML:** PyTorch, TensorFlow 기반 실험 및 모델 구현
- **시스템 최적화:** 데이터 압축, 경량화, 성능-효율 트레이드오프 분석
- **신호/시계열 처리:** STFT 기반 스펙트로그램, 시계열 예측 및 이상 처리
- **온디바이스:** Raspberry Pi 등 하드웨어 제약 환경 실행·검증
- **협업:** Git/GitHub 기반 프로젝트 관리

---

## 🚀 주요 프로젝트

### 1) 저전력 IoT 환경을 위한 초경량 데이터 압축 및 복원 (BAM 기반)
- **성과:**
  - 전송 페이로드 **32B → 20B (62.5% 감소)**
  - 복원 MSE **0.0036** 달성
  - payload 감소가 전송 성공률(PDR)을 높인다는 가설을 **실환경에서 한 달간 필드 측정으로 검증**(개선 경향 확인) — 측정값이 기대보다 낮은 원인이 **송신 준비 시간 병목**임을 사후 분석으로 규명
- **역할:** 팀원 — BAM 압축 모델 설계·구현 및 현장 필드 테스트 담당
- **의의:**
  재전송을 늘리는 대신 **데이터 자체를 줄이고 복원 성능을 최적화**하여
  저전력 LPWAN 환경에서 통신 효율과 신뢰성을 함께 개선
- Repo: https://github.com/gwon9906/Lightweight-MF-BAM

---

### 2) 산업 밸브 유량 예측 (Encoder-LSTM)
- **성과:**
  - 유량 예측 **MAPE 0.188** 달성
- **주요 접근:**
  - 밸브 개폐 시점 기준 시계열 재구성
  - Huber Loss 적용으로 이상치에 강건한 학습
  - 단순화된 정규화로 안정적 수렴 유도
- *(협업 프로젝트로 저장소 비공개)*

---

### 3) 초저 SNR 환경 LoRa 신호 복원 연구 (Complex-valued BAM)
- **문제:** 초저 SNR 환경에서 LoRa 심볼 복조가 무너지는 문제.
  선행 코드의 de-chirp 구현 오류(오버샘플링 FFT의 OSF-fold 합산 누락)를 발견·수정한 것이 출발점
- **접근:** 복소 IQ 신호를 다루는 complex-valued BAM 설계 (IEEE 논문의 Lagrange 안정성 조건에 맞춰 split-tanh·복소 가중치 구조), Noise2Noise·스킵 커넥션 등 구조를 바꿔가며 실험
- **결과:** 일부 구간(-25~-30dB)에서 baseline 대비 개선을 확인했으나 절대 정확도는 실용 수준에 미달.
  구조 변경만으로 해결되지 않는 한계로 판단해, **SOM으로 데이터 분포를 분석**한 결과 원본 IQ에서 심볼 간 거리 구분이 어렵다는 근본 원인을 규명하고 마무리
  (대조군 MNIST는 뚜렷하게 군집화된 반면 LoRa 심볼은 그렇지 않음)
- Repo: https://github.com/gwon9906/LoRa-bam-reconstruction

---

## 📚 연구 및 활동
- **Wireless AIoT System Lab** 학부 연구생, 동의대학교 (2024.07 ~ 2026.02)
  - 저신호(초저 SNR) 무선 신호 복원 연구
  - 엣지·무선 환경 센서 데이터 압축·전송
  - 산업 센서 시계열 예측 및 최적화

---

## 🎯 현재 학습 중
- **모델 양자화:** PTQ / QAT, 대칭·비대칭, per-channel / per-tensor, calibration,
  ultra-low-bit(ternary·1.58bit) — 압축 프로젝트의 다음 단계로 학습 중

---

## 📫 연락처
- Email: gwon99065@naver.com
- GitHub: https://github.com/gwon9906
- Portfolio: https://gwon9906.github.io
- Blog: https://latetime.tistory.com
