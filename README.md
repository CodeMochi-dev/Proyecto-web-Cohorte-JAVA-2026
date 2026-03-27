# Portafolio Cohorte 24 — Javalimos

Galería de perfiles del cohorte. Cada alumno tiene su tarjeta en el landing y su propio CV dentro de la carpeta `CVs/`.

---

## Cómo agregar tu CV al proyecto

Seguí estos pasos para incorporar tu perfil a la galería.

### 1. Hacer un fork del repositorio

Entrá al repositorio en GitHub:
👉 https://github.com/N4t0-tech/Proyecto-web-Cohorte-JAVA-2026

Hacé click en el botón **Fork** (arriba a la derecha). Esto crea una copia del proyecto en tu cuenta de GitHub.

---

### 2. Clonar tu fork localmente

En tu terminal, cloná **tu fork** (reemplazá `TU-USUARIO` con tu nombre de usuario de GitHub):

```bash
git clone https://github.com/TU-USUARIO/Proyecto-web-Cohorte-JAVA-2026.git
```

Entrá a la carpeta del proyecto:

```bash
cd Proyecto-web-Cohorte-JAVA-2026
```

---

### 3. Crear tu carpeta de CV

Dentro de la carpeta `CVs/`, creá una carpeta con el formato `Cv-NombreApellido`:

```
CVs/
├── CV-AlumEjemplo/
├── Cv-RenaCampos/
└── Cv-TuNombreTuApellido/   ← la tuya
```

Dentro de tu carpeta agregá al menos estos dos archivos:

```
Cv-TuNombreTuApellido/
├── index.html
└── style.css
```

Podés usar el CV que hiciste en la actividad anterior o crear uno nuevo desde cero. Lo importante es que el archivo principal se llame `index.html`.

---

### 4. Agregar tu perfil a la galería

Abrí el archivo `script.js` y agregá una entrada al array `profiles`. Copiá el bloque de ejemplo y completá tus datos:

```js
{
  name: 'Tu Nombre',
  role: 'Tu rol (ej: Frontend Developer)',
  bio: 'Una descripción breve tuya: intereses, stack, lo que quieras destacar.',
  github: 'https://github.com/tu-usuario',
  linkedin: 'https://linkedin.com/in/tu-usuario',
  cvPath: 'CVs/Cv-TuNombreTuApellido/index.html',
},
```

> **Importante:** el valor de `cvPath` tiene que coincidir exactamente con el nombre de la carpeta que creaste en el paso anterior.

---

### 5. Commitear y subir los cambios

```bash
git add CVs/Cv-TuNombreTuApellido/ script.js
git commit -m "feat: agrego CV de Tu Nombre"
git push origin main
```

---

### 6. Abrir un Pull Request

1. Andá a tu fork en GitHub
2. Hacé click en **Contribute → Open pull request**
3. Verificá que los cambios sean solo los tuyos (tu carpeta y tu entrada en `script.js`)
4. Poné un título descriptivo, por ejemplo: `feat: agrego CV de Tu Nombre`
5. Enviá el PR

Una vez aprobado y mergeado, tu tarjeta va a aparecer en el landing del cohorte. ✓

---

## Estructura del proyecto

```
Proyecto-web-Cohorte-JAVA-2026/
├── index.html          # Landing con la galería de perfiles
├── style.css           # Estilos del landing
├── script.js           # Datos de perfiles y renderizado de tarjetas
└── CVs/
    ├── CV-AlumEjemplo/ # Carpeta de ejemplo
    └── Cv-RenaCampos/  # CV de cada alumno
```
