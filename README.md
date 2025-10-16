# 🩺 심장병 예측 데이터 분석 프로젝트

UCI Machine Learning Repository의 심장병 데이터를 활용하여 데이터 분석 및 머신러닝 모델링을 실습하는 프로젝트입니다.

## 📂 데이터셋

  - 본 프로젝트는 `heart_disease.csv` 파일을 사용합니다.
  - 데이터 출처: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/dataset/45/heart+disease)

## 📊 속성 정보 (Attribute Information)

총 14개의 속성으로 구성되어 있으며, 각 속성의 의미는 다음과 같습니다.

| 속성명 (영문) | 속성명 (한글) | 설명 |
| :--- | :--- | :--- |
| `age` | **나이** | 환자의 나이 |
| `sex` | **성별** | 1: 남성, 0: 여성 |
| `cp` | **흉통\_유형** | 1: 전형적 협심증, 2: 비정형 협심증, 3: 협심증 외 통증, 4: 무증상 |
| `trestbps` | **안정\_혈압** | 안정 상태에서의 혈압 (mmHg) |
| `chol` | **콜레스테롤** | 혈청 콜레스테롤 수치 (mg/dl) |
| `fbs` | **공복\_혈당** | 공복 혈당 \> 120 mg/dl (1: True, 0: False) |
| `restecg` | **심전도\_결과** | 안정 시 심전도 결과 (0: 정상, 1: ST-T파 이상, 2: 좌심실 비대) |
| `thalach` | **최대\_심박수** | 운동 시 도달한 최대 심박수 |
| `exang` | **운동\_유발\_협심증** | 운동으로 인한 협심증 유발 여부 (1: Yes, 0: No) |
| `oldpeak` | **ST\_분절\_하강** | 운동 대비 안정 시 ST 분절 하강 수치 |
| `slope` | **ST\_분절\_기울기** | 운동 시 ST 분절의 기울기 (1: 상승, 2: 평탄, 3: 하강) |
| `ca` | **주요\_혈관\_수** | 형광 투시법으로 확인된 주요 혈관의 개수 (0-3) |
| `thal` | **탈라세미아** | 3: 정상, 6: 고정 결함, 7: 가역 결함 |
| `num` | **심장병\_진단** | 심장병 진단 결과 (0: 없음, 1-4: 있음) |

## 🚀 구글 코랩(Google Colab)에서 실행하기

구글 코랩 환경에서 아래 코드를 순서대로 실행하여 데이터를 불러올 수 있습니다.

### 1\. GitHub 저장소 복제

먼저, `!git clone` 명령어를 사용하여 이 저장소의 파일들을 코랩 환경으로 가져옵니다.

```python
!git clone https://github.com/thiskorea81/heart_disease.git
```

### 2\. Pandas로 데이터 불러오기

저장소 복제가 완료되면, `pandas` 라이브러리를 사용하여 `heart_disease.csv` 파일을 DataFrame으로 불러옵니다.

```python
import pandas as pd

# 파일 경로를 지정합니다.
file_path = '/content/heart_disease/heart_disease.csv'

# CSV 파일을 DataFrame으로 읽어옵니다.
df = pd.read_csv(file_path)

# 데이터의 첫 5행을 출력하여 잘 불러왔는지 확인합니다.
print(df.head())
```
