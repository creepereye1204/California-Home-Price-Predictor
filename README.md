데이터확인

![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.001.jpeg)

![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.002.jpeg)

1\.이상치제거

![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.003.jpeg)

집주인의중앙값, 집값의중앙값이 제한값에몰림![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.004.jpeg)![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.005.png)

해당구간제거

![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.006.jpeg) ![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.007.jpeg)

2\.카테고리피처변환

- 카테고리값끼리서로유사도가없음 ![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.008.jpeg)
- 카테고리타입인 ocean\_proximity를 원-핫인코더(One-hot encoder)로변환 

3\.데이터정규화

- 각특징별단위가다르고불규칙한부분(특이치)가 많으므로특이치에비교적약한 MinMaxScaler대신 StandardScaler 사용

![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.009.jpeg)

4\.결측치확인![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.010.jpeg)

결측치처리

- 결측치(Missing\_Value)를지우기에는 ![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.011.jpeg)데이터가많고직접다른값을넣기에는 데이터간의패턴이불규칙함 

  (이전값, 이후값넣기는의미가없다고판단또한그래프를보면 알수있듯 0을넣기에는해당값을가지는데이터가적음으로배 제) 

- 그러나표준편차가비교적적고 이상치의영향을적게받을수있는 중앙값이적절하다고판단. 

결과

![](Aspose.Words.1bdeaced-db5b-4876-bf3e-3602e4507997.012.png)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 004](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/0746c6dc-e8b7-4bc6-b848-ed2fd8a3e22c)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 003](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/3277ac0e-e16c-4920-85cd-127b951f5057)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 002](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/03e973cd-0978-4693-b5ba-0d87914ea736)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 001](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/498f4985-cc49-4da7-897f-12dc2ab239ae)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 012](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/706dd7d2-0065-4a15-965d-6b2ed4a2e512)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 011](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/ca6d58bb-33d9-4d6b-a79b-262710bd74f2)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 010](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/0e29e739-040b-4e26-9c19-5de931475745)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 009](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/780fefce-7eee-4870-893b-d610bf465355)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 008](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/a5dd0d19-45cc-495a-9e8f-a667dbed5368)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 007](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/523b0233-f1ed-42d2-8284-ef584be2e74d)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 006](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/84eb3b00-dfa0-4cfb-9410-ae0297647bf6)
![Aspose Words 1bdeaced-db5b-4876-bf3e-3602e4507997 005](https://github.com/creepereye1204/California-Home-Price-Predictor/assets/112455232/fb674594-3ece-40eb-8c7e-ffbd4f6db38c)
