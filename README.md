# AWS Laravel nginx config

AWS上でLaravelを動かすためのnginxやphp-fpmの設定です。

nginx and php-fpm config for Laravel on AWS.

## デプロイ方法 - How to deploy

```sh
# AWSにSSHする - SSH to AWS
ssh ec2-user@<aws-ip> -i <private-key-file-path>

git clone <this-repository>

sudo cp nginx/nginx.conf /etc/nginx/nginx.conf
sudo cp nginx/conf.d/laravel.conf /etc/nginx/conf.d/laravel.conf
sudo cp php-fpm/www.conf /etc/php-fpm.d/www.conf
```

# 上記以外のファイルについて - Files

* nginx/nginx_default.conf
  * 今回の変更を加える前の nginx のデフォルトの設定です
  * nginx default config file
