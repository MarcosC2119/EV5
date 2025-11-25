# Evaluación Nº5 - Desarrollo de Aplicaciones Móviles

Este repositorio contiene el desarrollo de la Evaluación Nº5 para la asignatura de Desarrollo de Aplicaciones Móviles con Python y Kivy.

## 📋 Descripción del Proyecto
El proyecto consiste en una aplicación móvil desarrollada con **Kivy** que implementa un sistema de métricas para registrar la interacción del usuario y el tiempo de uso. Además, está configurada para ser empaquetada como APK para Android utilizando **Buildozer**.

## 🚀 Funcionalidades
1.  **Contador de Eventos**: Registra cada vez que el usuario realiza una acción clave (presionar botón).
2.  **Timer de Sesión**: Muestra en tiempo real cuánto tiempo lleva abierta la aplicación.
3.  **Sistema de Logs**: Genera un archivo `app_metrics.log` con datos detallados para análisis posterior.

## 📊 Métricas Implementadas
El sistema registra automáticamente las siguientes métricas en el archivo de log:

### 1. Interacción de Usuario (Eventos)
- **Qué mide**: Frecuencia de uso del botón principal.
- **Formato Log**: `EVENTO: Usuario interactuó con botón. Total eventos: X`
- **Utilidad**: Permite analizar el nivel de "engagement" o actividad dentro de la app.

### 2. Duración de Sesión
- **Qué mide**: Tiempo total desde que se abre hasta que se cierra la app.
- **Formato Log**: 
    - Inicio: `SESION: Inicio de actividad en aplicación`
    - Fin: `SESION: Cierre de aplicación. Tiempo activo: X segundos`
- **Utilidad**: Fundamental para entender los patrones de uso y retención.

## 🛠️ Instalación y Ejecución

### Requisitos
- Python 3.7+
- Kivy (`pip install kivy`)

### Ejecución Local
```bash
python main.py
```

### Compilación APK (Android)
Este proyecto incluye el archivo `buildozer.spec` listo para compilar.
1.  Entorno Linux/WSL requerido.
2.  Instalar Buildozer: `pip install buildozer`
3.  Ejecutar:
    ```bash
    buildozer android debug
    ```
4.  El APK se generará en la carpeta `bin/`.

## 📂 Estructura del Repositorio
- `main.py`: Código fuente principal.
- `buildozer.spec`: Configuración para empaquetado Android.
- `app_metrics.log`: Archivo de ejemplo con métricas registradas.
- `documentacion/`: Contiene el informe PDF de la evaluación.

## 📝 Autor
Evaluación presentada para la asignatura de Desarrollo de Aplicaciones Móviles.
