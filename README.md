# UE4_SRanipal\\
\\
Unreal Engine4へのSRanipal（HTC VIVE Pro eye用Plugin）の導入が非常に面倒くさかったので色々メモしておく。\\
\\
まずバージョンについて確認しておくと、コンパイルエラー無く動作したのは\\
UE4-> 4.22.3, 4.23.1\\
SRanipal SDK -> 1.1.0.1\\
Visual Studio 2017 Community　->15．9.22\\
またVisual Studio　Installer -> 変更 -> 個別のコンポーネントから.NET Framewark 4.7.1 SDKを選択\\
Visual Studio　Installer -> 変更　-> ワークロード　C++によるゲーム開発を選択\\
\\
手順1\\
C++でプロジェクトを作成。\\
※このときファイルがOneDrive内だとエラーが発生するので注意\\
手順2\\
一度プロジェクトを閉じ.uprojectと同じ場所にPluguinsフォルダを作成し、その中にSRanipalファイルを配置。\\
手順3\\
test23.uprojectを右クリックしGenerate Visual　Studio project fileを選択\\
手順4\\
.SlnファイルをVSで起動し(プロジェクト名).Build.csを開きPublicDependencyModuleNamesに追加したPulginの名前を追加する。\\
手順5\\
プロジェクトを起動しプラグインが導入されていることを確認する。\\
手順6\\
コンテンツブラウザの表示オプションからプラグインコンテンツの表示をチェック\\
