## Modeling market-neutral strategy between 3 and 5 years of government bond futures.

한국 국채선물 3년과 10년 상품을 손으로 스캘핑 거래 하면서 만든 market neutral strategy 
2가지 를 선형회귀 하여 검증후 트레이딩 하는데 사용한다



Concept 1. 3년물과 10년물 limit orderbook 사이에서 3년물이 먼저 시장가 로 치고 나가면 10년물 또한 
3년물의 방향을 추종하는 경향이 매우 높음 반대의 경우도 마찬가지 

= 호가의 체결 방향을 보면서 market order 로 진입후 1~2tick 의 이익을 얻고 exit 





Concept 2. 3년물과 10년물 사이의 방향이 서로 엇갈릴 경우 가격의 spread 가 일정 부분 이상 벌어지지 않고
장 마감시간에 가까울수록 두 상품간의 가격의 괴리가 점점 줄어듬 

= 같은 시계열 snapshot 에서 linear regression 보다 높은 상품은 sell 낮은 상품은 buy 하여 헤지한뒤
spread 가 줄어들면 이익을 얻고 exit 

<img src="https://user-images.githubusercontent.com/90368209/141477910-2a42d96a-a349-4528-9c21-f68cfbe83f1c.JPG" width="650">





