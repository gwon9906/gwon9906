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

- 동의대학교 컴퓨터공학과 학사 졸업  
- 전력·연산·노이즈 등 **물리적 제약 환경에서 AI 성능을 최적화하는 문제**에 집중  
- 실험 기반 개선과 **정량 지표(PDR, MAPE, MSE 등)**를 통한 성과 검증을 강점으로 함  

---

## 🔧 핵심 역량

- **프로그래밍:** Python, C/C++  
- **AI/ML:** PyTorch, TensorFlow 기반 실험 및 모델 구현  
- **시스템 최적화:** 데이터 압축, 경량화, 성능-효율 트레이드오프 분석  
- **신호/시계열 처리:** STFT 기반 스펙트로그램, 시계열 예측 및 이상 처리  
- **협업:** Git/GitHub 기반 프로젝트 관리  

---

## 🚀 주요 프로젝트

### 1) 저전력 IoT 환경을 위한 초경량 데이터 압축 및 복원 (BAM 기반)

- **성과:**  
  - 전송 데이터 **32B → 20B (37.5% 감소)**  
  - **PDR 절대 기준 +14p.p. 향상**  
  - GPS 복원 MSE **0.0036** 달성  

- **역할:** 팀장, 알고리즘 설계부터 시스템 통합 및 실험 검증까지 전체 파이프라인 담당  

- **의의:**  
  재전송 증가 대신 **데이터 자체를 줄이고 복원 성능을 최적화**하여  
  저전력 LPWAN 환경에서 통신 효율과 신뢰성을 동시에 개선  

- Repo: https://github.com/gwon9906/Lightweight-MF-BAM  

---

### 2) 산업 밸브 유량 예측 (Encoder-LSTM)

- **성과:**  
  - MAPE **1.13 → 0.188 (약 83% 개선)**  

- **주요 접근:**  
  - 밸브 개폐 시점 기준 시계열 재구성  
  - Huber Loss 적용으로 이상치에 강건한 학습  
  - 단순화된 정규화로 안정적 수렴 유도  

*(협업 프로젝트로 저장소 비공개)*

---

### 3) 초저 SNR 환경 LoRa 패킷 복원 (진행 중)

- **목표:** 0 ~ -30 dB SNR 환경에서도 CRC 통과 가능한 패킷 복원  
- **현재 연구:**  
  - STFT 기반 복소 스펙트로그램 인코딩  
  - 다층 BAM 구조를 활용한 엣지-클라우드 압축 복원 파이프라인  

---

## 📚 연구 및 활동

- AI/ML 연구실 학부 연구생 (2024.06 ~ 현재)  
  - 저신호 환경 무선 신호 복원  
  - 산업 센서 시계열 예측 및 최적화 알고리즘 연구  

---

## 📫 연락처

- Email: gwon99065@naver.com  
- GitHub: https://github.com/gwon9906  
- Portfolio: https://gwon9906.github.io  
- Blog: https://latetime.tistory.com  
