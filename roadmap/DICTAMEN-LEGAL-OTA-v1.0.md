# DICTAMEN LEGAL — Estándares OTA para Aliun Travel SRL
**Fecha:** 19 Jul 2026 | **Referencia:** ISO 9468:2025
**Preparado por:** Director Aldo Hilario
**Custodiado por:** Hermes-QA (F6-LEGAL)

---

## MAPA DE PRIORIDADES F6-LEGAL

### Fase 1 — Cumplimiento mínimo inmediato (sprint)
| Código | Documento | Impacto |
|--------|-----------|---------|
| LEG-001 | Deploy política privacidad | Sin esto no cumplimos Ley 172-13 |
| LEG-002 | Política cancelaciones/reembolsos | Más reclamada por clientes |
| LEG-003 | Términos y condiciones | Requerido antes de escalar ventas |

### Fase 2 — Cumplimiento estándar OTA (mes)
LEG-006 al LEG-009: Reglas proveedor, disputas, precios, facturación

### Fase 3 — ISO 9468:2025 completo (trimestre)
LEG-010 al LEG-015: Cookies, consentimiento, quejas, marketing

---

## 1. Transparencia y Términos del Servicio

**Exige:** ToS vinculantes, reglas del proveedor, resolución de disputas.

Documentos a crear: LEG-003 (ToS), LEG-006 (reglas proveedor), LEG-007 (disputas)

---

## 2. Precios, Pago y Fiscalidad

**Exige:** Precio final sin cargos ocultos, ITBIS visible, derecho a factura.

Estado actual:
- BIEN: atlas_payments registra monto y método. WF-RECIBO-ABONO-v1 activo.
- FALTA: Política de precios publicada. ITBIS en flujo de reserva.

Documentos: LEG-008 (Precios y Pagos), LEG-009 (Facturación)

---

## 3. Cancelaciones y Reembolsos

**Exige:** Política VISIBLE antes de confirmar reserva. Usuarios pueden cancelar segun politica vigente al reservar.

Estado actual:
- FALTA: LEG-002 (política de reembolsos) — PROXIMA PRIORIDAD
- FALTA: Flujo de reserva no muestra política antes de confirmar
- GAP: Cancelaciones se manejan caso a caso sin documento rector

---

## 4. Protección de Datos y Privacidad

**Exige:** Política publicada, no divulgar sin consentimiento, marco de seguridad.

Estado actual:
- BIEN: POLITICA-PRIVACIDAD-v1.0 lista (LEG-001 — deploy pendiente Antigravity)
- BIEN: HTTPS/SSL activo. Service key en CI/CD secrets desde 17 Jul.
- FALTA: Política de cookies. Consentimiento explícito en checkout.

---

## 5. Protección al Consumidor y Disputas

**Exige:** Sistema formal de quejas en línea con mediación.

Estado actual:
- BIEN: Email + WhatsApp + Chatwoot (pendiente sdk.js)
- FALTA: Sistema formal de quejas documentado

Flujo de objeciones acordado (interno):
Cliente → Hermes Commercial → Hermes-QA revisa T&C → Director aprueba si reembolso

Documentos: LEG-013 (Protocolo Quejas), LEG-014 (Flujo Objeciones)

---

## 6. Contenido y Reseñas

Estado: hotel_profiles en Supabase (MCD-1 completado). Sin sistema de reseñas aún. Fase futura.

---

## 7. Marketing y Promociones

**Exige:** Sin servicios predeterminados. Condiciones visibles (no reembolsable).

Estado actual:
- BIEN: WF-MKT-GENERATE-OFFER-v3 activo con Instagram restaurado.
- FALTA: Aviso no reembolsable en ofertas cuando aplica.

---

## Marco Legal Aplicable (República Dominicana)

1. Ley 172-13 — Protección datos personales (cubierta en POLITICA-PRIVACIDAD-v1.0)
2. Ley 126-02 — Comercio electrónico y firmas digitales
3. Ley 358-05 — Protección al consumidor
4. ISO 9468:2025 — Estándar OTA internacional (referencia, no obligatorio en RD)
5. GDPR — Aplica si atendemos clientes UE (futuro)

---

*Hermes-QA custodio · F6-LEGAL · aliun-legal-v1 · 19 Jul 2026*
