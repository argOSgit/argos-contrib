# ArgOS - Repositorio de contribuciones

Este repositorio está destinado a recibir herramientas que puedan integrarse al sistema operativo ArgOS, un sistema especializado en ciberinteligencia y OSINT.

> Aquí no se aloja la VM ni el sistema operativo, solo los módulos de herramientas.

## ¿Querés contribuir?

1. Forkeá este repo
2. Trabajá sobre la rama `contrib` (no `main`)
3. Seguí las instrucciones en [CONTRIB.md](CONTRIB.md)
4. Subí tu herramienta bajo la estructura:
   herramientas/
   └── categoria/
       └── nombre_tool/
           ├── install.sh
           ├── info.md
           └── usage.md

## Revisión y merge

Todas las herramientas serán revisadas manualmente en una VM de prueba. Si funcionan correctamente, se integran al sistema y se hace merge al `main`.

## Contacto

Para dudas o sugerencias, abrí un issue o escribí en el canal oficial de ArgOS.
