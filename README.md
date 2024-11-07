# Proyecto LoRaWAN

Este repositorio contiene los archivos de docker-compose utilizados para la construcción de un proyecto LoRaWAN que conecta Chirpstack con Grafana en tiempo real.

## Contenido de carpetas

* `chirpstack/`: Contiene el archivo docker-compose además de configuración necesaria para correr los servicios
* `grafana/`: Contiene el archivo docker-compose para correr los servicios


# Configuración de Chirpstack

## Importar repositorio de dispositivos LoRaWAN

```bash
make import-lorawan-devices
```

## Ejecutar los servicios

```bash
$ docker-compose up
```

Después que los componentes estén inicilizados se podrá acceder a http://localhost:8080/ en el navegador para la interfaz de **Chirpstack**.

# Configuración de Chirpstack

## Ejecutar los servicios

```bash
$ docker-compose up
```

Después que los componentes estén inicilizados se podrá acceder a http://localhost:3000/ en el navegador para la interfaz de **Grafana** y http://localhost:8086/ para la configuración necesaria con **InfluxDB**.
