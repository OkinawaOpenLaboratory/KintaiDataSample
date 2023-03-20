# 勤怠データを使用したレポート作成・共有

このドキュメントでは、勤怠データを使用し Power BI で勤怠レポートの作成、Teams で勤怠レポートの共有を行う。

## 事前準備

事前に下記の準備をして下さい。

* Power BI Pro以上のライセンスを保持した Microsoft アカウント
* [Power BI Desktop のインストール](https://learn.microsoft.com/ja-jp/power-bi/fundamentals/desktop-get-the-desktop)
* [Teams](https://www.microsoft.com/ja-jp/microsoft-teams/log-in)
* [kintai.xlsx](https://github.com/OkinawaOpenLaboratory/KintaiDataSample/raw/main/kintai.xlsx)
* [kintaiReport.pbix](https://github.com/OkinawaOpenLaboratory/KintaiDataSample/raw/main/kintai.pbix)

## 設定方法

### 1. Power BI Desktop で勤怠レポート作成

Power BI Desktop で勤怠レポートを作成する。

#### 1.1. Power BI Desktop で kintaiReport.pbix の読み込み

Power BI Desktop を起動し、「ファイル」→「レポートを開く」→「レポートの参照」から、ダウンロードした kintaiReport.pbix を開く。

![image](https://user-images.githubusercontent.com/73327236/225881493-b6662d66-47a7-4996-a0f8-332758c65b12.png)

kintaiReport.pbix の読み込むと勤怠レポートが表示される。

#### 1.2. 勤怠データのデータソース更新

Power BI Desktop で「データの変換」を選択し Power Query Editor を開く。

Power Query Editorで「適用したステップ」→「ソース」を選択し、ダウンロードした kintai.xlsx の格納先にデータソースを更新する。

![image](https://user-images.githubusercontent.com/73327236/225882757-6d1084f7-cc76-466a-b3a3-570fb92bf5e4.png)

kintai.xlsx を読み込み後「閉じて適用」を選択する。

勤怠レポートの作成は以上です。

### 2. Power BI Desktop で作成した勤怠レポートを Power BI Service に発行

Power BI Desktop で作成した勤怠レポートを Power BI Service に発行する。

#### 2.1. Power BI Desktopでサインイン

Power BI Desktop の編集画面で「サインイン」を選択し事前準備で用意したアカウントでサインインを行う。

#### 2.2. 勤怠レポートを Power BI Service に発行

勤怠レポートの画面で「発行」→「ワークスペース」を選択し、Power BI Desktop で作成した勤怠レポートを Power BI Service に発行する。

![image](https://user-images.githubusercontent.com/73327236/225884855-20d27016-f3c7-4664-acb0-9e5773bde688.png)

勤怠レポートを Power BI Service に発行する設定は以上です。

### 3. 勤怠レポートを Teams に共有

Power BI Service に発行された勤怠レポートをTeamsのタブに共有する。

#### 3.1 Teams の起動

事前準備した Microsoft アカウントで Teams を起動する。

#### 3.2 Teams で勤怠レポーを共有する

Teams で勤怠レポートを共有するチャネルでタブの追加を選択し「Power BI」を選択する。

Power BI の設定画面で勤怠レポートを選択し、Teams の画面で勤怠レポートが表示されることを確認する。

![image](https://user-images.githubusercontent.com/73327236/225886206-2193efac-e6ff-49bf-9010-2b6d2e9ea0c0.png)

![image](https://user-images.githubusercontent.com/73327236/225886394-e83867bf-27d5-4c39-9c0b-4bf0ce158c30.png)

Teams で勤怠レポートを共有する設定は以上です。