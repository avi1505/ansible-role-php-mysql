# PHP-MySQL-role

Installeert php-mysql en mysql-client op Ubuntu 24.04.
Bij geupdatet packages wordt Apache herstart.

## Afhankelijkheden

Deze role gebruikt avi1505.php, die avi1505.apache gebruikt.

## Standaardvariabelen

```yaml
php_mysql_packages:
  - php-mysql
  - mysql-client
```

## Voorbeeld

```yaml
---
- name: Webserver met PHP-MySQL configureren
  hosts: webservers
  become: true

  roles:
    - avi1505.php_mysql
```

## Licentie

MIT