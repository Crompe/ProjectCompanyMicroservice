# ProjectCompanyMicroservice
Proyecto realizado con el fin de practicar la estructura de Software basada en Microservicios. Este proyecto simula el flujo empresarial de una empresa, donde se gestiona a clientes, empleados, administradores, productos, inventario y sus compras. 
Cada microservicio a excepción de EurekaServer y ApiGateway, cuenta con su propia base datos, permitiendo así, la independencia total de cada uno de estos, pero siempre manteniendo la comunicación oportuna entre ellos. Esto también nos brinda mayor escalabilidad a la hora de extensiones o mejoras en cada uno, como también, nos brinda mayor seguridad. 
El servicio de AuthService, está programado para que la seguridad se centralice en el: este es quien acumula a los usuarios sin importar el rol, les da un token y les permite loguearse, dependiendo de su rol, tienen acceso a ciertos endpoints o no. 
Todos los microservicios se comunican por medio de Feign. 

# Microservicios del Sistema

| Servicio              | Descripción                                          | Repositorio |
|--------------------   |------------------------------------------------------|-------------|
| *Eureka Server*       | Descubrimiento de servicios                          | https://github.com/Crompe/EurekaService.git
| *API Gateway*         | Enrutamiento y gestión de rutas hacia servicios      | https://github.com/Crompe/ApiGateway.git
| *Auth Service*        | Gestión de usuarios, autenticación y seguridad       | https://github.com/Crompe/AuthService.git
| *Client Service*      | Gestión y CRUD de clientes                           | https://github.com/Crompe/ClientService.git
| *Product Service*     | Gestión de productos                                 | https://github.com/Crompe/ProductService.git
| *Inventory Service*   | Control de inventario y stock                        | https://github.com/Crompe/InventoryService.git
| *Order Service*       | Creación y administración de órdenes de compra       | https://github.com/Crompe/OrderService.git
| *Employee Service*    | Gestión de empleados                                 | https://github.com/Crompe/EmployeeService.git


# Todos los microservicios están implementados como proyectos independientes y son gestionados como mudulos en este proyecto principal. 

# Tecnologías útilizadas: 

*Java 17
*Spring Boot 3
*Spring Cloud
*Eureka Discovery Server
*Spring Security + JWT
*Maven
*Docker (en proceso)
*JUnit + Mockito (pruebas en proceso)

# Estado del Proyecto

 *Estructura modular terminada: Tarea culminada.

 *Repositorios separados para cada microservicio: Tarea Culminada

 *Dockerización de servicios: En proceso

 *Pruebas unitarias y de integración: En proceso

 *Documentación Swagger por microservicio: En proceso

# Autor: Diana Marcela Carvajal Losada. Estudiante de Ingeniería de Sistemas. Septimo semestre en curso. 
