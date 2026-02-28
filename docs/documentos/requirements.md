# Requisitos – CapsulePOS

## Link al tablero Jira

https://miumg-team-dqo5nb5b.atlassian.net/jira/software/projects/SCRUM/boards/1

> Nota: El tablero Jira requiere acceso institucional.
> Todas las historias, prioridades y flujo del tablero se muestran en el video adjunto.

---

## Historias de Usuario

1. US-01 – Inicio de sesión por roles (Must)
2. US-02 – Registrar venta (Must)
3. US-03 – Actualización automática de inventario (Must)
4. US-04 – Gestión de productos (Must)
5. US-05 – Reporte de ventas diarias (Should)
6. US-06 – Registro de entradas de inventario (Should)
7. US-07 – Gestión de clientes (Could)
8. US-08 – Módulo de promociones (Won’t)

---

## Historias Must con Given / When / Then

### US-01

Given que el usuario ingresa credenciales válidas  
When presiona iniciar sesión  
Then el sistema permite acceso según su rol  

Given que el usuario ingresa credenciales incorrectas  
When intenta iniciar sesión  
Then el sistema muestra mensaje de error  

---

### US-02

Given que el cajero selecciona productos con stock disponible  
When confirma la venta  
Then el sistema calcula el total correctamente  

Given que un producto no tiene stock  
When intenta agregarlo  
Then el sistema muestra alerta  

---

## MVP Rationale

El MVP incluye login, registro de ventas, actualización automática de inventario y gestión de productos,
ya que son las funcionalidades esenciales para que el punto de venta pueda operar.
Sin estas funcionalidades el negocio no puede vender ni controlar su inventario.
Las demás historias agregan valor pero no son críticas para la operación inicial.
