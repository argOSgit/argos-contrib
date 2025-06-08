# ArgOS - Repositorio de contribuciones

Este repositorio está destinado a recibir herramientas que puedan integrarse al sistema operativo **ArgOS**, un sistema especializado en ciberinteligencia y OSINT.

> Aquí no se aloja la VM ni el sistema operativo, solo los módulos de herramientas.

Repositorio oficial: [https://github.com/argOSgit/argos-contrib](https://github.com/argOSgit/argos-contrib)

---

## ¿Querés contribuir?

Seguí estos pasos para enviar tu herramienta:

### 1. Hacé fork del repositorio

Entrá a: [https://github.com/argOSgit/argos-contrib](https://github.com/argOSgit/argos-contrib)

Hacé clic en el botón **Fork** (arriba a la derecha).  
Elegí tu cuenta personal como destino del fork. GitHub va a crear una copia del repositorio en tu perfil, por ejemplo:

```
https://github.com/tu_usuario/argos-contrib
```

### 2. Cloná tu fork en tu PC

> Asegurate de clonar tu fork, no el repo original

```bash
git clone https://github.com/tu_usuario/argos-contrib.git
cd argos-contrib
```

### 3. Cambiate a la rama `contrib` y actualizá

```bash
git checkout contrib
git pull origin contrib
```

### 4. Creá una carpeta con la herramienta

Agregá la herramienta en esta estructura:

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

### 5. Hacé commit y push a tu fork

```bash
git add .
git commit -m "Agrego tool en OSINT"
git push origin contrib
```

### 6. Desde GitHub, creá un Pull Request hacia `contrib`

- Nunca hagas PR directo a `main`
- Solo se aceptan PRs contra la rama `contrib` del repositorio original (`argOSgit`)

---

## ¿Querés trabajar solo con una herramienta?

Si no querés clonar todo el repositorio, podés usar `sparse-checkout` para trabajar solo sobre una carpeta específica:

```bash
git clone --filter=blob:none --no-checkout https://github.com/argOSgit/argos-contrib.git
cd argos-contrib
git sparse-checkout init --cone
git sparse-checkout set herramientas/osint/tool
```

Esto te permite clonar únicamente la carpeta de la herramienta sin descargar el resto.

---

## Revisión y merge

Nosotros vamos a:

- Clonar tu fork en una VM de prueba
- Ejecutar `install.sh`
- Validar que todo funcione
- Hacer merge a `main` solo si está todo correcto

---

## Contacto

Para dudas o sugerencias, abrí un issue en el repositorio oficial o escribí en el canal oficial de ArgOS.
