**SKT FLY AI Challenger 5기**

# 바른말싸미 👋⌨️
사이버상 초등생의 언어 폭력 방지를 위한 AI 기반 키패드 서비스 입니다.

## 2. 프로젝트 개요
### 2-1. 제안 배경
- 2023년 하반기에 교육부가 진행한 학교폭력 실태조사에서 사이버 폭력 중 언어폭력이 37.1%로 1위를 차지하고, 초중고 학생들 중 초등학생 피해응답률이 최대 9배 높음 
- 언어습관이 형성되는 시기인 초등학생들 중심으로 사이버 폭력 해결이 필수적
- 초 3생이 교감 선생님 뺨을 때린 사건.
- 초등 6학년 남학생, 교실서 담임 폭행 "학생들 앞에서 수십대 맞아..".

앞선 이슈들은 신체적 폭력 뿐 아니라, 폭력적인 언어 사용과 함께 됩니다.
부모님 입장에서는 가정 밖의 자녀 행동을 알 수 없으니, "우리아이가 그럴 줄 몰랐어요"라는 말이 나올 수 밖에 없을 것 같습니다.

### 2-2. 목표
- 보호자 : 자녀의 언어 사용 습관을 점검 및 교육 환경 제공 (사생활 침해 x)

## 3. 기능
![image](https://github.com/user-attachments/assets/a24cb517-f2c1-4cac-aadc-5a1d5115e36d)

## 4. 시스템 아키텍쳐
![22](https://github.com/user-attachments/assets/655f243a-7d4b-46d1-8ea5-f331839a4dcc)


[Keypad]
![최종발표자료](https://github.com/user-attachments/assets/1bdd4e5c-905b-43ce-9bc9-31404616bc25)

[App Report]
![0901150543612106](https://github.com/user-attachments/assets/db6b7695-7db3-4ac7-b8f3-8837ef5292d4)

### 4-1. 구현 툴

| Category  | Technologies                                        |
|-----------|-----------------------------------------------------|
| AI model  | BERT, ELECTRA, RAG, GPT-4o, Prompt Engineering                             |
| Keypad    | Android native (kotlin)                                      |
| Frontend  | Flutter, Figma                                      |
| Backend   | Azure, docker, FastAPI, MySQL                               |
| CI/CD     | GitHub Actions                                      |



## 5. AI 기술
### 5-1. 데이터 전처리 : 감정 태깅
- 텍스트 윤리검증 데이터 약 36만 개 사용
- [KcELECTRA](https://github.com/Beomi/KcELECTRA) 를 사용하여 8가지 윤리 및 44가지 감정 라벨링

### 5-2. 감정과 윤리 분류를 한번에 하는 멀티태스킹이 가능한 BERT
- [KoSimCSE-BERT-multitask](https://huggingface.co/BM-K/KoSimCSE-bert-multitask) 활용

### 5-3. 프롬프트
- gpt-4o 모델을 활용
- 레포트를 위한 3개의 프롬프트 템플릿 제작
  - 사용자 : 언어습관 레포트
  - 보호자 : 사용자의 언어습관 레포트, 사이버 폭력 위험 레포트
  - point :
    - 객관성 확보 : 실제 발화에서 비속어 횟수 통계, 발화 내역을 통해 언어, 비속어 사용 습관에 대한 정보를 제공. [내역 문서화 (.txt)]
    - 참고자료 : kakaotalk, 푸른코끼리

## 6. 시연 영상

https://github.com/user-attachments/assets/ac08bcb5-da2e-4b94-a4f2-b56f4fc4a724



  
## 7. 팀원 소개

| 이름   | 역할                                       | 
| ------ | ------------------------------------------ | 
| [김현동](https://github.com/miffDONG) 🤨 |PM, AI    |
| [김호준](https://github.com/Hxjxxn95) 😊 | AI, 키패드 | 
| [배성욱](https://github.com/uksungbae) 😁 | 백엔드, 프론트엔드                     | 
| [손서희](https://github.com/sh1257) 😘 | 프론트엔드, 디자인               |
| [옥지원](https://github.com/JiWonOck) 😯 | 발표, 데이터             | 


## 8. Link
To be updated


## 9. Award

6회 K디지털 트레이닝 해커톤 자유과제부문 - 장관상(최우수상🥇)
