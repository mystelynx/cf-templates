# cf-templates

CloudFormationのサンプルテンプレートをTypesafeConfigに置き換えてみる

```
pip install pyhocon
pyhocon -i template.conf -o cf.json -f json -o template.json
```

### 今分かってる制約
- 正規表現などで`\\`を入れたいときは`\\\\`としておく
- 配列内の`""`は消去されてしまう？ので`${?empty}""`とかいておく（empty=存在しないキー名ならなんでも）

TODO:
include対象のファイルがないときにエラーにしたい。。。
