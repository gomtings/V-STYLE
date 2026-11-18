# 제3자 라이선스 고지

V-STYLE은 아래 오픈소스, AI 모델, 데이터를 사용합니다. 각 라이선스의 전문은 제공처의 저장소나 모델 카드에서 확인해 주세요. 앱 안의 **설정 → 앱 정보 → 오픈소스 라이선스**에서도 볼 수 있습니다.

> 이 테스트 배포는 **비상업·연구 목적**입니다. 일부 구성요소(MobileCLIP 모델, Open-Meteo 무료 이용)는 비상업 용도만 허용합니다. 상업적으로 배포하려면 먼저 해당 구성요소를 교체하거나 사용 허가를 받아야 합니다.

## AI 모델
| 구성요소 | 용도 | 라이선스 |
|---|---|---|
| Gemma 4 (Google) | 코디 설명 | Apache License 2.0 |
| SenseVoice (Alibaba FunAudioLLM) | 음성 인식 | 코드 MIT, 모델은 FunASR Model Open Source License Agreement (출처와 모델 이름 표기 필요) |
| Silero VAD | 음성 구간 감지 | MIT |
| Supertonic-3 (Supertone) | 음성 합성 | 코드 MIT, 모델 가중치 OpenRAIL-M |
| D-FINE | 옷 검출 | Apache License 2.0 |
| MobileCLIP (Apple) | 옷 속성 분석 | 코드 MIT, 모델 가중치 Apple Machine Learning Research Model License (**연구·비상업 용도만**) |
| KcELECTRA (Beomi) | 부적절한 표현 판별 | MIT |
| openWakeWord (David Scripka) | 호출어 감지 | Apache License 2.0 (임베딩 모델은 Google 제공, Apache License 2.0) |

- 음성 인식에는 Alibaba FunAudioLLM의 **SenseVoice** 모델을 사용합니다.
- Apple Machine Learning Research Model is licensed under the Apple Machine Learning Research Model License Agreement.

## 학습 데이터
- 옷 검출 모델(D-FINE)의 학습에 **Open Images Dataset V7**(Google LLC)의 사진과 주석 일부를 사용했습니다. 주석은 CC BY 4.0, 사진은 사진별 CC BY 라이선스입니다. 사진별 저작자, 라이선스, 원본 주소 목록은 [attribution/open-images-dfine-v3.csv](attribution/open-images-dfine-v3.csv)에 있습니다.

## 소프트웨어 구성요소
- Apache License 2.0: AndroidX·Jetpack Compose, Kotlin·KotlinX, CameraX, Room, Google ML Kit, LiteRT·LiteRT-LM, sherpa-onnx
- MIT License: ONNX Runtime

## 날씨 데이터
날씨는 앱이 직접 받지 않고 **우리 서버가 대신 받아 전해 줍니다.** 앱은 서버가 준 출처 문구를 날씨 카드에 표시합니다.

- **기상청** 동네예보(기상청 API허브): 이용 조건은 기상청 API허브의 이용약관을 따르며, 출처는 "기상청"입니다.
- **Open-Meteo.com**: Weather data by [Open-Meteo.com](https://open-meteo.com), CC BY 4.0. 무료 이용은 비상업 목적에 한합니다.
