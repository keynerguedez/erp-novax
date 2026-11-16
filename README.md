# ERP Grupo Novax — demo navegable

Prototipo del ERP para el grupo de empresas de Keyner (Inversiones Novax C.A., Las Condes, Moto Lavado, DestapeYa y Presidencia). Sirve para discutir con el equipo cómo va a funcionar el sistema antes de montarlo en ERPNext.

Es un solo archivo, `index.html`: se abre en cualquier navegador (teléfono o computadora) y no necesita servidor. Los datos se guardan en el propio navegador de quien lo usa.

## Cómo probarlo

1. Abrir `index.html`.
2. Arriba, en **Ver como**, elegir el perfil: Dueño, Administrador, Contabilidad, Gerente ventas, Vendedor · Walesca / Raúl, Cajero, Despacho · Jean Paul / Yonaiker.
3. En **Datos**: *en cero* para cargar facturas, cobros y gastos desde cero, o *de ejemplo* para ver el sistema con movimiento (cifras ilustrativas, no son los números reales de Profit).
4. **Día del demo** (−1 / +1 / +30) adelanta la fecha para ver vencimientos, alertas y quincenas.
5. **Reiniciar** borra todo lo cargado.

## Qué incluye

- **Facturación**: catálogo pre-venta, contado / financiado (40 % + 4 cuotas de 15 %) / crédito solo dueño, descuentos predefinidos con autorización, pagos mixtos (Zelle, Binance, Bs…), flete por destino, historial por vendedor.
- **Autorizaciones**: descuentos, anulaciones y pagos grandes; nadie ejecuta solo lo que afecta el dinero.
- **Financiamientos**: ficha por cliente, cuotas, alertas de vencimiento, comisión sobre lo cobrado.
- **Cuentas por cobrar y por pagar**: diseño del ERP de Robust (vencimientos 15/30, chips por tipo de tercero, fila por acreedor desplegable).
- **Despachos y servicios**: despachos disponibles que toman Jean Paul o Yonaiker, cobro de flete en sitio, servicio e instalación por línea de producto.
- **CRM · chats**: bandeja tipo Botinfy, cotizar y facturar desde la conversación.
- **Socios 50/50**: reparto automático por línea con la comisión a medias.
- **Nómina**: sueldo mensual en dos quincenas, comisiones, préstamos con planilla de cuotas, orden de pago en USDT → Bs.
- **Cuenta del accionista**: retiros y gastos personales como préstamo, cruce automático con deudas personales de trabajadores.
- **Administrador**: agenda del día, cierre de caja con arqueo, impuestos SENIAT, auditoría inmutable, límite de pagos.

## Estado

Demo funcional para validar reglas de negocio. El sistema real se monta en ERPNext (Frappe Cloud, `novax.s.frappe.cloud`) con una app propia, leyendo y migrando los datos desde Profit.
