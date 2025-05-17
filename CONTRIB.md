# Guía de contribución a ArgOS

Gracias por tu interés en contribuir al sistema operativo ArgOS. Este repositorio contiene solamente los módulos o herramientas que pueden integrarse al sistema.

Este repositorio no incluye la VM ni el sistema operativo, únicamente las herramientas complementarias.

## Qué tipo de contribuciones se aceptan

Se aceptan herramientas relacionadas exclusivamente con Ciberinteligencia u OSINT, que sean funcionales, legales, y con utilidad clara.

Cada herramienta debe incluir:

- Script de instalación automatizado (`install.sh`)
- Descripción breve con URL oficial (`info.md`)
- Guía de uso básica (`usage.md`)

## Estructura del repositorio

```
herramientas/
└── categoria/
    └── nombre_tool/
        ├── install.sh   ← Instalación automatizada
        ├── info.md      ← Descripción breve + enlace oficial
        └── usage.md     ← Instrucciones de uso
```

## Instrucciones para contribuir

1. Hacé fork de este repositorio.
2. Cloná tu fork localmente:
   git clone https://github.com/tu_usuario/argos-contrib.git
   cd argos-contrib

3. Cambiate a la rama de contribución:
   git checkout contrib
   git pull origin contrib

4. Creá una nueva rama con el nombre de tu herramienta:
   git checkout -b mi_tool
