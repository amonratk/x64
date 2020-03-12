# How to enable some extension

## enabled mbstring

1. Checking exist dll first `C:\tools\php74\ext` should be exist `php_mbstring.dll`
2. Enabled via uncommend file on `C:\tools\php74\php.ini`

```bash
;extension=mbstring
extension=mbstring
```

## enabled curl

1. Checking exist dll first `C:\tools\php74\ext` should be exist `php_curl.dll`
2. Enabled via uncommend file on `C:\tools\php74\php.ini`

```bash
;extension=curl
extension=curl
```

## enabled intl

1. Checking exist dll first `C:\tools\php74\ext` should be exist `php_intl.dll`
2. Enabled via uncommend file on `C:\tools\php74\php.ini`

```bash
;extension=intl
extension=intl
```

## enabled soap

1. Checking exist dll first `C:\tools\php74\ext` should be exist `php_soap.dll`
2. Enabled via uncommend file on `C:\tools\php74\php.ini`

```bash
;extension=soap
extension=soap
```

## enabled mysql

1. Checking exist dll first `C:\tools\php74\ext` should be exist `php_pdo_mysql.dll`
2. Enabled via uncommend file on `C:\tools\php74\php.ini`

```bash
;extension=pdo_mysql
extension=pdo_mysql
```

## enabled SQL Server

1. Download dll files <a href="https://go.microsoft.com/fwlink/?linkid=2120362">Download</a>
2. Double click `SQLSRV58.EXE`
3. Accept all of terms then click `Yes`
4. Browse directory to paste dll file then press `OK`
5. Copy `php_sqlsrv_74_nts_x64.dll` and `php_pdo_sqlsrv_74_nts_x64.dll` to `C:\tools\php74\ext`
6. Update `C:\tools\php74\php.ini`

```bash
extension=sqlsrv_74_nts_x64
extension=pdo_sqlsrv_74_nts_x64
```

## enabled PHP Accelerator

1. Download dll files <a href="https://windows.php.net/downloads/pecl/releases/apcu/5.1.18/php_apcu-5.1.18-7.4-nts-vc15-x64.zip">Download</a>
2. Unzip `php_apcu-5.1.18-7.4-nts-vc15-x64.zip` and give up `php_apcu.dll`
3. Copy `php_apcu.dll` and paste to `C:\tools\php74\ext`
4. Update `C:\tools\php74\php.ini` 

```bash
extension=apcu
```
