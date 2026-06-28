# 📊 De Datos a Decisiones: Caso de Negocio y Auditoría Estratégica Global

<blockquote>
 <h3>🚀 El Gancho Ejecutivo</h3>
 <p>Sistema de auditoría estratégica e inteligencia interactiva diseñado para la C-Suite con el fin de proteger el margen operativo, mitigar el riesgo de fuga en cuentas VIP y optimizar la inversión en la estrategia de expansión internacional. Una solución analítica completa que transforma más de 5 millones de registros comerciales crudos en directrices de negocio inmediatas.</p>
</blockquote>

---

## ☕ La Reunión Inicial: Cuando el Negocio Desafía al Dato

Todo comenzó con una de esas reuniones de lunes por la mañana que se alargan más de la cuenta. El **CEO** y el **CMO** me presentaron una lista de peticiones estándar. Querían gráficos limpios: ver la facturación mensual de 2011, saber cuáles eran los 10 países con más ingresos (sin contar Reino Unido) y conocer a sus 10 mejores clientes.

Pero decidí que no iba a limitarme a entregarles una serie de gráficos planos en pestañas. El reto real no era *"dibujar los datos"*, sino cruzarlos para responder a los verdaderos dolores de cabeza de la junta directiva.

### 🎯 Los Dolores de Cabeza de la C-Suite (Reto Corporativo)

*   **Sección 1: El Control del Negocio (Vista Global):** ¿Cómo aseguramos que la facturación total no dependa de un "producto milagro"? Necesitamos validar si el pronóstico del año entrante es lo suficientemente sostenible para respaldar el plan comercial actual.
*   **Sección 2: La Fuga de Clientes (Foco CRM & Marketing):** No basta con saber quiénes compran más. ¿Dónde se localiza exactamente la inactividad? ¿Estamos perdiendo cuentas críticas en el Top 10 histórico sin darnos cuenta?
*   **Sección 3: La Expansión Inteligente (Foco Operaciones):** ¿Cómo elegir el próximo mercado internacional basándonos en la rentabilidad real del ticket medio y no solo en un volumen de pedidos engañoso?

---

## 🖥️ Arquitectura del Caso y Soluciones Estratégicas

### 📊 Sección 1: Desempeño Comercial y Pronóstico Global
*Foco del CEO y CMO: Diagnóstico Macro y Resiliencia Temporal*

<p align="center">
  <img src="https://github.com/Elian-digital/powerbi-executive-analytics-case/blob/main/images/pagina-1.png?raw=true" alt="Desempeño Comercial y Pronóstico Global" width="90%">
</p>

*   **Mitigación del Riesgo Operativo:** Facturar **$9 mill.** repartidos en un catálogo de **3.780 SKUs** demuestra que el negocio goza de una excelente diversificación de ingresos; la estructura comercial no depende de productos estrella, blindando la estabilidad financiera ante variaciones en la demanda.
*   **Concentración en el Q4:** Los ingresos muestran estabilidad durante los primeros meses del año, experimentando una **aceleración exponencial en el último trimestre**. Este comportamiento marca el pico estacional crítico donde el CMO debe concentrar el presupuesto publicitario.
*   **Estabilidad del Pronóstico:** El modelo predictivo proyecta un comportamiento controlado y sostenible para el inicio de 2012, lo que valida la continuidad del plan estratégico vigente sin necesidad de aplicar ajustes presupuestarios drásticos.

---

### 👥 Sección 2: Análisis y Comportamiento de Clientes (CRM)
*Foco del CMO: Alertas de Abandono y Salud del Funnel*

<p align="center">
  <img src="https://github.com/Elian-digital/powerbi-executive-analytics-case/blob/main/images/pagina-2.png?raw=true" alt="Análisis y Comportamiento de Clientes" width="90%">
</p>

*   **Fuga en el Onboarding (Abandono Temprano):** La alta densidad de puntos rojos concentrados en la zona de baja frecuencia del gráfico de dispersión confirma que nuestro **43% de inactividad global (+60 días)** ocurre inmediatamente después de los primeros pedidos. El foco de marketing debe ser optimizar la experiencia de bienvenida y retención temprana.
*   **Rescate Crítico de Cuenta VIP:** El módulo de retención identificó que el cliente **ID 12346** —uno de nuestros diez compradores históricos más valiosos— se encuentra actualmente **inactivo**. Se requiere una intervención directa y personalizada del equipo de cuentas para reactivarlo antes de una pérdida definitiva.
*   **Identificación del 14% Anónimo:** Un **14% de los ingresos** proviene de transacciones sin registrar. Implementar incentivos de registro inmediato en el *checkout* es prioritario para capturar estos perfiles en el CRM y mitigar proactivamente su inactividad.

---

### 🌍 Sección 3: Estrategia de Expansión Global
*Foco del CEO: Maximización del Margen e Inversión Eficiente*

<p align="center">
  <img src="https://github.com/Elian-digital/powerbi-executive-analytics-case/blob/main/images/pagina-3.png?raw=true" alt="Estrategia de Expansión Global" width="90%">
</p>

*   **Prioridades de Expansión Premium:** **Australia y Singapur** se consolidan como los nichos más rentables debido a su elevado ticket medio (de hasta $2,5 mil). Representan una oportunidad óptima para expandir el negocio maximizando el margen con un bajo esfuerzo logístico.
*   **Aislamiento de Anomalías de Datos:** El análisis profundo detectó que el volumen de **Líbano ($1,7 mil)** es un indicador engañoso al depender de un **único pedido aislado**. Se descarta formalmente cualquier inversión de infraestructura en esta región por el alto riesgo de volatilidad.
*   **Estrategia Dual de Captación:** Se establece un plan de dos vías: mantener acciones de volumen para mercados consolidados como Países Bajos (91 pedidos / $3,0 mil de ticket medio) y desplegar captación selectiva para los nichos de alto margen detectados.

---

## 🛠️ Detrás de la Pantalla: Competencias y Back-End Técnico

Para que los directivos pudieran consumir estos insights con un solo vistazo en una sola vista *scannable*, fue necesario transformar por completo la estructura técnica de los datos crudos:

*   **Modelado Dimensional Avanzado (Star Schema):** La base de datos original venía integrada en una única tabla plana. Diseñé un modelo en estrella real, separando los datos lógicos en una tabla de hechos (`Fact_Sales`) vinculada a dimensiones limpias y optimizadas (`Dim_Customers`, `Dim_Products`, `Dim_Geography`).
*   **Limpieza de Datos e Integridad:** Apliqué transformaciones previas en el motor de datos para excluir registros erróneos (cantidades inferiores a 1 unidad, precios unitarios negativos y muchos errores de inventario), garantizando que las métricas finales de la C-Suite estuvieran libres de ruido operativo.
*   **Diseño de Interfaz Ejecutiva:** Implementé paneles de filtros desplegables y botones de navegación integrados. Esto eliminó las pestañas nativas inferiores de Power BI, logrando un lienzo limpio, de diseño corporativo, sofisticado y enfocado a la toma de decisiones.

---

## 💼 Habilidades Blandas Demostradas en este Caso

*   **Pensamiento Crítico Aplicado:** Capacidad de refutar peticiones iniciales básicas para proponer análisis cruzados de alto impacto (identificación de alertas de riesgo en lugar de simples rankings).
*   **Comunicación Ejecutiva:** Traducción directa de métricas densas de bases de datos a conclusiones de negocio claras para la toma de decisiones de la directiva.
*   **Proactividad Comercial:** Diseño de sistemas de alertas tempranas para proteger los activos más valiosos de la organización (clientes premium inactivos).
