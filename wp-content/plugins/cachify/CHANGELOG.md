# Changelog
All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).

## 2.3.1
* Fix: clean up unused parameter evaluation after publishing a post to prevent PHP notice (#187) (#188)
* Fix: correct minor spelling mistakes (#193, props timse201)
* Fix: update support links (#194, props timse201)

## 2.3.0
* New: WP-CLI integration (#165, props derweili)
* New: `cachify_flush_cache_hooks` filter added to modify all hooks that flush the cache
* New: Flush cache when a user is created / updated / deleted
* New: Flush cache when a term is created / updated / deleted (#169, props derweili)
* New: Cache behavior after post modification is now configurable in plugin settings (#176)
* Enhance: Cache exceptions/User-Agents translation (#52, props timse201)
* Enhance: Readme FAQ (#51, props timse201)
* Enhance: sizeable exclusion boxes + placeholder (#53, props timse201)
* Enhance: FAQ and Support links (#55, props timse201)
* Enhance: Add text caption to "flush cache" button
* Enhance: Icon font converted to SVG (#64)
* Enhance: Improved HDD cache invalidation for hierarchical post types (#71, props Syberspace)
* Enhance: Unified and shortened HTML signature across all caching methods (#108) (#109)
* Security: Tabnabbing prevention (#55, props timse201)
* Maintenance: Tested up to WordPress 5.4


## 2.2.4
* Fixes caching for mixed HTTPS and HTTP setups
* Fixes an issue with the icon styling in the admin toolbar
* Ensures compatibility with the latest WordPress version

## 2.2.3
* New: Generated a POT file
* New: Added German formal translation
* Updated, translated + formatted README.md
* Updated expired link URLs in plugin and languages files
* Updated plugin authors

## 2.2.2
* Fix: parameter return by filter dashboard_glance_items
* Generous use of the filter esc_html

## 2.2.1
* Fix for the PHP notice "Call to undefined function is_plugin_active_for_network" on WordPress Multisite

## 2.2.0
* Toolbar: Display of the "Flush the cachify cache" button on the frontend
* Toolbar: Controlling the display of the "Flush the cachify cache" button via hook

## 2.1.9
* Vervollst??ndigung des Cachify-Pfades in `robots.txt`: `Disallow: /wp-content/cache/cachify/`
* *Release-Zeitaufwand (Development & QA): 0,75 Stunden*

## 2.1.8
* HHVM-Unterst??tzung f??r die *Memcached* Caching-Methode (Danke, [Ulrich Block](http://www.ulrich-block.de))

## 2.1.7
* Cache-Leerung bei Custom Post Types
* Einf??hrung zus??tzlicher Sicherheitsabfragen
* Code-Refactoring

## 2.1.6
* Button "Cache leeren" sichtbar sowohl in WP 3.8 wie WP 3.9

## 2.1.5
* Support f??r WordPress 3.9
* Button "Cache leeren" sichtbar bei jeder Bildschirmaufl??sung

## 2.1.4
* Support f??r WordPress 3.8.1

## 2.1.3
* Manuelle Auswahl: Beim Artikel-Update nur den Seitencache l??schen
* Lokalisierung der Plugin-Dateien
* Umbauten am Plugin-Core
* Detaillierter auf [Google+](https://plus.google.com/+SergejM??ller/posts/By2PEtRMk8g)

## 2.1.2
* Optimierung f??r WordPress 3.8
* Option hinzugef??gt: Neue Kommentare l??sen einen Cache-Reset aus

## 2.1.1
* Hook `cachify_skip_cache` f??r die Steuerung der Cache-Generierung
* Support f??r das MP6 Plugin
* Detaillierter auf [Google+](https://plus.google.com/110569673423509816572/posts/S1mpFsG3NZC)

## 2.1.0
* Cache-Leerung bei Plugin-Deaktivierung

## 2.0.9
* Quelltext-Minimierung als Selektbox und Hook
* Interne Umstellung auf Konstanten

## 2.0.7
* Unterst??tzung f??r Memcached
* WordPress 3.6 Support
* Cache-Neuaufbau beim Theme-Wechsel
* Quelltext-Optimierungen

## 2.0.6
* Cache-Neuaufbau einer Blogseite nur bei Kommentaren, die freigegeben sind

## 2.0.5
* Cache-Leerung nach einem WordPress-Upgrade
* Keine Cache-Ausgabe f??r Jetpack Mobile Theme
* Abfrage auf eingeloggte Nutzer bei APC als Caching-Methode
* ??nderung der Systemvoraussetzungen
* Cache-Reset nach WordPress-Update

## 2.0.4
* Bessere Trennung der Cache-Gesamtgr????e im Dashboard-Widget "Auf einen Blick"

## 2.0.3
* Cache-Leerung beim Ver??ffentlichen verf??gbarer Custom Post Types
* Noindex in der von WordPress generierten `robots.txt` f??r den Ordner mit HDD-Cache
* Hook `cachify_flush_cache` zum Leeren des Cache aus Drittanwendungen

## 2.0.2
* Unterst??tzung f??r WordPress 3.4
* Hochaufl??sende Icons f??r iPad & Co.
* Anpassungen f??r ??ltere PHP5-Versionen
* Entfernung des Plugin-Icons aus der Sidebar

## 2.0.1
* Verbesserter Autoload-Prozess
* Diverse Umbenennungen der Optionen
* Cache-Neuaufbau bei geplanten Beitr??gen (Cachify DB)

## 2.0
* ??berarbeitung der GUI
* Source Code-Modularisierung
* Cache-Gr????e auf dem Dashboard
* Festplatte als Ablageort f??r Cache
* Produktseite online: http://cachify.de
* Cache-Neuaufbau bei Kommentarstatus??nderungen
* APC-Anforderungen: APC 3.0.0, empfohlen 3.1.4
* Optional: Kein Cache f??r kommentierende Nutzer
* Schnell??bersicht der Optionen als Inline-Hilfe
* Mindestanforderungen: WordPress 3.1 & PHP 5.1.2

## 1.5.1
* `zlib.output_compression = Off` f??r Apache Webserver

## 1.5
* ??berarbeitung des Regexp f??r HTML-Minify
* Reduzierung des Toolbar-Buttons auf das Icon
* Formatierung und Kommentierung des Quelltextes

## 1.4
* Xmas Edition

## 1.3
* Unterst??tzung f??r APC (Alternative PHP Cache)
* Umpositionierung des Admin Bar Buttons

## 1.2.1
* Icon f??r die "Cache leeren" Schaltfl??che in der Admin Bar

## 1.2
* Schaltfl??che "Cache leeren" in der Adminbar (ab WordPress 3.1)
* `flush_cache` auf public gesetzt, um von [wpSEO](http://wpseo.de "WordPress SEO Plugin") ansprechen zu k??nnen
* Ausf??hrliche Tests unter WordPress 3.3

## 1.1
* Interne Pr??fung auf fehlerhafte Cache-Generierung
* Anpassungen an der Code-Struktur
* Entfernung der Inline-Hilfe
* Verkn??pfung der Online-Hilfe mit Optionen

## 1.0
* Leerung des Cache beim Aktualisieren von statischen Seiten
* Seite mit Plugin-Einstellungen
* Inline-Dokumentation in der Optionsseite
* Ausschluss von Passwort-gesch??tzten Seiten
* WordPress 3.2 Support
* Unterst??tzung der WordPress Multisite Blogs
* Umstellung auf den template_redirect-Hook (Plugin-Kompatibilit??t)
* Interne Code-Bereinigung

## 0.9.2
* HTML-Kompression
* Flattr-Link

## 0.9.1
* Cache-Reset bei geplanten Beitr??gen
* Unterst??tzung f??r das Carrington-Mobile Theme

## 0.9
* Workaround f??r Redirects

## 0.8
* Blacklist f??r PostIDs
* Blacklist f??r UserAgents
* Ausnahme f??r WP Touch
* Ausgabe des Zeitpunktes der Generierung
* Umbenennung der Konstanten

## 0.7
* Ausgabe des Speicherverbrauchs

## 0.6
* Live auf wordpress.org
