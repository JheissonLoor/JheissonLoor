<div align="center">

# Jheisson Loayza Ortega (Jheisson Loor)
### Software Engineer · Full Stack & Backend Architecture
**Lima, Perú · Remoto / Híbrido**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jheisson_Loayza_Ortega-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jheisson-loayza-ortega-0007a7272/)
[![GitHub](https://img.shields.io/badge/GitHub-JheissonLoor-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/JheissonLoor)
[![Email](https://img.shields.io/badge/Contacto-Directo-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jheisson_acuario96@hotmail.com)

<p align="center">
  Desarrollador de software enfocado en la construcción de sistemas empresariales transaccionales, APIs REST resilientes, arquitecturas basadas en roles (RBAC) y modelado relacional riguroso con PostgreSQL, MySQL, React, TypeScript, Python y Flutter.
</p>

</div>

---

### 🌐 Professional Overview (English)
> **Software Engineer** specializing in **Full Stack & Backend Architecture**. Proven track record designing and implementing transactional business solutions, inventory ERP systems, real-time telecommunications platforms, and secure multi-tenant architectures using React, TypeScript, Next.js, Python (FastAPI, Flask), PostgreSQL, MySQL, and Flutter.

---

### 🏛️ Principios de Ingeniería / Engineering Principles

- **Seguridad en la Capa de Datos:** Prioridad por el aislamiento de datos y control de accesos a nivel de base de datos (*Row Level Security - RLS* en PostgreSQL/Supabase, esquemas fuertemente tipados e índices transaccionales) antes que delegar toda la integridad a la capa de aplicación.
- **Testing Pragmático & Automatizado:** Implementación de pipelines de integración continua (CI) con pruebas unitarias, validación de integración sobre bases de datos efímeras (*PGlite*) y pruebas End-to-End (*Playwright*).
- **Diseño Tipado y Guiado por Dominio:** Separación rigurosa de responsabilidades, hashing criptográfico (*Argon2id*), firma de tokens JWT (*jose*) y consultas SQL compiladas y tipadas en tiempo de desarrollo (*Kysely*, *Prisma*).

---

## 💼 Confidential Enterprise Engineering Projects

> *Sistemas empresariales propietarios actualmente en fase activa de construcción. Bajo prácticas estrictas de confidencialidad y propiedad intelectual, el código fuente y los datos productivos se mantienen privados. A continuación se detallan las decisiones de arquitectura, módulos implementados y rutas de desarrollo verificables:*

```
┌──────────────────────────────────────────────────────────────────────────────┐
│ 1. ERP Textil Industrial (Inventario Crudo, Despacho & Trazabilidad)        │
├──────────────────────────────────────────────────────────────────────────────┤
│ • Stack: React + TypeScript + Supabase (PostgreSQL 16) + PGlite              │
│ • Alcance: Control operativo y trazabilidad de rollos textiles desde el      │
│   ingreso físico a almacén hasta el despacho mayorista.                      │
│ • Funcionalidades Implementadas:                                             │
│   - Motor de cálculo y conciliación de inventario con suite de +60 pruebas   │
│     automatizadas ejecutadas en base de datos PostgreSQL en memoria (PGlite).│
│   - Cutover de políticas RLS para revocar privilegios anónimos sobre tablas │
│     y secuencias críticas de despacho y usuarios.                            │
│   - Generación dinámica de rotulado técnico y códigos QR para operarios.     │
│ • En Desarrollo / Roadmap:                                                   │
│   - Módulo de facturación electrónica y sincronización bidireccional         │
│     continua con sistemas contables existentes.                              │
└──────────────────────────────────────────────────────────────────────────────┘

┌──────────────────────────────────────────────────────────────────────────────┐
│ 2. Sistema Integral de RRHH y Control de Asistencias                         │
├──────────────────────────────────────────────────────────────────────────────┤
│ • Stack: TanStack Start (SSR) + TanStack Router + Kysely + Better Auth       │
│ • Alcance: Centralización de asistencias de personal, jerarquía de roles     │
│   administrativos y generación estructurada de auditoría operativa.          │
│ • Funcionalidades Implementadas:                                             │
│   - Arquitectura por capas (domain/application/infrastructure) con           │
│     consultas SQL tipadas en tiempo de compilación mediante Kysely.          │
│   - Autenticación endurecida con Better Auth, hashing Argon2id y sesiones    │
│     protegidas contra CSRF con middleware específico.                        │
│   - Motor inmutable de auditoría y ejecutor de migraciones con validación    │
│     estricta de invariantes de seguridad en bases de datos locales.          │
│ • En Desarrollo / Roadmap:                                                   │
│   - Módulo de reportes consolidados de planillas y diseño de conector de     │
│     solo lectura desacoplado para relojes biométricos (ZKBio Time).          │
└──────────────────────────────────────────────────────────────────────────────┘
```

---

## 🔬 Featured Projects / Engineering Case Studies

### 🏨 [NexoHotel — Property Management Platform (PMS)](https://github.com/JheissonLoor/nexohotel)
*Plataforma web administrativa privada para la operación diaria hotelera (gestión de habitaciones, huéspedes por DNI, caja y auditoría).*

- **Problema:** La administración hotelera requiere trazabilidad inmediata del estado de habitaciones y caja sin margen de descalce operativo.
- **Stack:** `Next.js 15` · `TypeScript` · `Prisma ORM` · `PostgreSQL` · `Docker Compose` · `Playwright`
- **Funcionalidades Implementadas:**
  - Máquina de estados finitos para ciclo de vida de habitación (`Disponible` → `Ocupada` → `Limpieza` → `Mantenimiento`).
  - Registro y check-in/out de huéspedes por DNI, control de caja diaria y emisión de comprobantes.
  - Autenticación con **Argon2id**, tokens JWT criptográficamente firmados con **Jose** y protección de rutas RBAC.
- **Evidencias & Aportes Técnicos:**
  - Suite de pruebas E2E con **Playwright** en `tests/`.
  - Contenerización multi-etapa con Docker y pipelines de backup y CI en GitHub Actions.
  - Diseño integral de esquema relacional y arquitectura Full Stack.

### 📡 [Unified Telecom QA Platform](https://github.com/JheissonLoor/Unified_Telecom_qa_platform_utp)
*Plataforma de comunicaciones unificadas con aseguramiento de calidad según estándares ISO/IEC.*

- **Problema:** Integrar servicios de voz/video IP con gestión centralizada de identidades bajo controles estrictos de calidad de software.
- **Stack:** `Python (FastAPI)` · `Asterisk PJSIP` · `SIP.js` · `midPoint (IAM)` · `coturn` · `PostgreSQL` · `Docker`
- **Funcionalidades Implementadas:**
  - Canal de señalización PJSIP en Asterisk integrado con clientes SIP en navegador web mediante WebRTC.
  - Sincronización y aprovisionamiento automatizado de cuentas de usuario con Evolveum midPoint.
  - Reverse proxy Nginx y servidor STUN/TURN con coturn para conectividad NAT.
- **Evidencias & Aportes Técnicos:**
  - 13 pruebas automatizadas y Quality Gates en GitHub Actions (`quality.yml`).
  - Orquestación de infraestructura multi-contenedor con Docker Compose.

### 🍽️ [UTTOF Restaurant — Multi-Tenant Foodservice Engine](https://github.com/JheissonLoor/UUTOF-restaurant)
*Plataforma gastronómica multi-sucursal con pantallas de cocina en tiempo real (KDS).*

- **Problema:** Coordinar pedidos de salón, comandas de cocina y cobranza en locales gastronómicos con baja latencia y consistencia transaccional.
- **Stack:** `Python (FastAPI)` · `React` · `MySQL / MariaDB (SQLAlchemy Asyncmy)` · `Tailwind CSS`
- **Funcionalidades Implementadas:**
  - Backend relacional asíncrono con 11 scripts de migración SQL para gestión multi-sucursal y configuración de locales.
  - Pantalla de Cocina (KDS) con gestión de estados de preparación en tiempo real.
  - Módulos desacoplados para Meseros (toma de comandas), Cocina y Administrador.
  - Localización peruana: moneda PEN (S/), validación telefónica (+51) y flujo de pagos QR con Yape.
- **Evidencias & Aportes Técnicos:**
  - Arquitectura separada frontend/backend con motor asíncrono SQLAlchemy y pool de conexiones `asyncmy`.

### 📱 [Aethera — Real-Time Mobile Application](https://github.com/JheissonLoor/aethera)
*Aplicación móvil con arquitectura limpia y sincronización reactiva para comunicación de parejas a larga distancia.*

- **Problema:** Mantener experiencias visuales fluidas y sincronización de presencia en tiempo real con tolerancia a desconexión de red.
- **Stack:** `Flutter` · `Dart 3.7+` · `Riverpod 3.x` · `Firebase (Auth, Realtime DB, Cloud Messaging, Storage)`
- **Funcionalidades Implementadas:**
  - Arquitectura modular orientada a características (*Feature-First*) impulsada por Riverpod.
  - Cola de sincronización fuera de línea (`_offlineQueue`) para despacho de acciones al recuperar conectividad.
  - Gestión de sesiones con Firebase Auth y notificaciones push con Cloud Messaging.
- **En Desarrollo / Pendiente:**
  - Integración extendida de servicios de analítica y sincronización persistente en segundo plano.
- **Evidencias & Aportes Técnicos:**
  - 11 pruebas unitarias y de widgets en `test/` con pipeline automatizado en GitHub Actions (`ci_flutter.yml`).

### 📊 [Tambo BI — DataMart Analítico & Dashboard](https://github.com/JheissonLoor/tambo-bi-grupo06)
*DataMart en esquema copo de nieve con dashboard interactivo para análisis de promociones comerciales.*

- **Contexto & Naturaleza:** Caso de estudio analítico colaborativo (proyecto académico grupal, UTP) desarrollado sobre un conjunto de datos sintéticos representativo de transacciones de conveniencia minorista (Sede UC).
- **Stack:** `React` · `Vite` · `TypeScript` · `Supabase / PostgreSQL` · `Python` · `Vercel`
- **Funcionalidades Implementadas:**
  - Modelo dimensional analítico en copo de nieve (tabla de hechos, dimensiones y subdimensiones de promociones y productos).
  - Vistas analíticas SQL para evaluación de ticket promedio, márgenes de ganancia y elasticidad por campaña comercial.
  - Dashboard web interactivo con despliegue productivo verificado en Vercel.
- **Evidencias & Aportes Técnicos:**
  - Esquemas de migración y scripts de verificación SQL reproducibles en `supabase/`.

---

## 📊 Competencias Técnicas / Technical Matrix

```
┌────────────────────────┬─────────────────────────────────────────────────────────────┐
│ Dominio                │ Tecnologías de Trabajo Principal                            │
├────────────────────────┼─────────────────────────────────────────────────────────────┤
│ Frontend & Web         │ React · TypeScript · JavaScript · Next.js 15 · Tailwind CSS │
│ Backend & APIs         │ Python (FastAPI, Flask) · Node.js · RESTful API Design      │
│ Bases de Datos         │ PostgreSQL 16 · Supabase · MySQL / MariaDB · Prisma · Kysely│
│ Móvil                  │ Flutter · Dart 3.x · Riverpod                               │
│ Calidad & DevOps       │ Git · GitHub Actions (CI/CD) · Docker · Playwright · Pytest │
├────────────────────────┼─────────────────────────────────────────────────────────────┤
│ Dominio                │ Tecnologías Complementarias / Académicas                    │
├────────────────────────┼─────────────────────────────────────────────────────────────┤
│ Backend Complementario │ Java · Spring Boot · Java Servlets / JSP · JDBC             │
└────────────────────────┴─────────────────────────────────────────────────────────────┘
```

---

## 🎓 Formación / Education

- **Universidad Tecnológica del Perú (UTP)**
  *Ingeniería de Sistemas e Informática · Estudios de pregrado en curso*
- **Áreas de profundización técnica:** Arquitectura de software, diseño de bases de datos relacionales, seguridad defensiva en aplicaciones web y aseguramiento de la calidad de software (QA / testing automatizado).

---

## 📫 Contacto / Let's Connect

- **LinkedIn:** [linkedin.com/in/jheisson-loayza-ortega-0007a7272](https://www.linkedin.com/in/jheisson-loayza-ortega-0007a7272/)
- **Correo Directo:** [jheisson_acuario96@hotmail.com](mailto:jheisson_acuario96@hotmail.com)
- **GitHub:** [@JheissonLoor](https://github.com/JheissonLoor)

<div align="center">
  <sub>Construido con precisión técnica y rigor de ingeniería · 2026</sub>
</div>
