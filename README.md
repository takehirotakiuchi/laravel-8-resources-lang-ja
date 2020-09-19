# Laravel 8 JetStream 日本語化ファイル

Laravel 8 の日本語メッセージファイル一式です。
ダッシュボートなどで必要な部分を日本語化しています。

具体的には、i18n対応として`{{ __('message') }}`で記載されている箇所に対応しています。

```txt
./resources
└── lang
    ├── ja
    │   ├── auth.php
    │   ├── pagination.php
    │   ├── passwords.php
    │   └── validation.php
    └── ja.json
```

# 使い方

## 1. `config/app.php`の下記の部分を日本語に指定します。
`en`から`ja`に変更する

```php
    'locale' => 'ja',
    'fallback_locale' => 'ja',
```

## 2. このリポジトリをダウンロードして、上書きする

### マニュアルで対応する場合

ダウンロードした`resouces`ディレクトリをLaravelのルートディレクトリにコピーします。<br>
（Macの場合は、マージコピーする必要があるので、注意)

### コマンド操作で対応する場合
`your/laravel/root`の部分は、ご自身の環境に合わせてください。

```bash
git clone https://github.com/takehirotakiuchi/laravel-8-resources-lang-ja.git
cd laravel-8-resources-lang-ja
cp -pR ./resources your/laravel/root/resources
```

# 参考
- [GitHub - laravel/jetstream](https://github.com/laravel/jetstream)
- [Localization - Laravel - The PHP Framework For Web Artisans](https://laravel.com/docs/master/localization)
