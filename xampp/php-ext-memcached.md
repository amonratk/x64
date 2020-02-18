# How to download and install php extension (manual)

## Pecl

### Checking commend first

```bash
D:\> pecl list
(no packages installed from channel pecl.php.net)
```
```bash
D:\> pecl version
PEAR Version: 1.10.1
PHP Version: 7.4.2
Zend Engine Version: 3.4.0
Running on: Windows NT THRL-11154 10.0 build 17134 (Windows 10) AMD64
```

## Memcached

find
```bash
D:\> pecl search memcached
=======================================
PACKAGE   STABLE/(LATEST) LOCAL
memcached 3.1.5 (stable)        PHP extension for interfacing with memcached via libmemcached library
```

## Note

### Problem

while installation appear this error
```bash
WARNING: channel "pecl.php.net" has updated its protocols, use "pecl channel-update pecl.php.net" to update
```

### Fixed

```bash
> php -r "print_r(openssl_get_cert_locations());"
```

```bash
> pecl channel-update pecl.php.net
Updating channel "pecl.php.net"
Channel "pecl.php.net" is up to date
```

## Via Manual

### Download

1. Go to <a href="https://pecl.php.net/package/memcache">pecl.php.net</a>
2. Click download link of DLL with last release date
3. Choose 7.4 Thread Safe(TS) x64 (`https://windows.php.net/downloads/pecl/releases/memcache/4.0.5.2/php_memcache-4.0.5.2-7.4-ts-vc15-x64.zip`)
4. Unzip and copy `php_memcache.dll` to `D:\xampp\php\ext`
5. Update `php.ini` file


php.ini
```bash
extension=php_memcache.dll
```

## Friend


<https://github.com/yshurik/libmemcached-win/releases/tag/1.0.18>
