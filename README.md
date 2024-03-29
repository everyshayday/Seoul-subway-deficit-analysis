# [멋쟁이사자처럼] AI SCHOOL MID PROJECT 1
![image](https://github.com/everyshayday/AS8/assets/124337992/c01c475a-cb43-48e7-9f6e-962f256c54fa)
(이미지 출처: https://www.etoday.co.kr/news/view/2223025)

## 1. 프로젝트 개요
1-1. **주제**: 지하철 운영 적자의 원인이 고령층 무임승차 때문일까?

1-2. **주제 선정의 배경**: 23년 2월 현재, 대중교통 요금 인상이 화두로 떠오르고 있다. 실제 서울 지하철 요금은 수송원가가 기본운임보다 높은 구조이며 최근 5년간 평균 약 9,200억 원 수준의 적자가 발생했다. 서울시는 지하철 적자 주요인으로 노인 무임승차를 꼽으며 노인 연령 상향까지 논하고 있는 상황이다. 우리는 정말 지하철 적자 요인이 노인의 무임승차와 관련 있는지 확인해보고자 한다.

1-3. **본 프로젝트의 활용 방안 제시**
- 서울교통공사 : 적자 요인 분석에 활용 가능, 노인 무임승차 나이 상향 시 영향 확인 가능
- 지자체 : 대중교통 요금 인상에 대한 정책 결정의 근거로 참고 가능

## 2. 프로젝트 팀 구성 및 역할
| 이름 | 역할 | 담당 분석 파트 |
| --- | --- | --- |
| 강다솔 | 주제설정, 데이터 수집, EDA, 시각화, 결과도출, 발표자료 정리 | 2020년 고령층 무임 수송에 따른 손실액 감소원인 분석  |
| 김민기 | 주제설정, 데이터 수집, EDA, 시각화, 결과도출, 발표자료 정리, 코드 취합  | 지하철 적자와 고령 인구간의 상관관계 분석 |
| 김조은 | 주제설정, 데이터 수집, EDA, 시각화, 결과도출, 발표자료 정리 | 향후 5년간 노인 연령 상향과 기본료 인상의 변화차이율 분석 |
| 배상빈 | 주제설정, 데이터 수집, EDA, 시각화, 결과도출, 발표자료 정리 | 노임 무임승차제도 폐지의 사회적 편익 분석 |
| 임승민 | 주제설정, 데이터 수집, EDA, 시각화, 결과도출, 발표자료 정리, 발표자 | 서울교통공사 재무제표 분석 |
| 조세연(팀장) | 주제설정, 데이터 수집, EDA, 시각화, 결과도출, 회의 진행 및 일정관리, 발표자료 정리, ppt 제작  | 노인 연령 상향 시 발생하는 수익 계산 및 운임손실 차이 비교 |

## 3. 프로젝트 수행 절차 및 방법
3-1. **데이터 수집**
1. 분석 주제 및 가설 설정에 필요한 데이터 구상
2. KOSIS, 서울교통공사 웹페이지, 관련 논문 등 데이터를 구할 수 있는 방식 서칭
3. KOSIS의 행렬 전환 기능 등을 활용해 간단한 전처리 후 csv 파일 형태로 다운

3-2. **전처리 과정** 
1. `.head(),` `.info()`, `shape` 등 코드를 통해 전체적인 데이터프레임 구성과 데이터 타입 확인
2. 불필요한 컬럼 제거, 복잡한 컬럼명을 단순하게 변경
3. melt를 활용해 tidy data 만들기
4. 그 외 개인별 전처리 과정의 차이가 있음

3-3. **사용 데이터 출처**
- 국가통계포털(KOSIS) 데이터, 서울교통공사 데이터

## 4. 결과물
![image](https://github.com/everyshayday/AS8/assets/124337992/ecf1f6e0-609f-4da2-97a8-ba436331ed3b)
(pdf 파일 참고)

4-1. **결론 요약**
**1) 노인 무임승차가 지하철 적자의 원인이 될 수 있다.**
- 20년도 노인무임비용이 감소한 것을 근거로 고령층이 지하철 영업 손실에 영향을 끼치지 않았다고 할 수 없다.
- 기본운임인상을 통한 절감량이 현재 더 많지만, 고령화 문제로 인해 연령상향을 통한 절감량이 더 늘어날 수 있다.
- 손익계산서 분석 결과 적자 현황이 매우 심각. 매출원가를 하향 시킬 수 있는 방안이 필요하다.(기본운임인상, 무임연령상향 등)

**2) 노인 무임승차가 지하철 적자의 원인이라고 할 수 없다.**
- 지하철 적자와 고령 인구 증가는 반드시 비례하는 경우만 있는 것은 아니다.
- 노인 연령 상향으로 인해 발생한 수익은 지하철 적자를 유의미하게 메꿀 수 없다.

  => 두 가지 측면을 모두 뒷받침할 수 있는 결과가 고루 나옴

## 5. 프로젝트 회고 및 개선점
**1. 평가단 피드백**
1. 두 가지 측면(무임승차와 기본비용 상향)에서 비교해보고 어떻게 조정해야 사회적으로 이슈가 많고 했을 때 반발을 살 수도 있는지 보여주면서 다양한 솔루션을 제시해준 점도 좋았다.
2. 연령을 상향하면 비용을 절감할 수 있다는 결론이 났는데, 코로나 때 무임승차가 줄어들었다. 그 전후 시기 비교하는 것을 보여준 것도 좋았다.
3. 재무제표 손익계산서 분석까지 해준 것도 좋았다.

**2. 개인 회고**
- **Keep**: 분석 결과를 더욱 효과적으로 잘 전달하는 ppt(시각자료)를 만든 것. (나는 시각화에 강점이 있다는 것을 느꼈다)
- **Problem**: 팀장으로서 개인 작업에만 신경쓸 것이 아니라 팀원들의 작업에 어려움이 없는지도 살펴보고 적절한 도움을 줄 수 있어야 함.
- **Try**: 나는 전체적인 스토리텔링과 기획에 강점이 있지만 디테일한 부분을 놓치는 단점이 있음. 깊이있는 분석을 할 때 한단계 더 생각하는 습관을 가질 것.

