# Administración — Gestión Empresarial para PyMEs Peruanas

> **Parte del ecosistema [ARKELYTHEX](https://github.com/arkelythex)** — Infraestructura fiscal para LATAM.

**¿Para quién es esto?** Para dueños de pequeñas y medianas empresas en Perú que necesitan un sistema sencillo pero potente para gestionar su negocio — inventarios, facturación, cuentas, y reportes — todo en un solo lugar.

---

## ¿Qué hace?

Administración te permite llevar el control de tu empresa sin complicación:

- **Inventarios** — control de stock, entradas y salidas
- **Facturación** — emisión y seguimiento de comprobantes
- **Cuentas por cobrar/pagar** — control de ingresos y egresos
- **Reportes gerenciales** — visibilidad del estado de tu negocio

---

## Empezar

```bash
# Clonar
git clone https://github.com/arkelythex/Administracion.git
cd Administracion

# Instalar dependencias
bun install

# Configurar entorno
cp .env.example .env

# Iniciar
bun dev
```

> **Nota:** Este proyecto está en fase prototipo. Cosas pueden cambiar.

---

## Stack

TypeScript · React · SQL · REST API

---

## Architecture (current, prototype phase)

![Administración architecture](docs/diagrams/admin.architecture.light.svg#gh-light-mode-only)
![Administración architecture](docs/diagrams/admin.architecture.dark.svg#gh-dark-mode-only)

The only module implemented so far is payroll: a React frontend calls an Eden Treaty
typed client, which talks to the live Elysia server (`server/index.ts`, the one `bun dev`
actually runs), which calls the payroll calculation engine. `src/server/` is unused
scaffolding not wired into the running app — kept out of this diagram since it isn't real
today.

---

## 🌐 Ecosistema ARKELYTHEX

| Proyecto | Descripción |
|----------|-------------|
| [Monorepo ARKELYTHEX](https://github.com/arkelythex/Arkelythex) | Hub principal de desarrollo |
| [Digital Public Peru](https://github.com/arkelythex/Digital_Public_peru) | Transparencia fiscal |
| [elect-validate](https://github.com/arkelythex/elect-validate) | Validación electoral |
| [EdgeTraz-Agro](https://github.com/arkelythex/EdgeTraz-Agro) | Trazabilidad agroindustrial |
| [Administración](https://github.com/arkelythex/Administracion) | Gestión empresarial |

---

<p align="center">
  <sub>Parte de <a href="https://github.com/arkelythex">ARKELYTHEX</a> — Construyendo la infraestructura que LATAM merece.</sub>
</p>
