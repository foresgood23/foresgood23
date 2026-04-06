# >_ CMD & PowerShell — Buscador de Errores

Herramienta web para buscar errores comunes de CMD y PowerShell con soluciones paso a paso.

![HTML](https://img.shields.io/badge/HTML-5-orange?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-3-blue?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-black?logo=github)

---

## Características

- Búsqueda en tiempo real por código de error, título o descripción
- Filtros por shell: CMD, PowerShell o ambos
- Soluciones paso a paso con comandos copiables con un clic
- 12+ errores documentados con causa y solución
- Diseño dark mode, sin dependencias externas
- 100% deployable en GitHub Pages

---

## Demo en vivo

 **[Ver demo](https://tu-usuario.github.io/cmd-ps-errors)**

---

## Estructura del proyecto

```
cmd-ps-errors/
├── index.html    # App completa (HTML + CSS + JS en un solo archivo)
└── README.md
```

Sin dependencias, sin build steps, sin frameworks. Abre `index.html` y funciona.

---

## Cómo usar localmente

```bash
git clone https://github.com/tu-usuario/cmd-ps-errors.git
cd cmd-ps-errors
# Abre index.html en tu navegador
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```

---

## Deploy en GitHub Pages

1. Sube el repo a GitHub
2. Ve a **Settings → Pages**
3. En "Branch" selecciona `main` y carpeta `/ (root)`
4. Guarda — en unos minutos tendrás una URL pública

---

## Errores incluidos

| Código | Descripción | Shell |
|--------|-------------|-------|
| Error 5 | Acceso denegado | CMD + PS |
| Error 2 | Archivo no encontrado | CMD |
| No reconocido | Comando no reconocido | CMD |
| PSSecurityException | Scripts deshabilitados | PowerShell |
| Error 1603 | Fallo en instalación MSI | CMD + PS |
| TIMEOUT | Tiempo de espera agotado | CMD + PS |
| PSRemoting | No conecta al servidor remoto | PowerShell |
| Error 53 | Ruta de red no encontrada | CMD |
| OutOfMemory | Memoria insuficiente | PowerShell |
| Error 1722 | Servidor RPC no disponible | CMD + PS |
| NETHELPMSG 2221 | Usuario no existe | CMD |
| Get-ItemProperty error | Clave de registro no encontrada | PowerShell |

---

## Roadmap

- [ ] Agregar más errores (contribuciones bienvenidas)
- [ ] Buscador con IA integrada
- [ ] Modo claro / oscuro
- [ ] Exportar solución como `.bat` o `.ps1`

---

## Contribuir

¿Conoces un error que falta? ¡Añádelo!

1. Haz fork del repositorio
2. Añade tu error al array `errors` en `index.html`
3. Abre un Pull Request

Formato de cada error:
```javascript
{
  code: "Código del error",
  title: "Descripción corta",
  shell: "cmd" | "ps" | "both",
  cause: "Por qué ocurre este error.",
  steps: [
    { text: "Descripción del paso", cmd: "comando-a-ejecutar" }
  ]
}
```

---

## Licencia

MIT — úsalo, modifícalo y compártelo libremente.

