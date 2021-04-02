# feature engineering
## log 변환
* 왜곡된 분포도를 가진 dataset을 정규분포에 가깝게 만들어줌
 * ex) 신용카드 거래 중 정상이 30만건, 사기가 500건
* np.log1p(`series`) 으로 로그변환, np.expm1(`value`) 으로 원본값 찾기

## IQR 
* 사분위를 이용하여 이상치 제거

## 언더샘플링 & 오버샘플링
> 언더샘플링
> * 많은 target값을 가지고있는 데이터를 적은 target값 데이터 양 정도로 감소 샘플링

> 오버샘플링
> * 적은 target값을 가지고있는 데이터를 많은 target값 데이터 양 정도로 뻥튀기 샘플링

>> SMOTE 방식
>> * K 최근접 이웃 방식으로 적은 target 값 사이사이에 임의로 데이터를 증식시켜서 오버샘플링 하는 방식

## standardscaler
* 평균이 0 인 정규분포 형태로 만들어줌


