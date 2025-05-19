
# 🖥️ ReparaTech - Subsistema de Gestión de Materiales

> _Sistema de gestión de materiales para el servicio técnico de reparaciones informáticas._

---

## 📑 Índice

- [🔧 Introducción](#-introducción)
- [📦 Funcionalidades del Subsistema](#-funcionalidades-del-subsistema)
  - [🗂️ Registro de materiales y repuestos](#️-registro-de-materiales-y-repuestos)
  - [📥 Gestión de stock](#-gestión-de-stock)
  - [🧾 Orden de compras](#-orden-de-compras)
  - [🛠️ Asignación de materiales](#️-asignación-de-materiales)
  - [🕓 Historial de materiales](#-historial-de-materiales)
- [📊 Estructura del Código Java](#-estructura-del-código-java)
- [🖼️ Galería de Imágenes](#️-galería-de-imágenes)
- [⚠️ Notificaciones y Alertas](#️-notificaciones-y-alertas)
- [👥 Integrantes del Grupo](#-integrantes-del-grupo)

---

## 🔧 Introducción

El **Subsistema de Gestión de Materiales** es una parte clave del sistema de reparaciones informáticas. Este módulo permite:

- 📦 Controlar el inventario de piezas y repuestos.
- 📋 Gestionar pedidos a proveedores.
- 🛠️ Asignar materiales a reparaciones concretas.
- ⚠️ Evitar quiebres de stock con alertas automáticas.

> 💡 _Este subsistema se integra con los módulos de personal, reparaciones, clientes e informes._

---

## 📦 Funcionalidades del Subsistema

### 🗂️ Registro de materiales y repuestos

Permite agregar nuevos ítems al inventario, incluyendo:

- Nombre del material
- Descripción
- Proveedor
- Precio unitario
- Cantidad

---

### 📥 Gestión de stock

- Control de entradas y salidas.
- Visualización de stock actual.
- Alerta de **stock bajo** cuando la cantidad llega al mínimo.
- Recuento automatizado.

---

### 🧾 Orden de compras

- Generación automática de pedidos a proveedores.
- Historial completo de órdenes emitidas.
- Asociaciones con proveedores registrados.

---

### 🛠️ Asignación de materiales

- Los materiales pueden asignarse a reparaciones específicas.
- Se registra cantidad usada, fecha y técnico responsable.

---

### 🕓 Historial de materiales

- Informes por período, reparación o cliente.
- Consulta del uso y coste acumulado por reparación.

---

## 📊 Estructura del Código Java

```java
public class Material {
    private String nombre;
    private int stock;
    private String proveedor;
    private double precio;

    public Material(String nombre, int stock, String proveedor, double precio) {
        this.nombre = nombre;
        this.stock = stock;
        this.proveedor = proveedor;
        this.precio = precio;
    }

    public void actualizarStock(int cantidad) {
        this.stock += cantidad;
    }

    public boolean esStockBajo() {
        return this.stock < 5;
    }

    // Getters y Setters...
}
```

---

## 🖼️ Galería de Imágenes

> *Visualización simulada del panel de stock del sistema:*

![Panel de gestión de materiales](https://via.placeholder.com/800x400?text=Gestión+de+Stock)

---

## ⚠️ Notificaciones y Alertas

> ✅ **NOTIFICACIÓN**: El nuevo repuesto *Memoria RAM 8GB* ha sido registrado correctamente.

> ⚠️ **ADVERTENCIA**: El stock de *Disco SSD 500GB* está por debajo del mínimo.

> ❌ **ERROR**: No se ha podido actualizar el stock debido a un fallo de conexión con la base de datos.

---

## 👥 Integrantes del Grupo

Este proyecto ha sido desarrollado por estudiantes del **1º DAW - IES Font de Sant Lluís**:

- 👤 Manuel Rubio
- 👤 Irma
- 👤 Ruben
- 👤 Alejandro

| Nombre     | Rol | Subsistema     |
|------------|------|------------|
| Manu   | Scrum   | Gestion de materiales     |
| Ruben      | 31   | Gestion de reparaciones  |
| Alejandro       | 29   | Gestion de clientes   |
| Irma      | 39   | Gestion de informes   |




🔗 [Volver al índice](#📑-índice)
