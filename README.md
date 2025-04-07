# Project6
### 미국 남동부 지역에서의 사회적 취약성 및 자연재해 시공간 분석 연구


## Table of Contents
- [프로젝트 Description](#프로젝트_Description)
- [프로젝트 정보](#프로젝트_정보)
- [프로젝트 결과](#프로젝트_결과)
  

## 프로젝트 Description
- 미 남동부의 자연재해에 대해 시계열에 따른 변화를 포괄하는 공간 분포 확인
- 자연재해 핫·콜드스팟과 사회적 취약지수·주택 가격 간 관계 규명
- 사회적 취약성을 고려한 자연재해 위기 지역 추출 및 우선 지원 제안


## 프로젝트 정보
1) **프로젝트 사용 환경**
   - 사용 환경: Arcgis Pro, QGIS, R, Python (VS code)

2) **프로젝트 구성 절차**
   - **발생형 핫스팟 분석 : 자연재해의 시공간패턴 확인**
     
     * 자료 수집 (미 남동부 자연재해 데이터 - 산불, 허리케인 / county 경계 / 사회적 취약 지수)
     * Arcgis Pro 툴 사용 (Create Space Time Cube by Aggregating Points -> Emerging Hot Spot Analysis)
     * 최근 30년간 자연재해가 증가한 핫스팟 Grid 결과 추출 및 해석
   - **분산분석 : 자연재해와 사회적 취약성 관계규명**
     * 사용 핫스팟 결과 수집 (조지아주, 플로리다주 화재 핫스팟 Grid), 수치 자료 수집
     * Arcgis Pro 툴 사용 (Spatial Join & Create CSV)
     * R, Python 사용을 통한 ANOVA 분산 분석
     * 결과물 해석 및 취약지 추출


## 프로젝트 결과
- 핫스팟 County 중 기대 결과를 증명하는 SVI 변수가 많을 수록, 세부 SVI 변수에 따라 누락되는 취약계층 적음
  
  * 빈곤율, 노인비율, 소수자 비율(인종)이 기대 결과를 증명하는 A 지역, 노인비율만이 기대결과를 증명하는 B지역 중 A지역이 다양한 취약계층을 더 잘 포착된 것으로 판단 가능
- 핫스팟 County 중 기대결과에 충족하는 SVI 변수의 총합이 최대인 곳을 우선 지원 취약지로 선정
  * 조지아 주 : Greene, Putnam, Warren County / 플로리다 주 : Calhoun, Hamilton County

