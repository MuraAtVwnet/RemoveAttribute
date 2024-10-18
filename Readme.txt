■ これは何?
クリップボードに格納されている文字列の属性を削除して、ブレーンテキストにします

■ 実行方法
クリップボードに文字列を読み込んだら、以下コマンドを PowerShell プロンプトで実行すると、クリップボードにセットされている文字列の属性を削除します

RemoveAttribute

(removea[TAB] でコマンド補完されます)

■ 動作確認環境

Windows PowerShell 5.1
PowerShell 7.4.5 (Windows)
たぶん Mac Linux でも動くはず

Windows Powershell の場合、スクリプトの実行許可が必要なので、以下コマンドで許可状態を確認して下さい

Get-ExecutionPolicy

結果が、「RemoteSigned」になっていないかったら、以下コマンドを入力(1回のみ)

Set-ExecutionPolicy RemoteSigned -Scope CurrentUser -Force



■ オプション

RemoveAttribute の後に、ハイフンを入力して TAB を叩くと、オプションが補完されるのて、必要オプションを選択してください

RemoveAttribute -[TAB]


-VertionCheck

最新版のスクリプトがあるか確認します
最新版があれば、自動ダウンロード & 更新します


■ GitHub

https://github.com/MuraAtVwnet/RemoveAttribute
git@github.com:MuraAtVwnet/RemoveAttribute.git


■ Web Page


■ スクリプトインストール方法

# 以下を PowerShell プロンプトにコピペ

$ModuleName = "RemoveAttribute"
$GitHubName = "MuraAtVwnet"
Invoke-WebRequest -Uri https://raw.githubusercontent.com/$GitHubName/$ModuleName/master/OnlineInstall.ps1 -OutFile ~/OnlineInstall.ps1
& ~/OnlineInstall.ps1

