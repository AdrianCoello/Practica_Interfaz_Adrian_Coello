# Práctica de Interfaces

Este repositorio contiene la implementación de una serie de ejercicios prácticos que exploran el uso de interfaces en Java. Cada ejercicio simula un escenario del mundo real, donde se aplican conceptos de programación orientada a objetos (POO) y diseño de interfaces.

## Escenarios y Requerimientos

### 1. Plataforma de Streaming de Contenidos
- **Interfaz:** `Reproducible` con métodos `reproducir()`, `pausar()` y `detener()`.
- **Clases:** `Pelicula`, `Serie`, `Documental`.
- **Atributos específicos:** Duración en `Pelicula`, cantidad de episodios en `Serie`, tema en `Documental`.
- **Clase Usuario:** Puede agregar contenido a su lista de favoritos y reproducirlo.

### 2. Sistema de Gestión de Pedidos para un Restaurante
- **Interfaz:** `Pedido` con métodos `preparar()`, `entregar()`.
- **Clases:** `PedidoParaLlevar`, `PedidoEnMesa`, `PedidoDomicilio`.
- **Interfaz Repartidor:** Implementada por `Motorizado` y `Ciclista`.
- **Clase Restaurante:** Gestiona pedidos y asigna repartidores.

### 3. Red Social con Interacciones
- **Interfaz:** `Interactuable` con métodos `comentar(String comentario)`, `reaccionar(String tipoReaccion)`, `compartir()`.
- **Clases:** `Foto`, `Video`, `Articulo`.
- **Clase Usuario:** Puede realizar interacciones con las publicaciones.

### 4. Sistema de Pago y Facturación para una Empresa
- **Interfaz:** `MetodoPago` con método `procesarPago(double monto)`.
- **Clases:** `TarjetaCredito`, `PayPal`, `TransferenciaBancaria`.
- **Interfaz Facturable:** Implementada por `FacturaElectronica` y `FacturaFisica`.
- **Clase Compra:** Usa ambas interfaces (`MetodoPago` y `Facturable`).

### 5. Plataforma de Aprendizaje Online
- **Interfaz:** `Curso` con métodos `iniciar()`, `completar()`.
- **Clases:** `CursoVideo`, `CursoPDF`, `CursoExamen`.
- **Interfaz Evaluable:** Implementada en `CursoExamen` con método `calificar(int puntaje)`.
- **Clase Estudiante:** Puede inscribirse y completar cursos.

### 6. Plataforma de Transporte Urbano
- **Interfaz:** `TransportePublico` con métodos `iniciarViaje(String origen, String destino)`, `calcularTarifa()`.
- **Clases:** `Taxi`, `Bus`, `BicicletaCompartida`.
- **Interfaz Conductor:** Implementada en `Taxi`.
- **Clase Usuario:** Puede solicitar un viaje.

### 7. Sistema de Inventario para un Almacén
- **Interfaz:** `Producto` con métodos `obtenerPrecio()`, `obtenerStock()`.
- **Clases:** `Electronico`, `Alimento`, `Ropa`.
- **Interfaz Almacenable:** Implementada en `Alimento` con verificación de fecha de caducidad.
- **Clase Inventario:** Gestiona los productos.

### 8. Sistema de Gestión de Empleados en una Empresa
- **Interfaz:** `Empleado` con métodos `calcularSalario()`, `obtenerCargo()`.
- **Clases:** `Administrativo`, `Tecnico`, `Gerente`.
- **Interfaz Bonificable:** Implementada en `Gerente`.
- **Clase Empresa:** Administra empleados.

### 9. Sistema de Recomendaciones de Productos
- **Interfaz:** `Recomendable` con método `obtenerRecomendaciones()`.
- **Clases:** `UsuarioPremium`, `UsuarioRegular`.
- **Clase Producto:** Atributos `nombre`, `categoria`, `precio`.
- **Clase SistemaRecomendaciones:** Sugiere productos.

### 10. Plataforma de Reservas de Hoteles
- **Interfaz:** `Reservable` con métodos `reservar(String fecha)`, `cancelarReserva()`.
- **Clases:** `Hotel`, `Departamento`, `CasaVacacional`.
- **Interfaz Calificable:** Implementada en `Hotel`.
- **Clase Usuario:** Puede hacer y cancelar reservas.


## Cómo Ejecutar el Proyecto

1. Clona este repositorio en tu máquina local.
2. Abre el proyecto en tu IDE favorito (Eclipse, IntelliJ, etc.).
3. Navega a la clase principal de cada escenario para ejecutar y probar la implementación.

## Contribuciones

Si deseas contribuir a este proyecto, por favor sigue los siguientes pasos:

1. Haz un fork del repositorio.
2. Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`).
3. Realiza tus cambios y haz commit (`git commit -m 'Añade nueva funcionalidad'`).
4. Haz push a la rama (`git push origin feature/nueva-funcionalidad`).
5. Abre un Pull Request.

---

¡Gracias por visitar este repositorio! Si tienes alguna pregunta o sugerencia, no dudes en abrir un issue o contactarme directamente.
