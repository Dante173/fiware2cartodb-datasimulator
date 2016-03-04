# Fiware2cartodb - Data Simulator
Data simulator for Fiware Orion to CartoDB connections.

For testing purposes only.

Remark: Under work!

## Requeriments
Fiware Orion to CartoDB connector API deployment:
- Add [fiware-orion2cartodb](https://github.com/GeographicaGS/fiware-orion2cartodb) as submodule. You must properly configure file orion2cartodb.yaml.
- Docker and Docker-Compose.
- Callback URL to send notifications must be visible to Context broker.

Broker (Data Simulator):
- Python >= 2.7 or Python >= 3.4.
- Python Requests library.

## Usage
Run Fiware Orion to CartoDB connector API:
- Build and run Docker Container with Docker-Compose (docker-compose.dev.yml).

Run broker (Data Simulator):
- You must properly configure files (fiware_auth.json and orioncontextbrokerconfig.py; see example files).
- Run data simulator:
```
$ python broker.py
```
- Stop data simulator: CTRL+C
