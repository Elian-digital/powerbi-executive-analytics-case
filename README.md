# 📊 De Datos a Decisiones: Auditoría Estratégica Global · Caso Tata C-Suite

> **El CEO y el CMO me pidieron gráficos. Les entregué un sistema de alertas.**

💡 *Caso desarrollado en la Tata Data Visualization Job Simulation ([Forage](https://www.theforage.com/simulations/tata/data-visualisation-p5xo)), resolviendo requerimientos analíticos reales de los roles de liderazgo de Tata Insights Group.*

---

## ☕ La Reunión Inicial

Todo comenzó con una de esas reuniones de lunes por la mañana que se alargan más de la cuenta. El CEO y el CMO presentaron una lista de peticiones estándar: ver la facturación mensual de 2011, los 10 países con más ingresos y el ranking de mejores clientes.

Decidí no limitarme a entregar gráficos planos en pestañas. El reto real no era *dibujar los datos*, sino cruzarlos para responder a los verdaderos dolores de cabeza de la junta directiva.

### Los tres problemas que no habían formulado todavía

- **Control del negocio:** ¿La facturación depende de algún producto estrella? ¿El pronóstico del año siguiente aguanta el plan comercial actual?
- **Fuga de clientes:** ¿Estamos perdiendo cuentas críticas del Top 10 histórico sin darnos cuenta?
- **Expansión inteligente:** ¿Cómo elegir el próximo mercado internacional basándonos en margen real y no en volumen de pedidos engañoso?

---

## 📊 Lo que encontré

### Sección 1: El negocio está diversificado pero tiene un pico crítico

<p align="center">
  <img src="https://github.com/Elian-digital/powerbi-executive-analytics-tata-job-simulation/blob/main/images/pagina-1.png?raw=true" width="90%">
</p>

Facturar **$9M** repartidos en **3.780 SKUs** demuestra que no hay dependencia de productos estrella, nuestra estructura financiera es resistente. Pero los ingresos se aceleran exponencialmente en el Q4: ahí es donde el CMO debe concentrar el presupuesto. El modelo predictivo confirma un inicio de 2012 estable, sin necesidad de ajustes drásticos.

### Sección 2: El 14% del revenue es anónimo y uno de los Top 10 ya no compra

<p align="center">
  <img src="https://github.com/Elian-digital/powerbi-executive-analytics-tata-job-simulation/blob/main/images/pagina-2.png?raw=true" width="90%">
</p>

El cliente **ID 12346** (uno de los diez compradores históricos más valiosos) está inactivo. Requiere intervención directa antes de una pérdida definitiva. Además, el **43% de inactividad global** ocurre en los primeros pedidos: el problema no es la retención a largo plazo, es el onboarding. Y un **14% de ingresos** viene de transacciones sin registrar en CRM, clientes invisibles que no se pueden retener porque no existen en el sistema.

### Sección 3: Australia y Singapur, sí. Líbano, no

<p align="center">
  <img src="https://github.com/Elian-digital/powerbi-executive-analytics-tata-job-simulation/blob/main/images/pagina-3.png?raw=true" width="90%">
</p>

**Australia y Singapur** tienen el ticket medio más alto (hasta $2,5K) con volumen suficiente para justificar inversión. **Líbano** aparece con $1,7K de ticket pero depende de un único pedido aislado, por lo que queda descartado por riesgo de volatilidad. La estrategia de expansión es dual: volumen en mercados consolidados (Países Bajos: 91 pedidos / $3K ticket) y captación selectiva en los nichos de alto margen.

---

## 🛠️ Backend Técnico

- **Modelado Dimensional:** La base de datos original era una única tabla plana. Diseñé un Star Schema real: `Fact_Sales` + dimensiones limpias (`Dim_Customers`, `Dim_Products`, `Dim_Geography`).
- **Limpieza de datos:** Exclusión de registros erróneos (cantidades < 1 unidad, precios negativos, errores de inventario) para garantizar que los KPIs de la C-Suite estuvieran libres de ruido.
- **Diseño de interfaz ejecutiva:** Paneles de filtros desplegables y navegación integrada que eliminan las pestañas nativas de Power BI; lienzo limpio, corporativo, orientado a decisión.

---

### 🤝 Contacto
- **LinkedIn:** [linkedin.com/in/eliandaghoum](https://www.linkedin.com/in/eliandaghoum/)
- **Email:** eliandaghoum@gmail.com
- **GitHub:** [@Elian-digital](https://github.com/Elian-digital)
