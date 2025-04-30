# API Experiment Pipeline v1

### 개요
- **목적** : 아이디어를 자동으로 GPT 호출 → 결과·비용·속도를 기록  
- **스택** : Google Colab, OpenAI GPT-4o-mini, Python, pandas  
- **산출물** :  
  - `pipeline_v1.ipynb` : 실행 노트북  
  - `result.csv` : 원본 로그  
  - `result_scored.csv` : 길이 규칙 채점 결과  

### 사용 방법
1. `pipeline_v1.ipynb` 열기 → 자신의 `OPENAI_API_KEY` 입력  
2. `ideas.txt` 에 아이디어 줄마다 추가  
3. **Run all** 실행 → `result*.csv` 자동 갱신

### TODO
- 다중 모델 라우팅(Claude, Gemini)  
- 벡터DB RAG 연결  
- 실패 로그 자동 Slack 알림

## v2: 멀티-모델 라우터
- 파일: `result_multi.csv`
- 모델별 비용 집계 코드 추가
