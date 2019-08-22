# [composer](https://getcomposer.org/)

## install

- windows
  
  Download and Run [Composer-Setup.exe](https://getcomposer.org/Composer-Setup.exe).

- linux
  ```php
    php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
    php -r "if (hash_file('sha384', 'composer-setup.php') === 'a5c698ffe4b8e849a443b120cd5ba38043260d5c4023dbf93e1558871f1f07f58274fc6f4c93bcfd858c6bd0775cd8d1') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
    php composer-setup.php --install-dir=/usr/local/bin  --filename=composer
    php -r "unlink('composer-setup.php');"
  ```

- 镜像
  - 全局配置
  ```
    composer config -g repo.packagist composer https://mirrors.aliyun.com/composer/
  ```
  - 项目配置
  ```
    composer config repo.packagist composer https://mirrors.aliyun.com/composer/
  ```
  - 取消配置
  ```
    composer config -g --unset repos.packagist
  ```
  