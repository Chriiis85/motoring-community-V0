# TFG DAW 2024 — Motoring Community (PHP & MySQL)

[Ver en Español](#-español) | [View in English](#-english)

> 🎓 **Trabajo de Fin de Grado** · Técnico Superior en Desarrollo de Aplicaciones Web (DAW)  
> 🏛️ **Centro:** I.E.S. Puig Adam (Getafe, Madrid) · **Año:** 2024  
> 🚀 **Evolución moderna (Next.js 16 + React 19):** [Motoring Community](https://github.com/Chriiis85/motoring-community) · [Demo](https://motoring-community-v1.vercel.app)

---

## 🇪🇸 Español

¡Hola! 👋 Soy **Christian**. Este repositorio contiene el código de mi **Trabajo de Fin de Grado (TFG)** con el que completé el grado superior de **DAW**.

Como aficionado a la Fórmula 1, quise desarrollar una **plataforma web completa** trabajando directamente con las tecnologías fundamentales de la web: **PHP**, **JavaScript**, **CSS3** y **MySQL**, sin recurrir a frameworks pesados.

Este proyecto fue el punto de partida y la base sobre la que más adelante construí [Motoring Community](https://github.com/Chriiis85/motoring-community) con Next.js y React. Toda la estructura de datos, las consultas a clasificaciones, los foros y la lógica de usuarios se idearon y probaron primero aquí.

### Qué incluye la plataforma

- **Foro y usuarios:** Sistema de registro e inicio de sesión, perfiles de usuario y publicación de hilos de debate para comentar los fines de semana de carreras (`forum.php`, `users.php`).
- **Calendario con cuenta atrás:** Fechas y horarios de cada Gran Premio de la temporada junto con los planos de los circuitos.
- **Clasificaciones en directo:** Tablas actualizadas del Mundial de Pilotos y Constructores con puntos y banderas.
- **Fichas de pilotos y escuderías:** Información técnica de los monoplazas, dorsales y biografías de los pilotos.
- **Accesibilidad web:** Navegación pensada para teclado (`tabindex`), estructura semántica limpia y contrastes cuidados para lectores de pantalla (WCAG 2.1).
- **Docker:** Configuración básica con Dockerfile y Docker Compose para levantar el entorno con Apache, PHP y MySQL en local en un par de minutos.

### Retos técnicos resueltos

1. **Estructura MVC en PHP nativo:**  
   Separé controladores, vistas modulares (`header.php`, `footer.php`, `calendar.php`) y consultas a base de datos de forma limpia para entender en profundidad el ciclo de vida de las peticiones HTTP y la gestión de sesiones.
2. **Modelado de base de datos en MySQL:**  
   Diseñé el esquema relacional (`BD_Motoring_Community.sql`) con claves foráneas e índices para relacionar usuarios, publicaciones del foro, comentarios y resultados deportivos de forma eficiente.
3. **Peticiones dinámicas con JavaScript:**  
   Implementé llamadas asíncronas para actualizar datos y resultados de competición sin necesidad de recargar la página completa.

### Tecnologías utilizadas

- **Backend:** PHP nativo (MVC, sesiones, PDO)
- **Base de Datos:** MySQL
- **Frontend:** HTML5 semántico, CSS3 (Flexbox y Grid), JavaScript (ES6+)
- **Entorno:** Docker, Apache, `.htaccess`
- **Accesibilidad:** Criterios WCAG 2.1 / WAI-ARIA

### Cómo probarlo en local

#### Opción A: Con Docker (Recomendado)
```bash
# 1. Clonar el repositorio
git clone https://github.com/Chriiis85/TFG-DAW-2024.git
cd TFG-DAW-2024

# 2. Levantar los contenedores
docker compose up -d

# 3. Abrir en el navegador: http://localhost:8080
```

#### Opción B: Con XAMPP o WAMP
```bash
# 1. Clonar en la carpeta htdocs
git clone https://github.com/Chriiis85/TFG-DAW-2024.git

# 2. Importar la base de datos
# Abre phpMyAdmin e importa el archivo: BD_Motoring_Community.sql

# 3. Abrir en el navegador: http://localhost/TFG-DAW-2024/index.php
```

---

## 🇬🇧 English

Hello! 👋 I'm **Christian**. This repository contains the source code for my **Final Degree Project (TFG)** for the Higher Technical Degree in **Web Application Development (DAW)** at **I.E.S. Puig Adam** (Madrid, Spain).

As a Formula 1 enthusiast, I built this full-stack web application directly with core web technologies: **native PHP**, **vanilla JavaScript**, **CSS3**, and **MySQL**.

This project served as the initial prototype and architectural foundation for what later became [Motoring Community](https://github.com/Chriiis85/motoring-community) (my modern rewrite with Next.js and React). The forum logic, database schemas, and race results integration were all initially developed here.

### Features

- **Forum & User Accounts:** Secure login and registration, user profiles, and discussion threads for race weekends (`forum.php`, `users.php`).
- **Calendar & Countdown:** Race schedule with local session times and track circuit maps.
- **Live Standings:** Driver and Constructor championship tables with points and team standings.
- **Driver & Team Profiles:** Car specs, driver numbers, and biographies.
- **Web Accessibility:** Accessible semantic layout with keyboard navigation support (WCAG 2.1).
- **Docker Setup:** Pre-configured Docker environment running Apache, PHP, and MySQL for simple local setup.

### Technical Highlights

1. **Native PHP MVC Architecture:**  
   Clean separation between controllers, views, and data queries without frameworks, reinforcing core concepts of server-side sessions and HTTP lifecycles.
2. **Relational MySQL Database:**  
   Relational database schema (`BD_Motoring_Community.sql`) with foreign keys and indexes linking users, forum posts, and race data.
3. **Async JavaScript:**  
   Asynchronous fetch requests updating race telemetry and forum interactions without full-page reloads.

### Tech Stack

- **Backend:** Native PHP (MVC, PDO)
- **Database:** MySQL
- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **Environment:** Docker, Apache, `.htaccess`

### Local Setup

#### Option A: Docker
```bash
git clone https://github.com/Chriiis85/TFG-DAW-2024.git
cd TFG-DAW-2024
docker compose up -d
# Navigate to: http://localhost:8080
```

#### Option B: XAMPP / WAMP
```bash
# Clone into htdocs and import BD_Motoring_Community.sql in phpMyAdmin
# Navigate to: http://localhost/TFG-DAW-2024/index.php
```

---

<div align="center">
  <sub>Christian Moreno Díaz · TFG DAW 2024</sub>
</div>
