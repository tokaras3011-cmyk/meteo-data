# meteo-data

Publikovaná data pro aplikaci **Meteo VČ**.

`weights.json` — váhy modelů z verifikace proti staničním datům ČHMÚ (MAE teploty za
poslední 3 dny) + kalibrace bouřkové pravděpodobnosti. Zapisuje `ingest.ps1`, aktualizuje se
1× za hodinu naplánovanou úlohou `MeteoIngest`.

Aplikace si soubor stahuje z `raw.githubusercontent.com`, protože staniční data ČHMÚ nemají
CORS a verifikace tedy nemůže běžet přímo v telefonu.
