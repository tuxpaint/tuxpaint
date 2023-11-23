# Tabla de contenidos
1. [Hacking Ético](#HackingEtico)
2. [Bastionado](#Bastionado)
3. [Forense](#Forense)
4. [PPS](#PPS)

# HackingEtico

#### Hacking Web
- [Burp Suite](https://portswigger.net/burp) - Suite de herramientas de hacking web para probar y explotar vulnerabilidades en aplicaciones web (herramienta gráfica).
- [SQLMap](https://github.com/sqlmapproject/sqlmap) - Herramienta de automatización de inyección SQL para probar vulnerabilidades en bases de datos (herramienta de línea de comandos).
Ejemplo de uso: `sqlmap -u "http://example.com/?id=1" --dbms=mysql --dump` donde `http://example.com/?id=1` es la URL de la aplicación web vulnerable, `--dbms=mysql` indica el tipo de base de datos y `--dump` indica que deseas descargar toda la información de la base de datos.
- [OWASP ZAP](https://www.zaproxy.org/) - Proxy de seguridad web de código abierto que se puede utilizar para encontrar y explotar vulnerabilidades (herramienta gráfica).
- [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings) - Repositorio con una lista de payloads y bypasses útiles para Hacking Web (Repositorio Github y página Web).


#### OSINT

- [The Harvester](https://github.com/laramies/theHarvester) - Herramienta de recopilación de información que puede buscar correos electrónicos, nombres de usuario, hostnames, etc. en fuentes públicas (herramienta de línea de comandos).
Ejemplo de uso: `theharvester -d example.com -l 500 -b google` donde `example.com` es el dominio que deseas analizar, `-l 500` indica que deseas limitar la salida a 500 resultados y `-b google` indica que deseas usar la búsqueda de Google.
- [Maltego](https://www.maltego.com/) - Herramienta de investigación y análisis de enlaces para recopilar información y relaciones en línea (herramienta gráfica).

# Forense

#### Suites forenses

- [Autopsy](https://www.sleuthkit.org/autopsy/) - Herramienta de análisis forense que puede analizar imágenes de discos y sistemas de archivos (herramienta gráfica).

    - **WriteUps de ejemplo**:    
        - ![Forense en Windows](https://github.com/UchaCTF/WriteUps/tree/main/Forense/Windows/San%20Clemente%20CASO%20%232)

- [Bulk Extractor](https://github.com/simsong/bulk_extractor) - Herramienta de análisis forense digital que extrae automáticamente información como correos electrónicos, números de tarjeta de crédito y URLs de archivos, imágenes de disco y volcados de memoria (herramienta de línea de comandos). Ejemplo de uso: `bulk_extractor -o salida carpeta_imagen.dd` donde `salida` es la carpeta de destino para los resultados del análisis y `carpeta_imagen.dd` es la imagen de disco o archivo que se va a analizar.

- [OS Forensics](https://www.osforensics.com/) (versión de prueba limitada a 30 días)

- [FTK Imager](https://accessdata.com/product-download/ftk-imager-version-4-5)

- [SDL Redline](https://www.mandiant.com/resources/download/redline)

#### Análisis de memoria RAM

- [Volatility](https://www.volatilityfoundation.org/) - Herramienta de análisis de memoria para extraer información de la memoria volátil de un sistema (herramienta de línea de comandos).
Ejemplo de uso: `volatility -f memoria.mem imageinfo` donde `memoria.mem` es el archivo de imagen de memoria volátil que deseas analizar.

    - **WriteUps de ejemplo**:    
        - ![Forense en Windows](https://github.com/UchaCTF/WriteUps/tree/main/Forense/Windows/San%20Clemente%20CASO%20%232)

#### Montaje de imágenes

- [OSF Mount](https://www.osforensics.com/tools/mount-disk-images.html)

#### Editor hexadecimal de disco

- [Active disk Editor](https://www.disk-editor.org/)

#### Análisis de MFT

- [Mft2Csv_old](https://tzworks.net/prototype_page.php?proto_id=3)
- [Mft2Csv](https://github.com/jschicht/Mft2Csv/releases/tag/v2.0.0.49)

#### Análisis de LogFile y UsnJrnl

- [Log File Parser](https://github.com/jschicht/LogFileParser)
- [NTFS Log Tracker](https://github.com/jschicht/NTFS-Log-Tracker)

#### Análisis del registro de Windows

- [RegRipper](https://github.com/keydet89/RegRipper3.0)
- [Windows Registry Recover](https://www.nirsoft.net/utils/windows_registry_recovery.html)
- [Registry Explorer](https://ericzimmerman.github.io/#!index.md)
- [RECmd](https://ericzimmerman.github.io/#!index.md)
- [USBDeview](https://www.nirsoft.net/utils/usb_devices_view.html) (análisis de dispositivos USB)
- [USB Detective](https://www.13cubed.com/products) (análisis de dispositivos USB)

#### Análisis de los logs de windows (Event Log)

- [FullEventLogView](https://www.nirsoft.net/utils/full_event_log_view.html) de Nirsoft

#### Análisis de Prefetch y Superfetch

- [WindowsPrefetchView](https://www.nirsoft.net/utils/win_prefetch_view.html) de Nirsoft
- [CrowdResponse](https://www.crowdstrike.com/resources/community-tools/crowdresponse/)

#### Análisis del registro de actividad

- [Windows Timeline Parser](https://github.com/kacos2000/WindowsTimeline)
- [WxTCmd](https://github.com/EricZimmerman/WxTCmd)

#### Análisis de la papelera de reciclaje

- [Rifiuti2](https://github.com/abelcheung/rifiuti2)
- [RBCmd](https://github.com/kacos2000/RecycleBin)

#### Registros de seguimiento (Event Log Tracer, etl)

- [ETLParser](https://github.com/woanware/etlparser)

#### Navegadores Web

- [SQLite Studio](https://sqlitestudio.pl/)
- [IE HistoryView](https://www.nirsoft.net/utils/iehv.html) de Nirsoft
- [ESEDatabaseView](https://www.nirsoft.net/utils/ese_database_view.html) de Nirsoft
- [BrowsingHistoryView](https://www.nirsoft.net/utils/browsing_history_view.html) de Nirsoft
- [IECookiesView](https://www.nirsoft.net/utils/iecookies.html) de Nirsoft
- [EdgeCookiesView](https://www.nirsoft.net/utils/edge_cookies_view.html) de Nirsoft
- [IECacheView](https://www.nirsoft.net/utils/ie_cache_viewer.html) de Nirsoft
- [MZCacheView](https://www.nirsoft.net/utils/mozilla_cache_viewer.html) de Nirsoft
- [ChromeHistoryView](https://www.nirsoft.net/utils/chrome_history_view.html) de Nirsoft
- [ChromeCookiesView](https://www.nirsoft.net/utils/chrome_cookies_view.html) de Nirsoft
- [ChromeCacheView](https://www.nirsoft.net/utils/chrome_cache_view.html) de Nirsoft

#### Correo electrónico

- [PST Viewer](https://www.nucleustechnologies.com/pst-viewer.html)
- 👋 Hi, I’m @tuxpaint
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
tuxpaint/tuxpaint is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
