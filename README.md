# 🖥 AI Team
수행자: 이수연, 오재민, 강수정 
---
## 💡 Introduction
신용카드 사기 탐지 모델

## 🕰️ 수행 기간
2024.04.23~ 2024.05.03 

### **🕹 수행 방법▪도구**
- IDE : Jupyter Notebook, Google Colab
- Tool : Python
- library : pytorch, sklearn, matplotlib, numpy, pandas , imblearn 

# 신용사기 사기 탐지

## 목차
1. [소개 및 문제 정의](#소개-및-문제-정의)
2. [데이터 설명](#데이터-설명)
3. [모델 선택](#모델-선택)
4. [설계](#설계)
5. [모델 개선 시도](#모델-개선-시도)
6. [결론](#결론)

## 소개 및 문제 정의
본 프로젝트는 신용카드 사기 탐지 시스템의 설계를 목표로 합니다. 최근 몇 년간 신용카드 부정 사용 시도가 급증함에 따라, 이에 대한 효과적인 대응이 필요합니다. 본 연구에서는 Fraud Detection System(FDS)를 이용하여 사기 거래를 탐지하고 차단하는 방법을 연구합니다.

![004](https://github.com/LEESUSUSUSU/Credit-card-fraud-detection-model/assets/129818934/41c6659d-aad7-4656-8da2-1604a667e03c)



## 데이터 설명
### 유럽 데이터
- 불균형 데이터: 사기보다 정상 거래가 많음.
<p align="center">
  <img width="243" height="243" alt="불균형 데이터" src="https://github.com/LEESUSUSUSU/Credit-card-fraud-detection-model/assets/129818934/e0d9ba6e-bbd8-4a61-9a05-221fa1627f33">
  <br>불균형 데이터: 사기보다 정상 거래가 많음
</p>
- 상관 관계 행렬을 통해 변수 간의 관계를 분석.
- PCA를 이용한 클러스터링으로 사기 거래와 정상 거래의 분포를 시각화.


### 한국 vs 유럽 데이터
- 한국과 유럽 데이터의 주요 변수 비교.
- 시간과 관련된 데이터 분석.
<table>
  <tr>
    <td align="center">
      <img width="243" height="243" alt="스크린샷 2024-05-02 오후 7 44 44" src="https://github.com/LEESUSUSUSU/Credit-card-fraud-detection-model/assets/129818934/4005792b-4d01-4a99-82ca-0d4a330d0ca4">
      <br>한국
    </td>
    <td align="center">
      <img width="243" height="243" alt="스크린샷 2024-05-02 오후 7 51 46" src="https://github.com/LEESUSUSUSU/Credit-card-fraud-detection-model/assets/129818934/9c02a384-7ca9-4ec2-83d3-91ce2c062ee3">
      <br>유럽
    </td>
  </tr>
</table>

**시간과 연관성이 높은 컬럼**
- 클러스터링을 통해 거래 패턴 분석.


## 모델 선택
- **Logistic Regression**: AUC 0.95
- **CNN**: AUC 0.98
- 두 모델 모두 높은 AUC 점수를 보여 사기 탐지에 유용함.

![모델 선택]

## 설계
- 모델의 성능 평가 결과 비교.
- 정규화를 통해 모델 성능 향상 시도.

![설계]

## 모델 개선 시도
- **SMOTE**: Synthetic Minority Over-sampling Technique을 이용해 불균형 데이터 문제 해결.
- **NearMiss**: 언더 샘플링 기법을 이용해 데이터 균형 맞추기.

![모델 개선 시도]

## 결론
신용카드 사기 탐지 분야에서의 모델 개선 방향과 잠재적 도전 과제를 논의합니다. 향후 연구 방향으로는 데이터의 다양성과 모델의 복잡성을 고려한 추가 연구가 필요합니다.

![결론]
