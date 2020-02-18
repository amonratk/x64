# How to install APCu extension to XAMPP

## Download

### APCu

1. Go to <a href="http://pecl.php.net/package/apcu">pecl.php.net</a>
2. Click download link of DLL with last release date
3. Choose 7.x Thread Safe(TS) x64
4. Unzip and copy `php_apcu.dll` to `D:\xampp\php\ext`
5. Update `php.ini` file

php.ini
```bash
extension=php_apcu.dll
```

### APCu

1. Go to <a href="http://pecl.php.net/package/apcu_bc">pecl.php.net</a>
2. Click download link of DLL with last release date
3. Choose 7.x Thread Safe(TS) x64
4. Unzip and copy `php_apc.dll` to `D:\xampp\php\ext`
5. Update `php.ini` file

php.ini
```bash
extension=php_apc.dll
```

### XDebug

php.ini
```bash
extension=php_xdebug.dll
output_buffering=Off
```

## Reference

<https://kapilpatel84.wordpress.com/2016/06/15/install-xdebug-apcu-on-windows-xampp-for-php7/>