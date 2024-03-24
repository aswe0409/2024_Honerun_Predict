# 2024_Homerun_Predict

## 개요
한국 프로야구 한화이글스 팬으로 2023시즌 홈런왕인 노시환 선수의 2024 시즌 홈런 개수를 예측 해 보려고 합니다.

## 데이터 명 설명(columns name explanation)
경기 (Games, G): 선수가 참여한 총 경기 수입니다.

타석 (Plate Appearances, PA): 타자가 타격을 시도한 총 횟수로, 볼넷, 삼진, 안타 등 타자가 타석에 서는 모든 상황을 포함합니다.

타수 (At Bats, AB): 타자가 정식으로 타격을 시도하여 결과가 기록된 횟수로, 볼넷, 희생타, 몸에 맞는 볼 등은 제외됩니다.

안타 (Hits, H): 타자가 타격하여 베이스에 안전하게 도달한 횟수입니다.

홈런 (Home Runs, HR): 타자가 타격하여 공이 경기장 바깥으로 나가 한 번에 홈까지 도달하는 안타입니다.

득점 (Runs, R): 타자 또는 주자가 홈 베이스를 밟아 한 점을 올리는 것입니다.

타점 (Runs Batted In, RBI): 타자의 타격으로 주자가 득점을 올린 횟수입니다.

볼넷 (Base on Balls, BB): 타자가 투수로부터 네 번의 '볼'을 받아 1루로 진출하는 것입니다.

삼진 (Strikeouts, SO or K): 타자가 세 번의 '스트라이크'를 받고 아웃되는 것입니다.

도루 (Stolen Bases, SB): 주자가 투수의 공이 투구되는 동안 다음 베이스로 진루하는 것을 성공하는 것입니다.

BABIP (Batting Average on Balls In Play): 타자가 타구를 날렸을 때 안타가 될 확률을 나타내며, 수비수에게 잡히지 않은 타구의 타율입니다.

타율 (Batting Average): 공식 타석에서 안타를 칠 확률로, 안타 수를 타석 수로 나눈 값입니다.

출루율 (On-Base Percentage): 타자가 얼마나 자주 출루하는지 나타내는 비율로, (안타+볼넷+사구)/(타석+볼넷+사구+희생플라이)로 계산합니다.

장타율 (Slugging Percentage): 타자가 타석에서 기록한 총 베이스를 공식 타석 수로 나눈 값입니다.

OPS (On-base Plus Slugging): 출루율과 장타율을 합한 값으로, 타자의 전반적인 공격 기여도를 평가합니다.

wOBA (Weighted On-Base Average): 타자의 출루율을 더 세밀하게 가중치를 두어 계산한 통계로, 다양한 출루 방식을 점수화하여 평균을 낸 것입니다.

WAR (Wins Above Replacement): 대체 선수 대비 해당 선수가 팀에 가져다 준 승리의 가치를 나타냅니다.

단타 (Single): 타자가 타격하여 1루까지만 진루하는 안타입니다.

고4 (Base on Balls, Walk): 투수가 4구의 볼을 던져 타자가 1루로 진루하는 것입니다.

HBP (Hit By Pitch): 투수가 던진 공에 타자가 맞아 1루로 진루하는 것입니다.

희플 (Sacrifice Fly): 타자가 날린 뜬공을 잡아 아웃되지만, 이를 통해 주자가 득점하는 것입니다.

희타 (Sacrifice Hit, Sacrifice Bunt): 희생번트로, 타자가 고의로 아웃되어 주자를 진루시키는 타격입니다.

병살 (Double Play): 수비가 한 번의 플레이로 두 명의 주자를 아웃시키는 것입니다.

도실 (Stolen Base Percentage): 성공적으로 도루를 시도한 비율을 나타냅니다.

볼넷% (Walk Percentage): 타석 대비 볼넷을 얻는 비율입니다.

삼진% (Strikeout Percentage): 타석 대비 삼진을 당하는 비율입니다.

볼/삼 (BB/K): 볼넷 수를 삼진 수로 나눈 비율입니다.

ISO (Isolated Power): 타자의 장타력을 나타내는 지표로, 장타율에서 타율을 뺀 값입니다.

RC (Runs Created): 타자가 만들어낸 득점을 추정하는 통계입니다.

RC/27 (Runs Created per 27 Outs): 27아웃당 만들어낼 것으로 예상되는 득점을 나타냅니다

wRC (Weighted Runs Created): 타자가 만들어낸 득점을 조정하여, 리그 평균과 구장 특성을 반영한 통계입니다.

SPD (Speed Score): 선수의 주루 능력을 종합적으로 나타내는 점수로, 도루 성공률, 1루에서 3루까지 진루 능력 등 여러 요소를 종합한 것입니다.

wSB (Weighted Stolen Bases): 도루가 팀에 가져다 준 기대 득점을 가중치를 적용하여 계산한 값입니다.

wRAA (Weighted Runs Above Average): 리그 평균 선수 대비 해당 타자가 만들어낸 득점의 가치를 나타내는 통계입니다.

# 해당 프로젝트 관련 블로그
아래의 링크를 통해 해당 프로젝트에 대해 자세한 설명을 볼수 있습니다.

You can see more details of this project through the below link 
Thanks


https://velog.io/@aswe0409/series/Data-Analysis-%ED%99%88%EB%9F%B0-%EA%B0%9C%EC%88%98-%EC%98%88%EC%B8%A1
