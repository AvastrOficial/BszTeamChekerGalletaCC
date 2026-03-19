# BszTeamChekerGalletaCC

## 📋 Descripción

**BszTeamChekerGalletaCC** es una herramienta de verificación de tarjetas de crédito diseñada para sitios web que utilizan **WooCommerce** con **Braintree** como pasarela de pago.

El script automatiza el proceso de agregar métodos de pago en la sección **"Mi Cuenta"**, permitiendo validar tarjetas de forma automatizada.

---

## ⚠️ ADVERTENCIA LEGAL

> 🚫 Esta herramienta es solo para fines **educativos y de prueba en tus propios sitios**.
> El uso no autorizado para verificar tarjetas de crédito sin permiso explícito es **ilegal** y puede constituir **fraude**.

---

## 🚀 Características

| Función                  | Descripción                          |
| ------------------------ | ------------------------------------ |
| ✅ Verificación Braintree | Automatiza validación de tarjetas    |
| 🍪 Gestión de cookies    | Múltiples cookies por dominio        |
| 🔢 Selección numerada    | Fácil manejo de cookies              |
| ✏️ Edición de datos      | Editar y eliminar cookies            |
| 🌐 Gestión de webs       | Control total de dominios            |
| 🟢 Detección LIVE        | CVV incorrecto detectado como válido |
| ⏱️ Anti detección        | Espera de 15 segundos                |
| 🎨 Interfaz ANSI         | Colores en consola                   |
| 🔐 Validación sesión     | Verifica login antes de usar         |

---

## 📦 Requisitos

* Python **3.6 o superior**
* Librerías:

  * `requests`
  * `urllib3`

---

## 🔧 Instalación

```bash id="instalacion1"
git clone https://github.com/AvastrOficial/BszTeamChekerGalletaCC.git
cd BszTeamChekerGalletaCC
```

```bash id="instalacion2"
pip install requests urllib3
```

```bash id="instalacion3"
python checkerBsz.py
```

---

## 📁 Estructura de Archivos

| Archivo           | Descripción         |
| ----------------- | ------------------- |
| `webs.txt`        | Lista de dominios   |
| `cookies.txt`     | Cookies por dominio |
| `current_web.txt` | Web seleccionada    |

---

## 🎯 Cómo Funciona

### 1️⃣ Gestión de Cookies

| Opción | Acción             |
| ------ | ------------------ |
| A      | Agregar cookie     |
| S      | Seleccionar cookie |
| E      | Editar cookie      |
| D      | Eliminar cookie    |
| V      | Volver             |

---

### 2️⃣ Gestión de Webs

| Opción | Acción          |
| ------ | --------------- |
| A      | Agregar dominio |
| S      | Seleccionar web |
| E      | Editar dominio  |
| D      | Eliminar web    |
| V      | Volver          |

---

### 3️⃣ RUN CHECKER

* Verifica compatibilidad (**WooCommerce + Braintree**)
* Valida cookies
* Doble confirmación de seguridad
* Entrada de tarjetas:

```text id="formato1"
CC|MM|YYYY|CVV
```

* Espera de **15 segundos** entre verificaciones

---

## 📊 Resultados

| Estado      | Significado                     |
| ----------- | ------------------------------- |
| 🟢 LIVE     | Tarjeta válida o CVV incorrecto |
| 🔴 DECLINED | Tarjeta rechazada               |
| 🟡 ERROR    | Fallo en verificación           |

---

## 🔍 Ejemplo de Uso

```bash id="ejemplo1"
============================================================
              MENÚ PRINCIPAL
============================================================
🌐 Web actual: uavionix.com
📁 Cookies guardadas: 2
------------------------------------------------------------
[1] Gestionar Cookies
[2] Gestionar Webs
[3] RUN CHECKER
[4] Salir
============================================================

Selecciona una opción >>> 3
```

---

## 📝 Formato de Cookies

```text id="cookies1"
nombre1=valor1; nombre2=valor2; nombre3=valor3
```

### Ejemplo:

```text id="cookies2"
PHPSESSID=abc123; wordpress_logged_in=user|time|hash; wp-settings-time=123456
```

---

## 🛠️ Sitios Compatibles

| Requisito                              | Estado |
| -------------------------------------- | ------ |
| WooCommerce                            | ✔️     |
| Braintree                              | ✔️     |
| Ruta `/my-account/add-payment-method/` | ✔️     |
| Sesión iniciada                        | ✔️     |

---

## ⚙️ Configuración

Puedes modificar en el código:

| Configuración       | Ubicación     |
| ------------------- | ------------- |
| ⏱️ Tiempo de espera | Línea 868     |
| 🌐 User-Agent       | Línea 686     |
| 🎨 Colores          | Clase `Color` |

---

## 🤝 Contribuciones

1. Haz un **fork**
2. Crea tu rama:

```bash id="git1"
git checkout -b feature/AmazingFeature
```

3. Haz commit:

```bash id="git2"
git commit -m "Add some AmazingFeature"
```

4. Sube cambios:

```bash id="git3"
git push origin feature/AmazingFeature
```

5. Abre un **Pull Request**

---

## ⭐ Soporte

Si te sirve este proyecto:

* ⭐ Dale estrella
* 📢 Compártelo
* 🤝 Contribuye

