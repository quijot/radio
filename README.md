# radio

__radio__, un script python para escuchar la radio con mplayer

# Instalación

Descargar y descomprimir.

## Requisitos previos

GNU/Linux, python, mplayer. (Quizás también funcione en win y/o mac.)

# Uso

    $ ./radio <radio_id>

donde <radio_id> debe estar en alguna lista (archivos _.list_ en el directorio __lists__).

(Para _apagar la radio_, presione _Ctrl+C_.)

Si ejecuta

    $ ./radio

se imprime la ayuda.

## Listas de radios

Se administran en archivos con extensión _.list_.

Dentro del directorio donde está __radio__, debería encontrarse un directorio llamado _lists_ y allí dentro, un archivo oculto llamado _.default.list_. Si tiene el comando _tree_ instalado, pruebe, ubicado dentro del directorio donde está __radio__

    $ tree -a
        .
        ├── LICENSE
        ├── lists
        │   ├── .default.list
        │   └── ar.list
        ├── radio
        ├── radio_conf.py
        └── README.md

### Agregar radios

Puede agregar información de radios puede editar _.default.list_ o agregar archivos _.list_ con el mismo formato interno de _.default.list_, por ejemplo, se adjunta también _ar.list_ con radios de Argentina.

Dentro de _.default.list_ está indicado cómo agregar la información:

Para agregar una radio agregue una línea:
    radio_id: radio_name|radio_url

Por ejemplo:
    ahijuna: Radio Ahijuna FM 94.7|mms://200.110.208.108/ahijunafm

