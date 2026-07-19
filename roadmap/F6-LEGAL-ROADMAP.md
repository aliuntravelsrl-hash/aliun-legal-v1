# F6-LEGAL — Roadmap Estratégico
**Estado:** Frente futuro — en desarrollo conceptual
**Fecha:** 18 Jul 2026 | ATLAS-TECH + Director

---

## Visión

Aliun Travel SRL opera como **plataforma de intermediación bidireccional B2B + B2C**.
Esta naturaleza requiere una capa legal robusta que cubra:

- Relación con clientes individuales (B2C)
- Relación con mayoristas y agencias (B2B)
- Relación con proveedores hoteleros
- Compliance digital (Ley 172-13, Ley 126-02)
- Protección ante objeciones y disputas

---

## Árbol de documentos necesarios

```
F6-LEGAL
├── POLÍTICAS (cliente ve)
│   ├── Privacidad ✅ v1.0 vigente
│   ├── Reembolsos ← próxima prioridad
│   ├── Cookies
│   └── Cancelaciones
│
├── TÉRMINOS (cliente acepta)
│   ├── T&C Generales
│   ├── T&C B2B Mayoristas
│   └── T&C Excursiones
│
├── CONTRATOS (firma)
│   ├── Cliente Individual
│   ├── Cliente Grupo
│   ├── Proveedor Hotel
│   └── Mayorista/Agencia
│
└── OPERATIVO (interno)
    ├── Protocolo manejo objeciones
    ├── Protocolo reembolsos
    └── Protocolo disputas con proveedores
```

---

## Owner del frente

**Pendiente definir.** Opciones:
- Director maneja F6-LEGAL directamente
- Hermes-QA ampliado como supervisor de compliance
- Sub-agente legal dedicado (largo plazo)

---

## Tareas registradas

| Código | Tarea | Estado |
|--------|-------|--------|
| LEG-001 | Deploy política de privacidad | Pendiente Antigravity |
| LEG-002 | Política de reembolsos | 🔲 Pendiente |
| LEG-003 | Términos y condiciones | 🔲 Pendiente |
| LEG-004 | Contrato cliente individual | 🔲 Pendiente |
| LEG-005 | Términos B2B mayoristas | 🔲 Pendiente |

---

## Relación con el roadmap técnico

F6-LEGAL se activa completamente cuando:
1. Chatwoot online (clientes ven T&C antes de reservar)
2. Flow de reserva web (aceptación de T&C en checkout)
3. Sistema de firmas digitales (Ley 126-02)

*ATLAS-TECH · F6-LEGAL · 18 Jul 2026*
