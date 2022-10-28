# Bento

お弁当の売り上げの予測をする分析コンペティション

# Variables
### Dependent variable
y：お弁当の販売数
### Independent Variables
kcal：カロリー

name：名前から推定された主な調理法

weather；天気

event：イベント

payday：社員の給料日

remarks；お知らせ

week：曜日

soldout：売り切れたかどうか

temperature：気温

precipitation：湿度

# model
lightgbm


# Flow
1. 各変数（remarks, event, payday）についてダミー作成

2. 弁当の名前を調理法ごとに分類

3. 日付データを「日」に直す

4. 天気データを分類

5. Xにテストデータを格納して整理

6. テストデータに同様の加工を施す

7. lightgbmで学習

8. RMSEで評価

# RMSE

rmse_train 12.22849775179996

rmse_test 8.814918277995158
