# PHP Configuration

## PHP ini

### General configuration
#### General
```ini
upload_max_filesize = 32M
```
#### Extension
```ini
extension=bz2
extension=curl
extension=ffi
extension=ftp
extension=fileinfo
extension=gd2
extension=gettext

extension=mbstring
extension=exif      ; Must be after mbstring as it depends on it
extension=mysqli

extension=pdo_mysql
extension=pdo_sqlite

```
### Environment
#### Development
```ini
zend.exception_ignore_args = Off
```
```ini
error_reporting = E_ALL
display_errors = On
display_startup_errors = On
```

#### Production
```ini
zend.exception_ignore_args = On
```
```ini
error_reporting = E_ALL & ~E_DEPRECATED & ~E_STRICT
display_errors = Off
display_startup_errors = Off
```

