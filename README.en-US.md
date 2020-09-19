# Laravel 8 JetStream 日本語化ファイル

A set of Japanese message files for Laravel 8.
The necessary parts are Japaneseized for dashboards and so on.

To be specific, this corresponds to the part described in `{{{ __('message') }}} for i18n.

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

# Usage

## 1.  Change the locale specified in the file `config/app.php` to Japanese. Changing from `en` to `ja`

```php
    'locale' => 'ja',
    'fallback_locale' => 'ja',
```

## 2. このリポジトリをダウンロードして、上書きする

### GUI Operation

Copy the `resouces` directory downloaded from this repository to your Laravel root directory.

### Command Operation
Please change the `your/laravel/root` part to your environment.

```bash
git clone https://github.com/takehirotakiuchi/laravel-8-resources-lang-ja.git
cd laravel-8-resources-lang-ja
cp -pR ./resources your/laravel/root/resources
```

# 参考
- [GitHub - laravel/jetstream](https://github.com/laravel/jetstream)
- [Localization - Laravel - The PHP Framework For Web Artisans](https://laravel.com/docs/master/localization)
