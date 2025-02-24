# 概要
- Raspberry Pi を使ったロジックアナライザー(試作)

# 機能
- Raspberry Piを使って、サンプリングを実施。
- Windows上で、サンプリングデータを表示。

# 動作環境
- Windows
- Raspberry Pi

# セットアップ
## Windows
- インストーラ LogicAnalyzerSetup.exe を Windows 上の任意のフォルダにダウンロードし、管理者として実行します。  
- LogicAnalyzer がインストールされます。
## Raspberry Pi
- la_samp を Linux 上の任意のディレクトリにダウンロードします。

# 動作手順
- Windows 上で、スタートアップメニューから、LogicAnalyzer を実行します。
- LogicAnalyzer のメニュー Sampling > Init を実行します。la_samp からの接続待ち状態になります。
- Linux 上で la_samp を実行します。サンプリングを開始し、サンプリングデータを LogicAnalyzer に送信します。
  ```
  $ sudo la_sampl "WindowsのIPアドレス" "ポート番号"
  ```
- LogicAnalyzer でサンプリングデータを拡大・縮小表示したり、複数の信号をまとめて表示したりして、波形を観測します。

# 免責事項
- 個人の趣味で作った試作です。テストしていません。
- 万一問題が起きても一切の責任を負いません。自己責任でご使用ください。
