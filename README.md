# Anexo de Solicitud de Información para Soporte Técnico Ayuda en Ejercicios del Curso

**Estimado Usuario,**

Para poder ayudarle de la mejor manera con cualquier inconveniente que experimente en el desarrollo de los ejercicios de programación de este curso, le solicitamos que proporcione la siguiente información. Esto nos permitirá analizar el problema y brindarle una solución óptima.

Por favor, rellene los campos a continuación y adjunte cualquier archivo necesario:

---

## 1. Información del Sistema Operativo
- **Distribución**:  
  Indique la versión exacta de su sistema operativo, que debe cumplir con uno de los siguientes requisitos:
  - Ubuntu 22.04 o 24.04
  - Debian 12
- **Versión exacta del sistema operativo**:  
  - Ejemplo: `Ubuntu 24.04 LTS`, `Debian 12`, etc.

---

## 2. Especificaciones del Hardware
- **Cantidad de RAM**:  
  Asegúrese de que el sistema cuenta con al menos 4 GB de RAM.
- **Espacio en Disco Duro**:  
  Tamaño total disponible en el sistema: Idealmente entre 50 a 100 GB.
- **Procesador**:  
  Indique si es compatible con arquitectura AMD64 o Intel x64.

---

## 3. Versión de Odoo y Entorno
- **Versión de Odoo**:  
  Ejemplo: `Odoo 18`, `Odoo 17`.
- **Entorno de Ejecución**:  
  Docker o Script linux (especifique versión) o instalación directa en el sistema.
- **Versiones de Python y otras librerías**:
  - Versión exacta de Python utilizada en el entorno: Ejemplo `Python 3.11`.
  - Cualquier librería adicional relevante si tiene errores: Ejemplo, `psycopg2`, `Werkzeug`.

---

## 4. Descripción del Problema
- **Descripción detallada**: Explique los pasos seguidos antes de encontrar el error.
- **Mensajes de error**: Escriba el mensaje de error exacto si está visible.
- **Log de Errores**: Adjunte una imagen o archivo de texto con el log del error que aparece en la consola. Puede generar el archivo usando el siguiente comando, según su entorno:

  ```bash
  # Dentro de la carpeta de logs o desde la consola de odoo
  tail -n 100 /path/to/logfile.log > error_log.txt

  ```


  ### Comandos de ayuda Linux (ejecutar desde terminal)

    ```bash
  # sacar version del sistema linux
  cat /etc/os-release

  # ver si hay procesos activos de odoo
  ps aux |grep odoo-bin

  # eliminar limpiar procesos de odoo activos
  pkill -f odoo-bin
  
  # ver cantidad de ram y disco disponibles
  free -m
  df -h

  # reiniciar el servicio de odoo (instalacion desde script y en produccion)
  # ejemplo instalacion desde script en odoo 18
  sudo systemctl restart odoo18.service

  ```

