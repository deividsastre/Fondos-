<div align="center" style="text-align: justify;">

# Escaneo de Aplicaciones Web con Burp Suite

## 📌 Objetivo

Documentar el proceso de escaneo de una aplicación web utilizando **Burp Suite**, enfocado en pruebas de seguridad (pentesting) y análisis de tráfico **HTTP/HTTPS**.

---

## ⚙️ Configuración Inicial

### 1. Inicio de Burp Suite

Abrimos **Burp Suite**, previamente instalado en nuestra estación de trabajo.  
Al iniciar, Burp mostrará su panel principal con los módulos disponibles.

![Inicio de Burp Suite](images/Imagen2324.png)

---

### 2. Configuración del Proxy

Nos dirigimos a:

```text
Proxy → Proxy Settings
```

![Proxy Settings](images/Imagen2325.png)

Configuramos el proxy para que escuche en el **puerto 8080** y apunte a **localhost**, ya que el escaneo se realiza desde el mismo equipo.

![Configuración del puerto](images/Imagen2326.png)

Ejemplo de configuración:

```text
IP: 127.0.0.1
Puerto: 8080
```

---

### 3. Instalación del Certificado CA

Accedemos a la IP y puerto del proxy configurado desde el navegador y damos clic en **CA Certificate** para descargar el certificado.

![Descarga del certificado CA](images/Imagen2327.png)

Luego, ingresamos a la configuración del navegador y cargamos el certificado en el apartado de **administración de certificados**.

![Instalación del certificado](images/Imagen2328.png)

> ⚠️ **Nota:**  
> Este procedimiento se debe hacer para el corecto funcionamiento.

---

### 4. Visualización del Tráfico HTTP

En Burp Suite seleccionamos:

```text
Proxy → HTTP history
```

Aquí se visualizarán todas las solicitudes realizadas desde el navegador.

![HTTP History](images/Imagen2329.png)

---

### 5. Navegación de la Aplicación Web

Desde el navegador con el certificado instalado, accedemos a la aplicación web objetivo y realizamos una navegación completa por todas sus secciones.

![Navegación de la aplicación](images/Imagen2330.png)

---

### 6. Configuración del Scope y Escaneo

Definimos el alcance del escaneo en:

```text
Target → Lattitude.la → Add scope
```

![Agregar Scope](images/Imagen2331.png)

Luego iniciamos el escaneo desde:

```text
Lattitude.la → Scan
```

![Inicio del Scan](images/Imagen2332.png)

Configuramos el escaneo según los parámetros requeridos.

![Configuración del Scan](images/Imagen2333.png)

---

### 7. Monitoreo del Escaneo

El estado del escaneo puede visualizarse en el **Dashboard** de Burp Suite.

![Dashboard del Scan](images/Imagen2334.png)

---

### 8. Exportación de Resultados

Una vez finalizado el escaneo, seleccionamos los **Issues** detectados.

![Selección de Issues](images/Imagen2335.png)

Exportamos los resultados en formato **XML**.

![Exportación XML](images/Imagen2336.png)


Exportamos los resultados en formato **XML**, listo para ser cargado en **Eudora**.
![Exportación XML](images/Imagen2337.png)


</div>
