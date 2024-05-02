티스토리링크 - https://dohun-0714.tistory.com/20


# healthnutrition

수원대학교 국민건강영양데이터 분석 경진대회에 참여해 최우수상을 수상했습니다.
![image](https://github.com/dohun-mat/korea_nutrition_health_data_analysis_contest/assets/81942144/76632c99-bb04-4fc1-9a3b-c2aa7e0923b0)

![KakaoTalk_20230428_160301496](https://user-images.githubusercontent.com/81942144/235079270-f92fb179-2ada-4f0c-af52-3b35f9f3c4fe.jpg)



국가건강영양데이터를 통해 독거노인의 질병예측, 지역별 질병분석을 진행해 지역별로 올바른 질병예측을 할 수 있도록 돕습니다.

현재 187만 독거노인 시대인 우리나라에서 노인돌봄 서비스를 실제로 이용했다는 답변은 8.7%밖에 되지 않았습니다.
노인이 가장 흔히 겪는 문제는 '빈곤'과 '질병'이 대표적입니다. 
독거노인들의 삶을 더 윤택하게 하기 위해 국민건강영양데이터를 활용해 지역별 독거노인의 질병을 파악하고,
지역별로 필요한 독거노인들의 치료를 지원하고자 했습니다.


#분석과정

1. 데이터 시각화
: 독거노인과 비독거노인의 질병, 영양소 비교
2. 상관분석
: 독거노인 데이터의 pearson 상관계수를 사용해 연속형 변수의 상관관계를 측정
3. 클러스터링
: PCA 주성분분석을 통해 지역별 유사 질병수를 가진 개체를 묶어 그룹으로 구성
4. 로지스틱 회귀분석
: 로짓 함를 이용해 목표변수와 설병변수의 관계를 모델링


## 사용 데이터
독거노인 데이터 정의: 가구원수가 한명(cfam==1), 가구주가 본인임(fam_rela==1), 나이(age>=65)
비독거노인 데이터 정의: 가구원수가 한명인 경우 제외, 가구주가 본인이 아닌 사람 중에 나이가 65세 이상인 사람

## 독거노인 지역별 총질병수 평균
![image](https://user-images.githubusercontent.com/103898937/222125833-2863b6bb-92c8-43f8-ad22-1a758fb73580.png)

## 지역별 독거노인 질병 실태 파악
- 비독거노인보다 독거노인이 많은 질병: 고혈압, 당뇨, 고콜레스테롤혈증, 빈혈, 협심증
![독거노인 질병 비율](https://user-images.githubusercontent.com/103898937/222123966-32bad3f5-e2ea-4e15-ac46-97161125487a.jpg)
![독거노인과 비독거노인 질병 비교](https://user-images.githubusercontent.com/103898937/222124022-26c03257-c023-4bd3-b83e-7f7499b176bb.jpg)


## 상관분석

### 정신적 스트레스, 소득분위, 주관적 건강인지, 총질병수 관련 상관분석
![image](https://user-images.githubusercontent.com/103898937/222124350-8f100e37-d0e2-43f7-9397-4292b1324037.png)

### 음주, 흡연 여부와 질병 간의 상관분석
![image](https://user-images.githubusercontent.com/103898937/222124485-39db02f4-7b94-4b6d-b651-c01fd4a651b8.png)


##로지스틱 회귀분석
- 앞으로 환자의 질병 예측을 하고 환자 질병의 위험성에 대해 알아보고자 함.


##클러스터링
![image](https://user-images.githubusercontent.com/103898937/222125621-8416c808-e057-4878-bb79-c5fb1c4b5d1e.png)


#독거노인 질병예방 위한 해결 방안
- 지역의 적극적인 모니터링을 지원할 수 있는 시스템 만들기

1. 지역별 질병 체크
- 전국/해당 지역 질병 평균 비교, 타지역간의 비교, 해당 지역의 원하는 두년도 비교
![image](https://user-images.githubusercontent.com/103898937/222125068-c846e86c-5f8f-42a4-ae33-30741f72dc05.png)

2. 지역별 영양소 체크
- 전국/ 해당 지역 영양소 평균 비교, 타지역간의 비교, 원하는 년도간의 비교
![image](https://user-images.githubusercontent.com/103898937/222125237-607cea26-9670-4a23-926f-614ce5992bc0.png)

3. 알림 기능
- 해당 지역의 위험 질병 순위 알림 기능
![image](https://user-images.githubusercontent.com/103898937/222125390-d9f7d6c7-a91b-4ad3-b48e-722d193f525f.png)


#참가 후기
이번 경진대회를 통해 독거노인들의 질병 실태 파악과 예방에 도움



