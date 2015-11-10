# プロキシを設定しよう
プロキシ内でATOMを使用する場合は、必ず[apm](https://github.com/atom/apm)にプロキシ設定を行いましょう。プラグインをインストールできないATOMにあまり魅力はありません。以下のコマンドを実行してください。

**https-proxyの設定**
```
apm config set https-proxy http://username:password@proxy.example.com:8080
```

プロキシ設定が終わったら、上手く設定できているか確認しましょう。以下のコマンドを実行しましょう。
```
apm config list
```

以下のような設定情報が表示されると思います。
```
; cli configs
globalconfig = "/Users/admin/.atom/.apm/.apmrc"
user-agent = "npm/2.13.3 node/v0.10.40 darwin x64"
userconfig = "/Users/admin/.atom/.apmrc"

; userconfig /Users/admin/.atom/.apmrc
https-proxy = "http://username:password@proxy.example.com:8080"

; globalconfig /Users/admin/.atom/.apm/.apmrc
cache = "/Users/admin/.atom/.apm"

; node bin location = /opt/homebrew-cask/Caskroom/atom/1.1.0/Atom.app/Contents/Resources/app/apm/bin/node
; cwd = /Users/admin/Documents/github/masaki-kusuhata/study
; HOME = /Users/admin/.atom/.node-gyp
; 'npm config ls -l' to show all defaults.
```

設定した情報が表示されていれば、プロキシ設定は完了です。
