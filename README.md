<div align="center">

# Jheisson Loayza Ortega
### Software Engineer | Full Stack & Backend Developer
**Lima, Perú · Remoto / Híbrido**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jheisson_Loayza_Ortega-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jheisson-loayza-ortega-0007a7272/)
[![GitHub](https://img.shields.io/badge/GitHub-JheissonLoor-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/JheissonLoor)
[![Email](https://img.shields.io/badge/Contacto-jheisson__acuario96%40hotmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:jheisson_acuario96@hotmail.com)

<p align="center">
  Desarrollador de software enfocado en el diseño e implementación de sistemas transaccionales empresariales, APIs REST resilientes, modelado relacional riguroso (PostgreSQL / MySQL) y modernización progresiva de procesos operativos con React, TypeScript, Python y Flutter.
</p>

</div>

---

### 🌐 Professional Summary (English)
> **Software Engineer** specializing in **Full Stack & Backend Architecture**. Hands-on experience developing business-critical applications, enterprise ERP modules, inventory traceability engines, and relational database architectures. Strong advocate of domain-driven design, data-layer security (RLS, RBAC), automated continuous testing, and safe, incremental migrations of legacy environments.

---

## 💼 Professional Experience

### Desarrollador de Software / Full Stack Developer
**Comercial Cerro Alto S.A.C.** *(anteriormente CoolImport S.A.C.)*  
*Lima, Perú · Operaciones textiles e industriales*

Desarrollo y modernización de plataformas operativas internas para la digitalización y trazabilidad de procesos productivos, control de inventarios y gestión administrativa.

#### 1. Sistema ERP y Trazabilidad Textil *(En desarrollo activo)*
- **Trazabilidad de Planta:** Diseño de contratos de datos y flujo operativo para el registro, pesaje y rotulado técnico de rollos de tela cruda mediante códigos QR, reduciendo la dependencia de registros manuales y hojas de cálculo.
- **Transición Progresiva de Datos:** Migración gradual de estructuras de inventario hacia esquemas relacionales en PostgreSQL / Supabase, manteniendo compatibilidad operativa con aplicaciones heredadas en planta y terminales móviles (tablets).
- **Lógica de Negocio y Calidad:** Implementación de reglas desacopladas para validación de ingresos y despachos mayoristas con suites de pruebas automatizadas en Vitest para lógica de dominio, conciliación y control de permisos.

#### 2. Sistema Integral de RR.HH. y Control de Asistencias *(En desarrollo activo)*
- **Arquitectura Independiente:** Diseño de una aplicación desacoplada del ERP con arquitectura por capas (*domain / application / infrastructure*) basada en TanStack Start y TypeScript en modo estricto.
- **Seguridad en Capa de Datos:** Implementación de consultas SQL fuertemente tipadas en tiempo de compilación con Kysely, autenticación local con Better Auth (hashing criptográfico Argon2id), protección contra CSRF y motor inmutable de auditoría para accesos y cambios de rol.
- **Aislamiento Técnico:** Verificación local rigurosa mediante suites de pruebas automatizadas sobre entornos de base de datos efímeros y pipelines de integración continua (CI) en GitHub Actions bajo PostgreSQL 16 y 17.

> *Nota de confidencialidad y estado: Ambos sistemas son desarrollos empresariales internos y confidenciales. No se exponen datos operativos, información de personal ni credenciales productivas. Módulos como la sincronización contable o la integración de lectura para relojes biométricos se encuentran en fase de diseño o pruebas sintéticas locales.*

---

## ⚙️ Engineering Ownership & How I Work

Más allá de la codificación, mi enfoque de ingeniería prioriza la estabilidad operativa, la comprensión del negocio y la reducción de riesgos:

- **Levantamiento y Análisis Operativo:** Trabajo directo con las áreas de almacén, planta y administración para traducir flujos manuales de trabajo en especificaciones técnicas claras y modelos de datos normalizados.
- **Seguridad en la Capa de Datos (Data-Layer First):** Establecimiento de integridad referencial, restricciones transaccionales, auditoría y control de acceso a nivel de base de datos antes de confiar exclusivamente en validaciones de la interfaz.
- **Migración Segura y Convivencia de Sistemas:** Capacidad para modernizar sistemas sin interrumpir la operación diaria, diseñando capas de compatibilidad entre APIs modernas y servicios legados.
- **Testing Automatizado y Calidad:** Adopción de pruebas unitarias, de integración y E2E (Playwright, Vitest, Node Test Runner) integradas en pipelines de CI/CD para evitar regresiones antes de cada entrega.
- **Documentación Técnica Rigurosa:** Redacción de especificaciones de arquitectura, guías de continuidad operativa y registros de decisiones técnicas (ADRs) para garantizar la mantenibilidad del código.

---

## 🚀 Independent Products & Ventures

*Iniciativas tecnológicas y productos personales desarrollados de forma independiente:*

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│ 1. Aptelya — Global AI-Powered Learning Platform                                       │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ • Stack: React / Next.js · TypeScript · Supabase (PostgreSQL + RLS) · Redis · Worker   │
│ • Descripción: Plataforma interactiva para el aprendizaje práctico de ingeniería de    │
│   prompts e IA generativa. Cuenta con un corte vertical completo: diagnóstico, builder │
│   interactivo, procesamiento en segundo plano con worker asíncrono y portafolio.       │
│ • Enfoque: Arquitectura Full Stack modular, soporte multi-idioma nativo (ES, EN, PT)  │
│   y sandbox determinista de evaluación para pruebas reproducibles sin costo de API.    │
└────────────────────────────────────────────────────────────────────────────────────────┘

┌────────────────────────────────────────────────────────────────────────────────────────┐
│ 2. Aulanza — Educational Technology Foundation                                         │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ • Stack: Monorepo reproducible (pnpm) · Python 3.11 / FastAPI (uv) · PostgreSQL 17     │
│ • Descripción: Fundación de arquitectura para una plataforma pedagógica orientada a    │
│   docentes peruanos, estructurada bajo estándares de diseño modular y tipado estricto. │
│ • Enfoque: Contratos de API autogenerados, base de datos normalizada para metadatos    │
│   normativos públicos y pipeline de validación local mediante contenedores Docker.     │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🔬 Featured Engineering Projects / Case Studies

### 🏨 [NexoHotel — Property Management Platform (PMS)](https://github.com/JheissonLoor/nexohotel)
*Plataforma web administrativa privada para la gestión operativa y financiera hotelera.*

- **Problema:** Desfase operativo y falta de trazabilidad en el control de habitaciones, registros de huéspedes y caja diaria en establecimientos hoteleros independientes.
- **Stack:** `Next.js 15` · `TypeScript` · `Prisma ORM` · `PostgreSQL` · `Docker Compose` · `Playwright`
- **Funcionalidades Implementadas:**
  - Máquina de estados finitos para el ciclo de vida de cada habitación (`Disponible` → `Ocupada` → `Limpieza` → `Mantenimiento`).
  - Registro de huéspedes por DNI, control de arqueo de caja por turnos y emisión de comprobantes.
  - Autenticación segura mediante **Argon2id**, tokens JWT firmados criptográficamente (**Jose**) y protección de rutas RBAC.
- **Evidencia Técnica:** Suite de pruebas End-to-End con **Playwright** en `tests/`, Docker multi-etapa y pipelines de validación en GitHub Actions.

### 📡 [Unified Telecom QA Platform](https://github.com/JheissonLoor/Unified_Telecom_qa_platform_utp)
*Plataforma de comunicaciones unificadas con aseguramiento de calidad según estándares ISO/IEC.*

- **Contexto:** Proyecto académico colaborativo enfocado en ingeniería de calidad de software y estándares ISO/IEC 25010.
- **Stack:** `Python (FastAPI)` · `Asterisk PJSIP` · `SIP.js` · `midPoint (IAM)` · `coturn` · `PostgreSQL` · `Docker`
- **Aportes y Responsabilidad Técnica:**
  - Configuración del canal de señalización PJSIP en Asterisk e integración con clientes SIP web vía WebRTC.
  - Integración de servicios de gestión de identidades con Evolveum midPoint y pasarela STUN/TURN con coturn.
  - Implementación de Quality Gates en GitHub Actions (`quality.yml`) con pruebas automatizadas de cobertura.

### 🍽️ [UTTOF Restaurant — Foodservice Operations Engine](https://github.com/JheissonLoor/UUTOF-restaurant)
*Plataforma integral de gestión gastronómica con pantallas de cocina en tiempo real (KDS).*

- **Contexto:** Proyecto académico de Arquitectura de Software para locales gastronómicos multi-sucursal.
- **Stack:** `Python (FastAPI)` · `React` · `MySQL / MariaDB (SQLAlchemy Asyncmy)` · `Tailwind CSS`
- **Funcionalidades Implementadas:**
  - Backend relacional asíncrono con scripts de migración para administración de cartas y sucursales.
  - Pantalla de Cocina (KDS) interactiva con control de estados de comandas en tiempo real.
  - Localización peruana: manejo de moneda PEN (S/), validación telefónica (+51) y flujo de pagos QR con Yape.

### 📱 [Aethera — Real-Time Mobile Application](https://github.com/JheissonLoor/aethera)
*Aplicación móvil reactiva con tolerancia a desconexión para parejas a larga distancia.*

- **Problema:** Mantener experiencias visuales fluidas y sincronización de presencia en tiempo real bajo condiciones de conectividad inestable.
- **Stack:** `Flutter` · `Dart 3.7+` · `Riverpod 3.x` · `Firebase (Auth, Realtime DB, Cloud Messaging)`
- **Funcionalidades Implementadas:**
  - Arquitectura modular orientada a características (*Feature-First*) impulsada por Riverpod.
  - Cola de sincronización fuera de línea (`_offlineQueue`) para despacho retardado de acciones al recuperar conectividad.
  - Suite de pruebas unitarias y de widgets con pipeline automatizado en GitHub Actions (`ci_flutter.yml`).

### 📊 [Tambo BI — DataMart Analítico & Dashboard](https://github.com/JheissonLoor/tambo-bi-grupo06)
*DataMart en esquema copo de nieve con dashboard interactivo para análisis de promociones comerciales.*

- **Contexto:** Caso de estudio analítico colaborativo (proyecto grupal UTP) sobre transacciones representativas del sector minorista de conveniencia (Sede UC).
- **Stack:** `React` · `Vite` · `TypeScript` · `Supabase / PostgreSQL` · `Vercel`
- **Aportes Técnicos:** Modelado dimensional en copo de nieve (hechos, dimensiones y subdimensiones), vistas analíticas SQL para evaluación de ticket promedio y dashboard web desplegado en Vercel.

---

## 📊 Technical Competencies

```
┌────────────────────────┬─────────────────────────────────────────────────────────────┐
│ Dominio                │ Tecnologías Principales (Producción y Desarrollo Activo)    │
├────────────────────────┼─────────────────────────────────────────────────────────────┤
│ Frontend & Web         │ TypeScript · React · Next.js 15 · Tailwind CSS · TanStack   │
│ Backend & APIs         │ Python (FastAPI, Flask) · Node.js · RESTful Architecture    │
│ Bases de Datos         │ PostgreSQL 16/17 · Supabase · MySQL / MariaDB · Kysely      │
│ Móvil                  │ Flutter · Dart 3.x · Riverpod                               │
│ Calidad & DevOps       │ Git · GitHub Actions (CI/CD) · Docker · Playwright · Vitest │
├────────────────────────┼─────────────────────────────────────────────────────────────┤
│ Dominio                │ Tecnologías Complementarias / Académicas                    │
├────────────────────────┼─────────────────────────────────────────────────────────────┤
│ Backend Complementario │ Java · Spring Boot · Java Servlets / JSP · Prisma ORM       │
│ Almacenamiento & Otros │ MongoDB · SQLite · Redis                                    │
└────────────────────────┴─────────────────────────────────────────────────────────────┘
```

---

## 🎓 Education & Background

- **Universidad Tecnológica del Perú (UTP)**  
  *Ingeniería de Sistemas e Informática · Estudios de pregrado en curso*
- **Líneas de profundización técnica:** Arquitectura de software distribuido, seguridad y modelado en bases de datos relacionales, aseguramiento de la calidad (QA / testing automatizado) y modernización de sistemas empresariales.

---

## 📫 Contact / Let's Connect

- **LinkedIn:** [linkedin.com/in/jheisson-loayza-ortega-0007a7272](https://www.linkedin.com/in/jheisson-loayza-ortega-0007a7272/)
- **Correo Directo:** [jheisson_acuario96@hotmail.com](mailto:jheisson_acuario96@hotmail.com)
- **GitHub:** [@JheissonLoor](https://github.com/JheissonLoor)

<div align="center">
  <sub>Diseñado con precisión de ingeniería, transparencia técnica y rigor profesional · 2026</sub>
</div>
