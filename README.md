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


    `composer require --dev phpunit/phpunit`  
>
    `composer require erusev/parsedown`

### Datenbank:
1. Erstellen Sie in pgAdmin eine Datenbank namens `Erudita`.
2. Importieren Sie `database/database.sql` in pgAdmin, um die nötigen Tabellen in `Erudita` zu erstellen. 

### Zugangsdaten: 
1. Erstellen Sie eine Datei `credentials.php` und erstellen Sie dort eine variable `$DB_PASS`, die ihr Datenbankpasswort enthält.
1. Tragen Sie ihre restlichen Datenbank Zugangsdaten in `config.php` ein.
2. Erstellen Sie bei Google einen reCAPTCHA `site_key` und tragen Sie diesen ebenfalls in `config.php` ein. 

## Benutzung
Um Erudita zu nutzen, besuchen Sie einfach die Website und geben Sie in der Suchleiste den Namen des Artikels oder Themas ein, nach dem Sie suchen. Sie können auch durch die verschiedenen Kategorien navigieren, um mehr über ein bestimmtes Thema zu erfahren. Wenn Sie möchten, können Sie sich auch registrieren, um Artikel zu bearbeiten und neue Artikel hinzuzufügen.

## Roadmap
- Integration von Multimedia-Inhalten wie Videos und Audiodateien
- Möglichkeit, Artikel in andere Sprachen zu übersetzen
- Verbesserung der Benutzeroberfläche und -erfahrung

## Mitwirkende
- Raresh Velnik
- Kevin Palme
- Dominik Hein

## Lizenz
Erudita wird unter der MIT-Lizenz veröffentlicht. Weitere Informationen finden Sie in der [LICENSE](LICENSE) Datei.
