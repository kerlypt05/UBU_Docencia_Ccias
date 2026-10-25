# Material de clase · Panificación y Pastelería (9057) · Universidad de Burgos

Simuladores de apoyo a las clases teóricas de **Panificación y Pastelería (9057)**, Grado en Ciencias Gastronómicas.

Prof. Kerly Palacios · Departamento de Biotecnología y Ciencias de los Alimentos

**Acceso:** https://kerlypt05.github.io/UBU_Docencia_Ccias/ · las páginas piden una clave común, que se publica en UBUVirtual.

| Recurso | Clase | Carpeta |
|---|---|---|
| Simulación 1 · Proceso de elaboración de bizcocho (espuma batida) | Clase C2 · Bloque 2 | `c2-espumas/` |
| Simulación 2 · Ladrillos y mortero | Clase C2 · Bloque 2 | `c2-ladrillos-mortero/` |

Las herramientas de las prácticas (PR-3: análisis de la miga y simulador de contraste) están en otro espacio, con su propia clave: https://kerlypt05.github.io/UBU_Practicas_Cccias/ · Las carpetas `pr3-miga/` y `pr3-espumas/` de este repositorio solo redirigen allí.

## Organización

- Cada recurso tiene su carpeta, con una página de acceso (`index.html`) y `simulador.html`.
- `assets/logo_ubu.png`: logo de la Universidad de Burgos que muestran las páginas.
- Las páginas están **cifradas** (AES-256-GCM con clave derivada por PBKDF2). Sin la clave no se pueden leer ni en la web ni en este repositorio. Las fuentes en claro se conservan fuera del repositorio.
- `herramientas/cifrar_paginas.py` cifra las páginas; se usa también para cambiar la clave de curso.

En este repositorio solo se publica material para estudiantes.

## Versiones

Cada recurso se versiona por separado; la versión vigente figura en su página de acceso.

## Mantenimiento

Las páginas se generan y se cifran a partir de una carpeta de fuentes en claro que **no** está en este repositorio.

- **Cifrar o cambiar la clave:** `python3 herramientas/cifrar_paginas.py --fuentes CARPETA_FUENTES/docencia --salida . --clave "CLAVE"` y subir los `.html` cambiados. La clave no se guarda en ningún archivo: se escribe en ese comando.
- **Actualizar un simulador:** sustituir su `simulador.html` en `CARPETA_FUENTES/docencia/` y volver a cifrar. Para cambiar textos de las páginas de acceso, editar `_generar_paginas.py` y ejecutarlo.

Requisito: Python 3 con `pip install cryptography`.
