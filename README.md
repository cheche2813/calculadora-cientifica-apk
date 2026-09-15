# 🧮 Calculadora Científica (App Android)

Aplicación móvil de calculadora científica desarrollada para entornos Android, orientada a estudiantes y profesionales que requieren operaciones matemáticas avanzadas, trigonometría, funciones logarítmicas y álgebra de forma rápida y eficiente.

---

## 📋 Tabla de Contenidos
1. [Características Principales](#-características-principales)
2. [Arquitectura y Estructura de Recursos](#-arquitectura-y-estructura-de-recursos)
3. [Modelado Matemático y Funciones](#-modelado-matemático-y-funciones)
4. [Gestión de Excepciones](#-gestión-de-excepciones)
5. [Autor](#-autor)

---

## ✨ Características Principales

- **Modo Estándar y Científico:** Alterna fácilmente entre operaciones aritméticas básicas y funciones científicas avanzadas.
- **Trigonometría y Constantes:** Soporte completo para funciones trigonométricas ($\sin, \cos, 	an$, inversas) en grados y radianes, además de constantes matemáticas ($\pi, e$).
- **Funciones Exponenciales y Logarítmicas:** Cálculo de potencias ($y^x$), raíces cuadradas ($\sqrt{x}$), logaritmo natural ($\ln$) y logaritmo base 10 ($\log_{10}$).
- **Historial de Operaciones:** Registro temporal de consultas previas para reutilización de resultados.

---

## 📂 Arquitectura y Estructura de Recursos

El proyecto sigue los estándares de desarrollo nativo en Android, organizando los recursos visuales y de diseño de la siguiente manera:

| Directorio / Módulo | Descripción de Componentes | Propósito Técnico |
| :--- | :--- | :--- |
| `res/anim/` | Animaciones XML (`fade_in`, `slide_enter`, `zoom_enter`) | Transiciones fluidas entre paneles y respuesta táctil. |
| `res/drawable/` | Recursos gráficos vectoriales, selectores y fondos XML | Diseño de botones con estados táctiles interactivos. |
| `res/layout/` | Interfaces XML (`activity_main`, diálogos modales) | Disposición estructurada de la botonera científica y pantalla de display. |
| `res/mipmap/` | Iconos de la aplicación en múltiples resoluciones | Identidad visual adaptativa (`mdpi`, `hdpi`, `xhdpi`, `xxhdpi`, `xxxhdpi`). |

---

## 📐 Modelado Matemático y Funciones

Las expresiones matemáticas son evaluadas mediante un motor optimizado que soporta:

- **Trigonometría:** $\sin(	heta), \cos(	heta), 	an(	heta), rcsin(x), rccos(x), rctan(x)$
- **Exponenciales y Logaritmos:** $f(x) = e^x$, $\ln(x)$, $\log_{10}(x)$, $y^x$, $\sqrt{x}$
- **Operadores Auxiliares:** Factorial ($n!$), porcentajes y gestión de memoria aritmética ($M+, M-, MR, MC$).

---

## 🛡️ Gestión de Errores y Excepciones

El sistema cuenta con validaciones estrictas en tiempo de ejecución para evitar fallos críticos:
- **Indefinición aritmética:** $x / 0 
ightarrow$ `"Error: Indefinido"`
- **Dominios logarítmicos inválidos:** $\ln(x \le 0) 
ightarrow$ `"Error de Dominio"`
- **Desbordamiento numérico:** Control de límites por `Overflow / Underflow`.

---

## 👨‍💻 Autor

* **Desarrollador:** Luis Alejandro Florez Parra
* **Programa:** Análisis y Desarrollo de Software (ADSO)
* **Institución:** SENA CSET (Centro de Servicios Empresariales y Turísticos)
