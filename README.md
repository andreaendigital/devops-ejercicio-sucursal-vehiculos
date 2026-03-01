# Pipeline CI/CD: Validación y Despliegue Automatizado en AWS

Este proyecto consiste en la implementación de un ecosistema de Integración y Entrega Continua (CI/CD) utilizando **Jenkins** sobre una instancia **AWS EC2**. El objetivo es automatizar el ciclo de vida de una aplicación **Spring Boot**, desde el control de versiones en GitHub hasta su despliegue en un contenedor **Docker** con servidor **Tomcat**.

## ⚡ Tecnologías Utilizadas
* **Cloud:** AWS (EC2, Security Groups).
* **CI/CD:** Jenkins (Pipeline as Code, Webhooks).
* **Build Tool:** Maven.
* **Containerization:** Docker & Tomcat.
* **Backend:** Java Spring Boot.
* **Documentación:** Swagger & Postman.

## 🛠️ Proceso de Implementación

1.  **Infraestructura:** Provisión de una instancia EC2 (Ubuntu) con configuración de puertos (8080 para Jenkins, 9090 para Docker).
2.  **Configuración de Jenkins:** Instalación de dependencias y plugins necesarios (Maven, Git, Docker).
3.  **Integración con GitHub:** Configuración de Webhooks para disparar el Pipeline ante eventos de `push`.
4.  **Pipeline CI/CD:**
    * **Build:** Compilación del proyecto con Maven.
    * **Dockerize:** Creación de la imagen Docker de la aplicación.
    * **Deploy:** Ejecución del contenedor sobre Tomcat.
5.  **Validación:** Pruebas de endpoints mediante Swagger UI y tests de integración con Postman.

## 📹 Demostración
En este repositorio se incluye el enlace al video de presentación donde se evidencia el flujo completo del pipeline, la automatización por Webhook y el despliegue exitoso.
