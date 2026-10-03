# 🤝 Gastos compartidos

Web app para dividir gastos compartidos en proporción justa: cargás lo que pagó cada uno, definís qué % le corresponde a cada persona (por ejemplo, según el sueldo) y la app calcula quién le debe a quién cada mes.

**Probala acá:** https://fabri-palumbo.github.io/gastos-compartidos/

## Qué hace

- Carga de gastos con cuotas y excepciones de división por gasto
- Cálculo del resultado mensual: quién le debe a quién
- Dashboard con KPIs, evolución del gasto y categorías top
- Historial con tabla dinámica y gráficos comparativos entre meses
- Compromisos futuros: cuánto queda por pagar en cuotas, mes a mes
- Botón "Probar con datos de ejemplo" para ver la app funcionando sin cargar nada

## Cómo se usa

1. Entrá a la app y tocá **"¿Cómo se usa la app?"** (guía paso a paso dentro de la misma app).
2. Poné los nombres en **Configuración** y creá tu primer mes con **➕ Nuevo mes**.
3. Cargá los gastos, mirá el resultado y, antes de cerrar, tocá **💾 Exportar JSON**.
4. La próxima vez, **📂 Importar JSON** y seguís donde lo dejaste.

> La app no guarda nada por su cuenta: si cerrás la pestaña sin exportar, se pierde lo cargado.

## Privacidad y seguridad

- **Tus datos no salen de tu navegador.** La app no tiene backend, no pide cuentas ni registro y no envía información a ningún servidor.
- **No usa APIs de pago ni claves.** No hay credenciales en el código.
- **El archivo JSON que exportás tiene todos tus gastos.** Guardalo como cualquier documento personal y no lo subas a lugares públicos.
- **Importá solo archivos propios.** Al importar, la app valida y normaliza los datos, y escapa todo el contenido antes de mostrarlo, para evitar que un archivo manipulado inyecte código.
- **Dependencias externas:** solo Chart.js y chartjs-plugin-datalabels, cargados desde cdnjs.

¿Encontraste un problema de seguridad o un bug? Abrí un [issue](https://github.com/fabri-palumbo/gastos-compartidos/issues) en este repositorio.

## Tecnología

HTML, CSS y JavaScript en un único archivo (`index.html`), sin build ni backend. Gráficos con [Chart.js](https://www.chartjs.org/).
