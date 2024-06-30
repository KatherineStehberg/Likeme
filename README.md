Desafío 3 de Backend con Node y Express

Instrucciones:
Crear base de datos 'likeme':
Ejecutar el siguiente comando SQL para crear la base de datos:
sql

CREATE DATABASE likeme;


Crear la tabla 'posts':
Ejecutar el siguiente comando SQL para crear la tabla 'posts' dentro de la base de datos 'likeme':
sql

CREATE TABLE posts (
    id SERIAL PRIMARY KEY,
    titulo VARCHAR(25) NOT NULL,
    img VARCHAR(1000) NOT NULL,
    descripcion VARCHAR(255) NOT NULL,
    likes INT NOT NULL DEFAULT 0
);


Instalación de dependencias:
Ejecutar npm install en el directorio /backend y también en el directorio /frontend para instalar todas las dependencias necesarias.
Configuración de variables de entorno:
Crear un archivo .env en el directorio /backend y configurar las siguientes variables de entorno:
arduino

PORT=3000  // Corresponde al puerto del backend
PGHOST=localhost  // Corresponde al host de la DB
PGUSER=postgres  // Corresponde al usuario de la DB
PGPASSWORD=Vivachile28!  // Corresponde a la contraseña del usuario de la DB
PGDATABASE=likeme  // Corresponde a la base de datos a la que nos conectaremos
PGPORT=5432  // Corresponde al puerto habilitado para conectarse a la DB

Ejecución del proyecto:

Para iniciar el proyecto completo, ejecutar el comando npm run dev en el directorio /backend y también en el directorio /frontend. Esto levantará ambos servidores y luego podrás acceder a la URL del servidor de frontend en tu navegador.
Siguiendo estos pasos, tendrás configurada y lista la aplicación para ejecutarse correctamente con Node.js, Express, y la base de datos PostgreSQL.