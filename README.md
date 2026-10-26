# 🏎️ TFG DAW 2024 — Motoring Community (PHP & MySQL)

[🇪🇸 Ver en Español](#-español) | [🇬🇧 View in English](#-english)

> 🎓 **Trabajo de Fin de Grado** para la obtención del título de **Técnico Superior en Desarrollo de Aplicaciones Web (DAW)**  
> 🏛️ **Centro:** I.E.S. Puig Adam (Getafe, Madrid) · **Año:** 2024  
> 🚀 **Evolución moderna (Next.js 16 + React 19):** [Motoring Community](https://github.com/Chriiis85/motoring-community) · [Live Demo](https://motoring-community-v1.vercel.app)

---

## 🇪🇸 Español

¡Hola! 👋 Soy **Christian**. Este repositorio contiene el código fuente completo de mi **Trabajo de Fin de Grado (TFG)** en **Desarrollo de Aplicaciones Web (DAW)**.

Como apasionado del motor y de la Fórmula 1, quise enfocar mi proyecto final en la creación de una **plataforma comunitaria Full Stack completa** construida de forma artesanal con tecnologías web fundamentales: **PHP nativo**, **JavaScript modular**, **CSS3 puro** y **MySQL**.

Este proyecto representa la **primera versión y el origen arquitectónico** de lo que más tarde evolucioné hacia un ecosistema moderno con Next.js y React en [Motoring Community](https://github.com/Chriiis85/motoring-community). Aquí se validaron todos los modelos de datos, flujos de autenticación, integración de APIs de carreras y la experiencia comunitaria.

### 🚀 Funcionalidades Principales

- 🏁 **Foro Comunitario y Sistema de Usuarios:** Registro e inicio de sesión seguro, gestión de perfiles, publicación de hilos temáticos y respuestas dinámicas entre aficionados (`forum.php`, `users.php`).
- 📅 **Calendario Oficial y Cuenta Atrás:** Horarios adaptados de cada Gran Premio, trazados de circuitos y cuenta regresiva hacia el fin de semana de carrera.
- 🏆 **Clasificación del Mundial en Vivo:** Tablas actualizadas de pilotos y constructores con puntuaciones, banderas de países y escuderías.
- 🏎️ **Fichas Técnicas de Pilotos y Escuderías:** Catálogo con perfiles biográficos, dorsales, monoplazas y estadísticas históricas.
- ♿ **Accesibilidad Universal (WCAG & WAI-ARIA):** Navegación completa por teclado (`tabindex`), etiquetas semánticas y contrastes verificados para compatibilidad con lectores de pantalla.
- 🐳 **Entorno Contenerizado con Docker:** Configuración lista para desplegar en local con Apache, PHP y base de datos MySQL.

### 💡 Retos Técnicos Resueltos

1. **Arquitectura MVC Limpia en PHP Nativo:**  
   Diseño estructurado separando controladores, vistas modulares (`header.php`, `footer.php`, `calendar.php`) y servicios de datos sin depender de frameworks comerciales, dominando los fundamentos del ciclo de petición HTTP y sesiones de servidor.
2. **Modelado Relacional e Integridad en MySQL:**  
   Esquema de base de datos relacional (`BD_Motoring_Community.sql`) con claves foráneas, índices optimizados y restricciones de integridad para soportar usuarios, hilos de debate, comentarios y resultados deportivos.
3. **Peticiones Asíncronas y Consumo de APIs:**  
   Lógica en JavaScript (`JS/script.js`, `JS/news.js`) para consumir datos en tiempo real de APIs de competición y refrescar componentes sin recargar la página.

### 🛠️ Stack Tecnológico

- **Backend:** PHP nativo (Arquitectura MVC, manejo de sesiones, PDO/MySQLi)
- **Base de Datos:** MySQL (Modelado relacional, consultas preparadas)
- **Frontend:** HTML5 semántico, CSS3 responsive (Flexbox, CSS Grid), JavaScript (ES6+)
- **DevOps:** Dockerfile & Docker Compose, Apache Web Server, `.htaccess`
- **Accesibilidad:** Estándares WCAG 2.1 / WAI-ARIA (a11y)

### 💻 Cómo probarlo en local

#### Opción A: Con Docker (Recomendado)
```bash
# 1. Clonar el repositorio
git clone https://github.com/Chriiis85/TFG-DAW-2024.git
cd TFG-DAW-2024

# 2. Levantar los contenedores de Docker
docker compose up -d

# 3. Abrir en el navegador
# http://localhost:8080
```

#### Opción B: Con XAMPP / WAMP / LAMP
```bash
# 1. Clonar en tu directorio htdocs
git clone https://github.com/Chriiis85/TFG-DAW-2024.git

# 2. Importar la base de datos
# Abre phpMyAdmin y crea la base de datos importando el archivo:
# BD_Motoring_Community.sql

# 3. Acceder en el navegador
# http://localhost/TFG-DAW-2024/index.php
```

---

## 🇬🇧 English

Hello! 👋 I'm **Christian**. This repository hosts the complete source code for my **Final Degree Project (TFG)** for the **Higher Technical Degree in Web Application Development (DAW)** at **I.E.S. Puig Adam** (Madrid, Spain).

As a motorsport and Formula 1 enthusiast, I focused my capstone project on building a **full-stack community platform from the ground up** using foundational web technologies: **native PHP**, **vanilla JavaScript**, **custom CSS3**, and **MySQL**.

This project represents the **initial blueprint and architecture** that I later evolved into the modern Next.js 16 and React 19 application: [Motoring Community](https://github.com/Chriiis85/motoring-community). The data models, authentication flows, race API consumption, and social dynamics were first designed and battle-tested here.

### 🚀 Key Features

- 🏁 **Community Forum & User Management:** User registration and secure authentication, profile management, and interactive discussion threads for Grand Prix weekends (`forum.php`, `users.php`).
- 📅 **Grand Prix Calendar & Countdown:** Race schedule with local session times, circuit track maps, and live race weekend countdowns.
- 🏆 **World Championship Standings:** Real-time driver and constructor championship tables with points, wins, and country flags.
- 🏎️ **Driver & Team Spec Sheets:** Comprehensive catalog with driver biographies, racing numbers, car specs, and career stats.
- ♿ **Universal Accessibility (WCAG & WAI-ARIA):** Full keyboard navigation (`tabindex`), accessible semantic markup, and verified contrast ratios for screen-reader support.
- 🐳 **Dockerized Environment:** Pre-configured Docker setup running Apache, PHP, and MySQL for instant local reproducibility.

### 💡 Technical Highlights

1. **Clean MVC Architecture in Native PHP:**  
   Modular separation between controllers, views (`header.php`, `footer.php`, `calendar.php`), and data services without heavy frameworks, solidifying deep understanding of HTTP request lifecycles and server-side session management.
2. **Relational Database Modeling with MySQL:**  
   Engineered a structured relational schema (`BD_Motoring_Community.sql`) with foreign keys, indexes, and integrity constraints for users, posts, comments, and telemetry/standings data.
3. **Asynchronous API Consumption:**  
   JavaScript (`JS/script.js`, `JS/news.js`) handling async requests to competition data feeds, updating page widgets without full browser reloads.

### 🛠️ Tech Stack

- **Backend:** Native PHP (MVC architecture, session handling, PDO)
- **Database:** MySQL (Relational schema, prepared statements)
- **Frontend:** Semantic HTML5, pure CSS3 (Flexbox, CSS Grid), JavaScript (ES6+)
- **DevOps:** Dockerfile & Docker Compose, Apache Web Server, `.htaccess`
- **Accessibility:** WCAG 2.1 / WAI-ARIA standards (a11y)

### 💻 Local Setup Guide

#### Option A: Using Docker (Recommended)
```bash
# 1. Clone repository
git clone https://github.com/Chriiis85/TFG-DAW-2024.git
cd TFG-DAW-2024

# 2. Start containers
docker compose up -d

# 3. Access in browser
# http://localhost:8080
```

#### Option B: Using XAMPP / WAMP
```bash
# 1. Clone inside your htdocs directory
git clone https://github.com/Chriiis85/TFG-DAW-2024.git

# 2. Import database
# Open phpMyAdmin, create a database and import:
# BD_Motoring_Community.sql

# 3. Navigate to:
# http://localhost/TFG-DAW-2024/index.php
```

---

<div align="center">
  <sub>Desarrollado con dedicación por Christian Moreno Díaz · © TFG DAW 2024</sub>
</div>
