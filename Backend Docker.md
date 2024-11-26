# informeBack
**Informe BackDocker**

(Esto es solo un resumen basado en mis practicas)

**2. Fundamentos**
Docker es una plataforma de contenedorización que permite empaquetar aplicaciones y sus dependencias en contenedores ligeros y portátiles. En el backend, su uso facilita la escalabilidad, despliegue, y gestión de aplicaciones, ofreciendo un entorno consistente entre desarrollo, pruebas y producción.

Los contenedores son aislados y reproducibles, asegurando que la aplicación funcione de la misma forma independientemente del entorno en el que se ejecute.

**3. Conocimientos previos**

.Conceptos básicos de Docker: imágenes, contenedores, volúmenes y redes.

.Backend: Familiaridad con frameworks como Spring Boot, Node.js.

.Sistemas Operativos: Uso de terminales en sistemas Linux/Unix.

.Bases de Datos: Configuración y manejo de MySQL, PostgreSQL u otras bases de datos populares.

.Docker Compose: Para orquestar múltiples contenedores.

.Control de versiones: Uso básico de Git para el manejo del código fuente.

**4. Objetivos a alcanzar**

.Contenerizar un backend utilizando Docker.

.Facilitar el despliegue y escalabilidad del backend.

.Asegurar la consistencia del entorno entre desarrollo y producción.

.Configurar un sistema de persistencia para bases de datos utilizando volúmenes.

.Implementar buenas prácticas para la creación de imágenes Docker.

**5. Equipo necesario**

.Docker y Docker Compose instalados.

.Un IDE o editor de texto como IntelliJ IDEA, VS Code o similar.

.Sistema operativo compatible: Linux, macOS, o Windows con WSL2.

.Backend preexistente en cualquier lenguaje soportado (Java, Python, Node.js).

**6. Material de apoyo**

.Documentación oficial de Docker

.Tutoriales específicos para backend con el framework seleccionado (e.g., Spring Boot, Django).

.Guías de uso de Docker Compose.

**7. Procedimiento**

En el backend se debe de agregar un archivo dockerfile en la raiz del proyecto en el cual se debe de agregar lo siguiente: 

![image](https://github.com/user-attachments/assets/060a65ea-55bc-43bb-a8ec-af4fd925d680)

que ara que cree un archivo.jar que se llamara igual que el proyecto pero estara ubicado en la carpeta target.

Una vez creado ese archivo del dockerfile, debemos abrir una terminal de linux, debemos entrar a donde esta el archivo y para entrar debemos usar lo siguiente 

![image](https://github.com/user-attachments/assets/9f2e7e74-c016-4568-b33d-1146b95950b6)

usando mnt es para entrar al directorio del disco duro de windows(si es que el poyecto esta ahi) para entrar al proyecto, una vez que se haya ingresado se debe crear un docker-compose.yml con el siguiente 
codigo: 

![image](https://github.com/user-attachments/assets/8a61505b-61ba-4f1e-9e9b-abc4fefde7c1)

es algo similar al frontd solo se cambia el nombre del proyecto

Aplicamos el siguiente comando para que el docker inicialize el proyecto: docker compose build y docker compose up -d y con esto hara que el proyecto se cree para luego iniciarlo con docker.

**8. Resultados esperados**

-Un contenedor funcional del backend con sus dependencias configuradas.

-Backend listo para desplegar en entornos locales o en la nube.

-Facilidad para replicar el entorno en nuevos desarrolladores o servidores.

**9. Bibliografia**

-Docker Inc. (n.d.). Docker Documentation. Retrieved from https://docs.docker.com/

-Turnbull, J. (2014). The Docker Book: Containerization is the new virtualization.

-Medium & Dev.to articles: Optimizing Docker for Backend Development.

