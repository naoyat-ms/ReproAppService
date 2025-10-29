
##フォルダ構成
MyWebApp/
│
├── Program.cs
└── MyWebApp.csproj


###※補足
• <Project Sdk="Microsoft.NET.Sdk.Web"> は Web アプリケーション向けで、HTTP サーバやミドルウェアなどの機能が有効になります。
• <Project Sdk="Microsoft.NET.Sdk"> はコンソールアプリ向けで、Web 関連の機能は含まれません。


##ローカル動作確認
プロジェクトファイル (.csproj) が存在するディレクトリでビルド、実行
dotnet build
dotnet run

##App Service 上で動作確認
dotnet publish -c Release -o ./publish

App Service Windows, dotnet 8.0 作成。
publish 配下を zip して C:\home\site\wwwroot>  へデプロイ。

