# Respaldo de fotos del estado de las estaciones de Ecobici

Fotos del feed público GBFS de Ecobici (`station_status`), tomadas cada 5 minutos
(nominal) con GitHub Actions. Es el respaldo de una captura principal por minuto.

- Fuente: https://gbfs.mex.lyftbikes.com/gbfs/gbfs.json
- Cada archivo `estado/AAAA-MM-DD/estado_<marca UTC>.json.gz` es la respuesta cruda del feed.
- `catalogo_*.json.gz` es `station_information` (nombre, ubicación, capacidad), una vez por hora.
- Las fechas y horas de los nombres están en UTC.
- GitHub puede retrasar u omitir corridas: los huecos son esperables.
