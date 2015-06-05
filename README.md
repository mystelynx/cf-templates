# cf-templates

CloudFormationのサンプルテンプレートをTypesafeConfigに置き換えてみる

```
pip install pyhocon
pyhocon -i template.conf -o cf.json -f json -o template.json
```

TODO:
include対象のファイルがないときにエラーにしたい。。。
