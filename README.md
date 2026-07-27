# Módulos para la app Biblia

Módulos descargables en formato `.SQLite3`. La app los baja desde los
*releases* de este repositorio; no viajan dentro del APK, para mantenerlo liviano.

## Contenido

### Versiones bíblicas en español

Generadas a partir de los archivos USFM de [eBible.org](https://ebible.org),
tomando únicamente las traducciones marcadas allí como redistribuibles.

| Archivo | Versión | Licencia |
|---|---|---|
| `sparvg.SQLite3` | Reina Valera Gómez | © Humberto Gómez Caballero — redistribución autorizada |
| `spav1602p.SQLite3` | Valera 1602 Purificada | © Iglesia Bautista Bíblica de la Gracia — redistribución autorizada |
| `spabll.SQLite3` | Santa Biblia Libre Latinoamericano | Dominio público |
| `spablm.SQLite3` | Santa Biblia Libre para el Mundo | Dominio público |
| `spaonbv.SQLite3` | Open Nueva Biblia Viva | © Biblica, Inc. — licencia abierta |
| `spapddpt.SQLite3` | Palabra de Dios para Ti | © Asoc. Bíblica Latinoamericana — redistribución autorizada |
| `spabes.SQLite3` | La Biblia en Español Sencillo | © AudioBiblia.org — redistribución autorizada |
| `spavbl.SQLite3` | Versión Biblia Libre | © Gallagher y Barrios de Ávila — redistribución autorizada |

### Léxico

| Archivo | Contenido | Licencia |
|---|---|---|
| `strongs-rvr1909.SQLite3` | Números de Strong sobre el texto RVR1909 | Diccionario de Strong (1890), dominio público. Versión JSON de [Open Scriptures](https://github.com/openscriptures/strongs) (CC BY-SA) |

## Formato

Cada módulo declara su procedencia y licencia en su propia tabla `info`:

```sql
SELECT name, value FROM info;
```

## Nota sobre licencias

Acá solo se publican módulos con permiso de redistribución verificable. El
material licenciado que cada persona haya adquirido por su cuenta se carga
directamente en el dispositivo desde la app, sin pasar por este repositorio.
