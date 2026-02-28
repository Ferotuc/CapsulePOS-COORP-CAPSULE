# System Brief – CapsulePOS

## Problema

COORP CAPSULE vende accesorios de computadoras.
Actualmente no existe un sistema automatizado para gestionar ventas e inventario,
lo que provoca errores de stock, lentitud en caja y falta de reportes claros.

## Stakeholders

- Cajero
- Administrador
- Encargado de bodega
- Gerente
- Cliente final

## Scope

- Login por roles
- Registro de ventas
- Actualización automática de inventario
- Gestión de productos
- Reportes básicos de ventas

## No-Scope

- Tienda en línea
- Integración contable externa
- Multi-sucursal
- Sistema avanzado de promociones

---

## Diagrama de Contexto

```mermaid
flowchart LR
Cliente --> Cajero
Cajero --> CapsulePOS
Administrador --> CapsulePOS
Bodega --> CapsulePOS
CapsulePOS --> BaseDeDatos
CapsulePOS --> Cliente
