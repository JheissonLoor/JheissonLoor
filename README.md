<div align="center">

# Jheisson Loayza Ortega (Jheisson Loor)
### Software Engineer · Full Stack & Backend Architecture
**Lima, Perú · Remoto / Híbrido**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jheisson_Loayza_Ortega-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jheisson-loayza-ortega-0007a7272/)
[![GitHub](https://img.shields.io/badge/GitHub-JheissonLoor-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JheissonLoor)
[![Email](https://img.shields.io/badge/Contacto-Directo-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jheisson_acuario96@hotmail.com)

<p align="center">
  <em>Estudiante de últimos ciclos de Ingeniería de Sistemas e Informática (Universidad Tecnológica del Perú, graduación prevista: dic. 2026).</em><br>
  Enfocado en el diseño e implementación de sistemas empresariales transaccionales, APIs resilientes, arquitecturas basadas en roles (RBAC), control de identidades (IAM) y modelado relacional riguroso con PostgreSQL, React, TypeScript, Python y Flutter.
</p>

</div>

---

### 🌐 Executive Summary (English)
> **Systems & Computer Engineering student (Graduating Dec 2026 @ UTP, Peru)** focused on **Full Stack & Backend Engineering**. Hands-on experience building enterprise inventory & resource planning systems (ERP, HR/Attendance), real-time telecommunications platforms (Asterisk, WebRTC), and secure RESTful architectures using React, TypeScript, Next.js, Python (FastAPI/Flask), PostgreSQL, Supabase, and Flutter.

---

### 🏛️ Principios de Ingeniería / Engineering Principles

- **Seguridad en la Capa de Datos:** Implementación de aislamiento a nivel de base de datos (*Row Level Security - RLS* en PostgreSQL/Supabase) y esquemas fuertemente tipados antes que delegar toda la integridad a la capa de aplicación.
- **Testing Pragmático & Automatizado:** Construcción de pipelines de integración continua (CI) con suites de pruebas unitarias, de integración sobre bases de datos efímeras (*PGlite*) y pruebas End-to-End (*Playwright*).
- **Arquitectura Basada en Dominio:** Separación estricta de responsabilidades, hashing criptográfico de contraseñas (*Argon2id*), firma de tokens JWT (*jose*) y manejo reactivo de estados en frontend y móvil (*Riverpod / TanStack*).

---

## 💼 Experiencia en Sistemas Empresariales (NDA Protected)

> *Por acuerdos de confidencialidad y propiedad intelectual, el código fuente de los siguientes sistemas se mantiene en repositorios privados. Se detallan exclusivamente las decisiones de arquitectura, desafíos técnicos y soluciones de ingeniería implementadas:*

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ 1. ERP Textil Industrial (Inventario Crudo, Despacho & Trazabilidad)        │
├──────────────────────────────────────────────────────────────────────────────┤
│ • Stack: React + TypeScript + Supabase (PostgreSQL 16) + PGlite              │
│ • Desafío: Trazabilidad en tiempo real de rollos textiles desde el ingreso   │
│   a planta hasta el despacho mayorista, mitigando inconsistencias de stock. │
│ • Solución de ingeniería:                                                   │
│   - Motor de cálculo y conciliación de inventario con +60 tests automatizados│
│     ejecutados en base de datos PostgreSQL local en memoria (PGlite).        │
│   - Políticas RLS estrictas y migración de permisos para revocar privilegios │
│     anónimos sobre secuencias y tablas críticas de negocio.                  │
│   - Generación dinámica de rotulado técnico y códigos QR para planta.        │
└──────────────────────────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────────────────────────┐
│ 2. Sistema Integral de RRHH y Control de Asistencias                         │
├──────────────────────────────────────────────────────────────────────────────┤
│ • Stack: TanStack Start (SSR) + TanStack Router + Kysely + Better Auth       │
│ • Desafío: Centralizar la asistencia de personal, roles administrativos y    │
│   generación de reportes de auditoría con alta velocidad de respuesta.       │
│ • Solución de ingeniería:                                                   │
│   - Consultas SQL compiladas y tipadas en tiempo de desarrollo (Kysely)      │
│     sin la sobrecarga de consultas generadas por un ORM tradicional.         │
│   - Hashing seguro de credenciales con Argon2id y sesión endurecida.         │
│   - Pipeline de migración, seeding y verificación reproducible localmente.   │
└──────────────────────────────────────────────────────────────────────────────┘
```

---

## 🔬 Proyectos Destacados de Código Abierto / Featured Case Studies

### 🏨 [NexoHotel — Property Management Platform (PMS)](https://github.com/JheissonLoor/nexohotel)
*Plataforma web administrativa privada para hotelería real (gestión de habitaciones, huéspedes por DNI, caja diaria y auditoría).*

- **Stack:** `Next.js 15` · `TypeScript` · `Prisma ORM` · `PostgreSQL` · `Docker Compose` · `Playwright`
- **Decisiones & Aportes Técnicos:**
  - **Máquina de estados de habitación:** Gestión de ciclos de vida completos (`Disponible` → `Ocupada` → `Limpieza` → `Mantenimiento`).
  - **Seguridad aplicada:** Hashing con **Argon2id**, tokens JWT criptográficamente firmados con librería **Jose** y protección de rutas con control de acceso basado en roles (RBAC).
  - **DevOps & QA:** Suite de pruebas E2E con **Playwright**, containerización Docker multi-etapa y workflows de backup y CI en GitHub Actions.

### 📡 [Unified Telecom QA Platform](https://github.com/JheissonLoor/Unified_Telecom_qa_platform_utp)
*Plataforma de telecomunicaciones unificadas orientada a aseguramiento de la calidad bajo estándares ISO/IEC.*

- **Stack:** `Python` · `FastAPI` · `Asterisk PJSIP` · `SIP.js` · `midPoint (IAM)` · `coturn` · `PostgreSQL` · `Docker`
- **Decisiones & Aportes Técnicos:**
  - **Telefonía IP & WebRTC:** Orquestación de canal de señalización PJSIP en Asterisk integrado con clientes SIP en navegador web.
  - **Gestión de Identidades (IAM):** Integración con **midPoint** para aprovisionamiento automatizado y sincronización centralizada de cuentas de usuario.
  - **Pipeline de Calidad:** Quality Gates con GitHub Actions validando tipado, linters y 13 pruebas automatizadas.

### 🍽️ [UTTOF Restaurant — Multi-Tenant Foodservice Engine](https://github.com/JheissonLoor/UUTOF-restaurant)
*Plataforma de gestión gastronómica multi-sucursal con pantallas de cocina en tiempo real (KDS).*

- **Stack:** `Python (FastAPI/Flask)` · `React` · `PostgreSQL` · `Tailwind CSS`
- **Decisiones & Aportes Técnicos:**
  - **Diseño Relacional Robusto:** 11 scripts de migración estructurados para soportar multi-local, configuración de empresa y estados transaccionales de comandas.
  - **Módulos desacoplados:** Interfaces especializadas para Clientes (menú QR), Meseros (toma de pedidos), Cocina (KDS con cola de preparación) y Gerencia.
  - **Localización Perú:** Moneda en PEN (S/), pagos QR vía Yape y formateo telefónico regional (+51).

### 📱 [Aethera — Real-Time Mobile Application](https://github.com/JheissonLoor/aethera)
*Aplicación móvil con arquitectura limpia y sincronización reactiva en tiempo real para parejas a larga distancia.*

- **Stack:** `Flutter` · `Dart 3.7+` · `Riverpod 3.x` · `Firebase (Auth, Realtime DB, Cloud Messaging, Storage)`
- **Decisiones & Aportes Técnicos:**
  - **Arquitectura Modular:** Estructuración de carpetas orientada a características (*Feature-First*) impulsada por Riverpod.
  - **Sincronización en la Nube:** Manejo de presencia activa, persistencia remota y notificaciones push asíncronas.
  - **Testing & CI:** Suite de 11 pruebas unitarias y pipeline automatizado con GitHub Actions (`ci_flutter.yml`).

### 📊 [Tambo BI — DataMart Analítico & Dashboard](https://github.com/JheissonLoor/tambo-bi-grupo06)
*DataMart en esquema copo de nieve con dashboard interactivo para análisis de promociones comerciales.*

- **Stack:** `React` · `Vite` · `TypeScript` · `Supabase / PostgreSQL` · `Python` · `Vercel`
- **Decisiones & Aportes Técnicos:**
  - **Modelado Dimensional:** Diseño de modelo analítico en copo de nieve para optimización de consultas OLAP sobre promociones minoristas.
  - **Despliegue Continuo:** Aplicación productiva desplegada en Vercel con integración a base de datos analítica.

---

## 📊 Matriz de Competencias Técnicas / Technical Matrix

| Dominio | Tecnologías Principales | Enfoque & Buenas Prácticas |
| :--- | :--- | :--- |
| **Backend & APIs** | Python (FastAPI, Flask), Node.js, TypeScript, Java (Spring Boot, Servlets/JSP) | Diseño RESTful, autenticación JWT/Argon2id, middlewares de auditoría, WebSockets/WebRTC. |
| **Bases de Datos** | PostgreSQL 16, Supabase, Prisma ORM, Kysely, PGlite | Modelado relacional, esquemas dimensionales (Snowflake), Row Level Security (RLS), migraciones reproducibles. |
| **Frontend & Web** | React, Next.js 15, TanStack Router/Start, Tailwind CSS | Server Components, tipado estricto en TypeScript, accesibilidad y renderizado eficiente. |
| **Móvil** | Flutter, Dart 3.7+, Riverpod | Clean Architecture / Feature-First, sincronización en tiempo real y offline con Firebase. |
| **DevOps & QA** | Docker, Docker Compose, GitHub Actions, Playwright, Pytest | Contenerización multi-etapa, pipelines de CI/CD, pruebas de integración y E2E. |

---

## 🎓 Formación y Trayectoria

- **Ingeniería de Sistemas e Informática** — Universidad Tecnológica del Perú (UTP)
  *Ciclos finales · Graduación estimada: Diciembre 2026*
- **Líneas de profundización técnica:** Arquitectura de software distribuido, seguridad defensiva en aplicaciones web, testing automatizado y modelado de datos transaccionales de alto rendimiento.

---

## 📫 Contacto / Let's Connect

- **LinkedIn:** [linkedin.com/in/jheisson-loayza-ortega-0007a7272](https://www.linkedin.com/in/jheisson-loayza-ortega-0007a7272/)
- **Correo Directo:** [jheisson_acuario96@hotmail.com](mailto:jheisson_acuario96@hotmail.com)
- **GitHub:** [@JheissonLoor](https://github.com/JheissonLoor)

<div align="center">
  <sub>Construido con precisión técnica y rigor de ingeniería · 2026</sub>
</div>
