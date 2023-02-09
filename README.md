# Erudita

Erudita ist eine Online-Enzyklopädie, die es Nutzern ermöglicht, Wissen aus verschiedenen Bereichen zu suchen und zu teilen. Mit Erudita können Nutzer Artikel lesen und bearbeiten, um das Wissen, das sie mit der Gemeinschaft teilen möchten, zu verbreiten.

## Features
- Suchfunktion, um nach bestimmten Artikeln oder Themen zu suchen
- Möglichkeit, Artikel zu bearbeiten und zu verbessern
- Abschnitte, die sich auf spezifische Themen beziehen, um das Lesen zu erleichtern
- Verlinkung zu externen Quellen, um das Lernen zu vertiefen

## Installation
### Anforderungen:
Wir nutzen folgende Software zur Entwicklung:

- PostgreSQL
- pgAdmin
- Apache24
- PHP8
- Composer

### PHP Konfiguration:
aktivieren Sie folgende Erweiterungen in `php.ini`:
- curl
- gd
- mbstring
- pdo_pgsql

### Composer:
(Sie müssen Composer installiert haben: [https://getcomposer.org/download/](https://getcomposer.org/download/))

Installieren Sie folgende Pakete:  

    composer require --dev phpunit/phpunit -W
>

    composer require erusev/parsedown
    
>

### Datenbank:
1. Erstellen Sie in pgAdmin eine Datenbank namens `Erudita`.
2. Importieren Sie `database.sql` (aus dem Projekt `database`) in pgAdmin, um die nötigen Tabellen in `Erudita` zu erstellen. 

### Zugangsdaten: 
1. Erstellen Sie im Projekt `webserver` eine Datei `credentials.php` und erstellen Sie dort folgende Variablen:

```php
$DB_HOST = ''; // DB host name e.g. example.com
$DB_PORT = 5432; // DB port, usually 5432
$DB_NAME = ''; // DB name e.g.'Erudita' (up to you)
$DB_USER = ''; // DB username, usually 'postgres'
$DB_PASS = ''; // DB password
```

1. Tragen Sie ihre restlichen Datenbank Zugangsdaten in `config.php` ein.
2. Erstellen Sie bei Google einen reCAPTCHA `site_key` und tragen Sie diesen ebenfalls in `config.php` ein. (public key)

## Benutzung
Um Erudita zu nutzen, besuchen Sie einfach die Website und geben Sie in der Suchleiste den Namen des Artikels oder Themas ein, nach dem Sie suchen. Sie können auch durch die verschiedenen Kategorien navigieren, um mehr über ein bestimmtes Thema zu erfahren. Wenn Sie möchten, können Sie sich auch registrieren, um Artikel zu bearbeiten und neue Artikel hinzuzufügen.

## Datenbank
Nähere Informationen über unsere Datenbank finden Sie hier: [database/README.md](https://github.com/EruditaWiki/database/blob/main/README.md)

## Roadmap
Roadmap for future features: [Readmap.md](Roadmap.md)

## Mitwirkende
- Kevin Tamme
- Dominik Hein
- Rares Velnic

## Lizenz
Erudita wird unter der Apache License 2.0 veröffentlicht. Weitere Informationen finden Sie in der [LICENSE](LICENSE) Datei.
