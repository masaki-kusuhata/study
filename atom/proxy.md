# プロキシを設定しよう
プロキシ内でATOMを使用する場合は、必ずapmにプロキシ設定を行いましょう。プラグインをインストールできないATOMにあまり魅力はありません。以下のコマンドを実行してください。

**http-proxyの設定**
```
apm config set http-proxy http://username:password@proxy.example.com:8080
```

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
~~~~~~~~~~
; userconfig /Users/riaux06/.atom/.apmrc
http-proxy = "http://username:password@proxy.example.com:8080"
https-proxy = "http://username:password@proxy.example.com:8080"
~~~~~~~~~~~
```

設定した情報が表示されていれば、プロキシ設定は完了です。
