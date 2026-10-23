# Docencia en Ciencias Gastronómicas · Universidad de Burgos

Simuladores y aplicativos para los estudiantes de **Panificación y Pastelería (9057)**, Grado en Ciencias Gastronómicas.

Prof. Kerly Palacios · Departamento de Biotecnología y Ciencias de los Alimentos

**Acceso:** https://kerlypt05.github.io/UBU_Docencia_Ccias/ · las páginas piden una clave común, que se publica en UBUVirtual.

| Recurso | Práctica o clase | Página |
|---|---|---|
| Simulador de batidos de espuma | PR-3 · Bizcochos de espuma | `pr3-espumas/` |
| Aplicativo de análisis de miga (Colab) | PR-3 · Bizcochos de espuma | `pr3-miga/` |
| Simulador de ladrillos y mortero | Clase C2 · Bloque 2 | `c2-ladrillos-mortero/` |

## Organización

- Cada recurso tiene su carpeta, con una página de acceso (`index.html`) y su contenido (`simulador.html` o `guia.html`).
- Las páginas están **cifradas** (AES-256-GCM con clave derivada por PBKDF2). Sin la clave no se pueden leer ni en la web ni en este repositorio. Las fuentes en claro se conservan fuera del repositorio.
- `herramientas/cifrar_paginas.py` cifra las páginas; se usa también para cambiar la clave de curso.
- El código del aplicativo de miga (`pr3-miga/aplicativo_analisis_alveolar_PR3.py`), su cuaderno de Colab y `version.json` quedan **abiertos**: el cuaderno los descarga desde aquí al ejecutarse.

En este repositorio solo se publica material para estudiantes.

## Versiones

Cada recurso se versiona por separado, con etiquetas que llevan su nombre (por ejemplo `pr3-miga-v1.0`). El historial del aplicativo de miga está en `pr3-miga/CHANGELOG.md`.
