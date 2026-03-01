# MySQL + PHPMyAdmin

## Előkészületek

- `.env.example` fájlban találhatóak a szükséges környezeti változók. Amennyiben nem az alapértelmezett értékekre van szükség, ezt a fájlt le kell másolni és átnevezni `.env`-re, majd felülírni a szükséges értékeket.

## Futtatás

```bash
bash start.sh
```

## Leállítás

```bash
docker compose stop
```

## Eltávolítás

```bash
docker compose down # -v opcionális, a volume-ok törléséhez
```

## MySQL elérése

- Host: `localhost`
- Port: `3306`
- Felhasználónév: a `.env` fájlban megadott `MYSQL_USER` érték
- Jelszó: a `.env` fájlban megadott `MYSQL_PASSWORD` érték
- Adatbázis: a `.env` fájlban megadott `MYSQL_DATABASE` érték

## PHPMyAdmin elérése

- URL: <http://pma.localhost>
- Szerver: üresen hagyható, amennyiben az `.env` fájlban meg van adva a `PMA_HOST` érték
- Felhasználónév: a `.env` fájlban megadott `MYSQL_USER` érték
- Jelszó: a `.env` fájlban megadott `MYSQL_PASSWORD` érték
