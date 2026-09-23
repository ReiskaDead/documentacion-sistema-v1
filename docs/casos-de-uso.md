# Documentación de Arquitectura: Casos de Uso

## 1.Descripción del Módulo
El presente doocumento define los requisitos funcionales del **Sistema de Gestión Hospitalaria**. Se detalla la interacción entre los actores (Paciente, Médico, Administrador) y las funcionalidades del sistema.

## 2. Diagrama UML de Casos  de Uso
![Diagrama de Casos de Uso Hospitalario](assets/casos_de_uso.png)

## 3. Especificación de Relaciones 
* **Relaciones <<inclede>>:** *Reservar Cita* y *Generar Factura* requieren obligatoriamente la autenticación previa del usuario en el sistema.
* **Relaaciones <<extend>>:** *Aplicar Descuento de Seguro* se ejecuta únicamente si la factura generada cuenta con cobertura médita.
  