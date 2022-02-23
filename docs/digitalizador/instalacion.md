# Instalación




## Elementos de instalación

Para que el digitalizador funcione de forma correcta es necesario que disponga de los siguientes elementos:
1. Archivo de configuración con extensión YAML.
2. Carpeta dedicada para el almacenamiento de archivos de logs.
3. Ejecutable setup.exe.


```yaml
connection:
  driver: "SQL Server Native Client 11.0"
  server: "DESKTOP-HO3ONG6"
  user: "sa"
  password: "sa"
  database: "aduasism3_n"

debug: true

digitalizadores:
  pedimentoCompleto: off
  pedimentoPartida: off
  acuseEDocument: off
  acuseCove: off
  coveXML: on

motor:
  #(Tiempo maximo de espera para responder una peticion)
  segundos_de_timeout: 20 
  #(Para evitar bloqueos por parte de VUCEM)
  minutos_de_reposo: 1 
   #(Cantidad de veces que una peticion debe repetirse en caso de fallar)
  reintentos: 4
  #(Cantidad de referencias a digitalizar por oleada)
  cantidad_de_referencias: 30

logs:
  #(Logs por TXT)
  path: "C:\\Users\\ADUASIS-PIPE\\Documents\\logs\\"
  txt: on
  #(Logs desde consola [aplica solo en entorno de pruebas])
  cmd: off
```
