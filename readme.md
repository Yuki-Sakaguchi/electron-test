# Electronを使ってデスクトップアプリを作ってみる
Atomやvscode、などはElectronで作られている。  
Electronを使ってデスクトップアプリの作り方を学ぶ。

# 参考
[Electronでアプリケーションを作ってみよう](https://qiita.com/Quramy/items/a4be32769366cfe55778)  
[30分で出来る、JavaScript (Electron) でデスクトップアプリを作って配布するまで](https://qiita.com/nyanchu/items/15d514d9b9f87e5c0a29)  
[JavaScript (Electron) を使ってアプリの見栄えを整える](https://qiita.com/nyanchu/items/9a1c910bbca55e9d2f3c)  
[ELECTRONでTODOリストを作ってみた WITH WEB STORAGE](http://daifuku-p.org/w/?p=817)  
[Electronアプリをプロダクトとして「正しく」リリースするために必要な3つのこと](https://nulab-inc.com/ja/blog/typetalk/3-points-for-releasing-production-electron-app/)

# コマンド
実装
```
electron .
```
アプリケーションのアーカイブ化
```
asar pack ./sample ./sample.asar
```
パッケージ化して配布
```
electron-packager ./electron-test testron --platform=darwin,win32 --arch=x64 --electron-version=3.0.10
```

# 所感
* 本当にめちゃくちゃ簡単にアプリができた  
* Firebaseとかと連携すれば面白いものができそう  
* もっと簡単にできるNW.jsというものもあるみたい  
* アプリのアイコンとか作って配布してみるのも良いかも