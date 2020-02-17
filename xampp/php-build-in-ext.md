# How to download and install php extension(build-in)


Go to stop Apache on `XAMPP Control Panel` and click on ` Config->php.ini` then Find and Uncomment

## Intl + ICU and ICU Data

```bash
#ctrl+f
#intl
#;extension=intl
extension=intl
#file->save
```

## PDO PostgreSQL

```bash
#;extension=pdo_pgsql
extension=pdo_pgsql
```

## Expose PHP

```bash
#expose_php=On
expose_php=Off
```
