# ArgOS - Repositorio de contribuciones

Este repositorio está destinado a recibir herramientas que puedan integrarse al sistema operativo **ArgOS**, un sistema especializado en ciberinteligencia y OSINT.

> Aquí no se aloja la VM ni el sistema operativo, solo los módulos de herramientas.

Repositorio oficial: [https://github.com/argOSgit/argos-contrib](https://github.com/argOSgit/argos-contrib)

---

## ¿Querés contribuir?

Seguí los pasos para enviar tu herramienta de forma correcta:

### 1. Hacé fork del repositorio

Desde: [https://github.com/argOSgit/argos-contrib](https://github.com/argOSgit/argos-contrib)

### 2. Cloná tu fork en tu PC

```bash
git clone git clone https://github.com/argOSgit/argos-contrib.git
cd argos-contrib
```

### 3. Cambiate a la rama `contrib` y actualizá

```bash
git checkout contrib
git pull origin contrib
```

### 4. Creá una nueva rama para tu herramienta

```bash
git checkout -b mi_nueva_tool
```

### 5. Agregá tu herramienta en esta estructura:

```
herramientas/
└── categoria/
    └── nombre_tool/
        ├── install.sh   ← Instalación automatizada
        ├── info.md      ← Descripción + URL oficial
        └── usage.md     ← Instrucciones de uso
```

Ejemplo:
```
herramientas/osint/mi_tool/
├── install.sh
├── info.md
└── usage.md
```

### 6. Hacé commit y push a tu rama

```bash
git add .
git commit -m "Agrego mi_tool en OSINT"
git push origin mi_nueva_tool
```

### 7. Desde GitHub, creá un Pull Request hacia `contrib`

- Nunca hagas PR directo a `main`
- Solo se aceptan PRs contra la rama `contrib`

---

## Revisión y merge

Nosotros vamos a:

- Clonar tu rama en una VM de prueba
- Ejecutar `install.sh`
- Validar que todo funcione
- Hacer merge a `main` solo si está todo correcto

---

## Contacto

Para dudas o sugerencias, abrí un issue en el repositorio oficial o escribí en el canal oficial de ArgOS.

Gracias por tu aporte a la comunidad.
