# Introducción y Objetivos

## Objetivo del sistema

El presente documento describe la arquitectura de software del **Sistema ERP**, una plataforma diseñada para gestionar los procesos de negocio de una empresa, incluyendo compras, facturación, inventario, activos fijos, gestión de empleados y reportes ejecutivos (EIS).

Este documento se enfoca específicamente en el **Módulo de Compras**, el cual permite a los gestores de inventario y compras administrar productos, proveedores y órdenes de compra de manera centralizada.

## Requisitos de negocio más importantes (Módulo de Compras)

1. El sistema debe permitir registrar y mantener un catálogo actualizado de productos.
2. El sistema debe permitir registrar proveedores y asociarlos a los productos que ofrecen, incluyendo su precio unitario.
3. El sistema debe permitir crear órdenes de compra seleccionando productos y proveedores.
4. El sistema debe permitir consultar el historial de órdenes de compra realizadas para hacer seguimiento a los pedidos.
5. El sistema debe garantizar la integridad de los datos, validando la información obligatoria antes de guardar cualquier registro.

## Stakeholders principales

| Rol | Interés |
|---|---|
| Gestor de Compras | Administrar proveedores y órdenes de compra |
| Gestor de Inventario | Mantener el catálogo de productos actualizado |
| Administrador del Sistema | Garantizar el correcto funcionamiento de la plataforma |
