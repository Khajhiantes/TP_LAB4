# **Sistema de Gestión Escolar en Laravel**

![banner](https://github.com/user-attachments/assets/99aaaf56-729e-4620-b3b3-0a7e22f96121)

Este proyecto es una aplicación desarrollada en Laravel para gestionar estudiantes, cursos, profesores, materias y comisiones.

## Integrantes:
- RUBIN AZAS M. Luis (legajo: `26472`)
- ZAMORA Martín (legajo: `20660`)

---

## **Requisitos Previos**
Antes de iniciar, asegúrate de tener instalados los siguientes programas en tu PC:

- [Composer](https://getcomposer.org/)
- [XAMPP](https://www.apachefriends.org/index.html) (o cualquier servidor que incluya MySQL y PHP)

---

## **Pasos para Configurar el Proyecto**

### **1. Clonar el Repositorio abriendo el símbolo del sistema y pegar el siguiente código**
Clona este repositorio en tu máquina local:
```bash
git clone https://github.com/louisrubin/TP_LAB4
```
### **2. Accede a la carpeta del proyecto**
```bash
cd lab4Calculo2024
```
Es aquí desde donde se ejecutan todos los demás puntos.

### **3. Configurar el Archivo `.env`**
```bash
cp .env.example .env
```
Esto crea una copia del archivo de configuración de ejemplo para configurarlo en tu entorno local.

Luego, edita el archivo `.env` con los datos de conexión a tu base de datos. Por ejemplo:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=nombre_de_tu_bd
DB_USERNAME=tu_usuario
DB_PASSWORD=tu_contraseña
```

### **4. Generar la Clave de la Aplicación**
```bash
php artisan key:generate
```
Esto genera y configura una clave de cifrado única para proteger datos sensibles.

### **5. Crear la Base de Datos**
Asegúrate de haber creado una base de datos con el mismo nombre que especificaste en `DB_DATABASE` del archivo `.env`.

### **6. Ejecutar Migraciones y Seeders**
```bash
php artisan migrate --seed
```

### **7. Iniciar el Servidor de Desarrollo**
```bash
php artisan serve
```

Esto levantará el servidor en http://localhost:8000.

### **8. Ejecutar Apache y MySQL**
Abre XAMPP y asegúrate de que los servicios de Apache y MySQL estén corriendo

![Captura](https://github.com/user-attachments/assets/e073cded-74cc-45ce-a335-269b3c681b5c)
