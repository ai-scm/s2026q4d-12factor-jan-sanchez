# s2026q4d-12factor-jan-sanchez

Repositorio de estudio y práctica sobre la metodología **The Twelve-Factor App**, enfocado en los factores que considero más relevantes para el desarrollo y despliegue de aplicaciones modernas.

El análisis completo de cada factor se encuentra en [12Factor.md](./12Factor.md).

## ¿De qué trata este repositorio?

Este proyecto explora cómo aplicar los principios *Twelve Factor* para construir aplicaciones escalables, mantenibles y fáciles de desplegar. A continuación, un resumen de los factores que considero más importantes:

### 1. Dependencias
Evitar instalar dependencias directamente en la máquina local previene conflictos de versiones y facilita el despliegue. Aquí **Docker** juega un papel clave: permite encapsular todas las dependencias en un entorno controlado y reproducible en distintas máquinas mediante contenedores.

### 2. Configuración
Manejar la configuración mediante **variables de entorno** es crucial: evita exponer credenciales en el código, centraliza los cambios en un único punto y facilita la adopción de **Infraestructura como Código (IaC)** al poder modificar estas variables de forma sencilla.

### 3. Backing services
Tratar servicios externos (bases de datos, colas, etc.) como recursos intercambiables reduce el acoplamiento de la aplicación. Este principio está muy relacionado con **Clean Architecture**, ya que permite sustituir estos servicios sin tener que alterar significativamente la aplicación.

### 4. Igualdad entre desarrollo y producción
Desarrollo y producción deberían utilizar tecnologías y entornos muy similares para evitar incompatibilidades que retrasen el despliegue. El uso de **contenedores** ayuda a reducir esta brecha y acorta los tiempos de despliegue.

## Objetivo

El objetivo de este repositorio es servir como punto de partida para investigar y poner en práctica estos factores, priorizando la reproducibilidad, la seguridad y la independencia de la aplicación respecto a su entorno.
