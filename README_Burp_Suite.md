# Escaneo de Aplicaciones Web con Burp Suite

## 📌 Objetivo
Documentar el proceso de escaneo de una aplicación web utilizando Burp Suite, enfocado en pruebas de seguridad (pentesting) y análisis de tráfico HTTP/HTTPS.

## 🛠️ Herramientas
- Burp Suite Professional / Community
- Navegador web (Firefox o Chrome)
- Sistema operativo con permisos de instalación de certificados

## ⚙️ Configuración Inicial

### 1. Inicio de Burp Suite
Abrimos Burp Suite previamente instalado en nuestra estación de trabajo.

### 2. Configuración del Proxy
Ruta:
Proxy > Proxy Settings

- IP: 127.0.0.1
- Puerto: 8080

### 3. Instalación del Certificado CA
Accedemos a http://burp, descargamos el CA Certificate e instalamos el certificado en el navegador.

## 🌐 Navegación de la Aplicación Objetivo
Navegamos completamente la aplicación web para capturar todas las peticiones posibles.

## 📜 Análisis del Tráfico
Ruta:
HTTP history

## 🎯 Configuración del Scope y Escaneo
Ruta:
Target > Site map > Add to scope > Scan

## 📊 Monitoreo del Escaneo
Ruta:
Dashboard

## 🔐 Consideraciones de Seguridad
- Ejecutar escaneos solo con autorización
- No usar entornos productivos

## ✅ Conclusión
Burp Suite es una herramienta esencial para pruebas de seguridad en aplicaciones web.
