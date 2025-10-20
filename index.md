---
layout: default
title: "Andrés Esquivel Díaz"
---

<style>
:root{
  --bg:#f8fafc; --ink:#0f172a; --muted:#475569;
  --brand:#1e3a8a; --brand2:#2563eb; --card:#ffffff;
  --shadow:0 2px 10px rgba(2,132,199,.10);
}
body{background:var(--bg);color:var(--ink);font-family:Inter,"Segoe UI",Roboto,sans-serif;line-height:1.7;}
h1,h2,h3,h4{color:var(--brand);margin:.4rem 0 1rem;}
.container{max-width:1100px;margin:0 auto;padding:1rem;}
.page-header{display:none!important;}
.section{margin:2.2rem 0;}
.card{background:var(--card);border-radius:14px;box-shadow:var(--shadow);padding:22px 26px;margin-bottom:1.6rem;}
.imgbox{margin:.8rem 0;border:1px solid #e5e7eb;border-radius:12px;overflow:hidden;}
.imgbox img{width:100%;height:auto;display:block;}
table{width:100%;border-collapse:collapse;margin:.8rem 0 1.2rem;font-size:.96rem;}
th,td{border:1px solid #e5e7eb;padding:.55rem .7rem;text-align:left;}
th{background:#eef2ff;color:#1e3a8a;}
ol,ul{margin-top:.3rem;padding-left:1.2rem;}
footer{text-align:center;color:#94a3b8;margin:2.5rem 0 1rem;}
.hero{
  display:flex;flex-direction:column;align-items:center;text-align:center;
  background:linear-gradient(90deg,#1e3a8a 0%,#2563eb 100%);
  color:#fff;padding:2.4rem 1rem 2rem;border-radius:0 0 26px 26px;box-shadow:0 6px 18px rgba(0,0,0,.08);
}
.hero img{width:120px;height:120px;border-radius:50%;object-fit:cover;margin-bottom:1rem;
  box-shadow:0 0 0 4px #fff,0 0 0 8px rgba(255,255,255,.35);}
.hero h1{color:#fff;font-weight:800;font-size:2rem;margin:.2rem 0;}
.hero p{color:#e2e8f0;margin:0;}
.hero .btns a{display:inline-block;padding:.55rem 1rem;margin:.3rem;border-radius:10px;background:#fff;
  color:#1e3a8a;text-decoration:none;font-weight:600;}
.hero .btns a:hover{background:#dbeafe;color:#1e40af;}
</style>

<!-- Banner -->
<div class="hero">
  <img src="assets/img/andy.jpg" alt="Foto de Andrés Esquivel Díaz">
  <h1>Andrés Esquivel Díaz</h1>
  <p>Data Analyst | Python · SQL · Tableau · A/B Testing</p>
  <div class="btns">
    <a href="https://www.linkedin.com/in/andres-esquivel-diaz-08691337/" target="_blank">LinkedIn</a>
    <a href="https://github.com/aesquivel91" target="_blank">GitHub</a>
    <a href="mailto:a_esquivel_69@hotmail.com">Email</a>
    <a href="#projects">Ver proyectos</a>
  </div>
</div>

<!-- Sobre mí -->
<div class="container section card" id="sobre-mi">
  <h2>Sobre mí</h2>
  <p>
    Soy <strong>Licenciado con certificación en Análisis de Datos</strong>, con una trayectoria de <strong>13+ años liderando operaciones, análisis y optimización de procesos</strong> en el sector hotelero de lujo.
  </p>
  <p>
    Combino la experiencia práctica en eficiencia, liderazgo y servicio con habilidades técnicas en <strong>Python, SQL, Excel y Tableau</strong>, aplicadas en proyectos de <strong>análisis exploratorio, pruebas A/B y visualización interactiva</strong>. Mi enfoque está en <strong>transformar datos en estrategias accionables</strong>, optimizar recursos y contar historias con datos que generen valor real para el negocio.
  </p>
</div>

<!-- Habilidades -->
<div class="container section card" id="habilidades">
  <h2>Habilidades</h2>
  <ul>
    <li>🐍 <strong>Python</strong> (pandas, numpy, matplotlib, seaborn, plotly)</li>
    <li>💾 <strong>SQL</strong> (joins, CTEs, KPIs, consultas optimizadas)</li>
    <li>📊 <strong>Tableau / Power BI / Excel avanzado</strong> — dashboards e informes ejecutivos</li>
    <li>🧠 <strong>A/B Testing y estadística</strong> (scipy, statsmodels)</li>
    <li>⚙️ <strong>Git, GitHub, Jupyter Notebook, Streamlit</strong></li>
  </ul>
</div>

<!-- Proyectos -->
<div class="container section" id="projects">
  <h2>Proyectos destacados</h2>

  <!-- Telecom -->
  <div class="card" id="telecom">
    <h3>📞 Telecomunicaciones: Identificar operadores ineficaces</h3>
    <p><strong>Objetivo:</strong> Detectar operadores ineficaces para decisiones de capacitación, redistribución de carga y dimensionamiento.</p>

    <h4>EDA:</h4>
    <p><strong>Preguntas guía</strong></p>
    <ol>
      <li>¿Cuántos operadores distintos existen?</li>
      <li>¿Cuántos clientes aparecen en llamadas vs. en la tabla maestra?</li>
      <li>¿Cómo se distribuye <em>direction</em> (in/out)?</li>
      <li>¿Qué porcentaje de llamadas es interna (<code>internal=True</code>)?</li>
      <li>¿Cuál es la tasa de llamadas perdidas en entrantes (<code>is_missed_call=True</code>)?</li>
      <li>¿Qué planes concentran mayor actividad?</li>
    </ol>

    <h4>EDA y limpieza inicial</h4>
    <ul>
      <li>Actividad de clientes: 307 de 732 tuvieron llamadas; 425 sin tráfico en el periodo.</li>
      <li>Operadores únicos: 1,093.</li>
      <li>Dirección de llamadas: 59% salientes / 41% entrantes.</li>
      <li>Naturaleza: 11% internas; resto externas.</li>
      <li>Missed rate (entrantes): 39.3%, nivel elevado → foco de mejora.</li>
      <li>Evolución temporal: crecimiento marcado; de &lt;1,000 al inicio a &gt;15,000 llamadas/día en oct–nov.</li>
      <li>Planes tarifarios: el Plan A concentra cerca de la mitad del volumen.</li>
      <li>Decisión de limpieza: imputar <code>internal</code> nulos como <code>False</code>.</li>
    </ul>

    <h4>Feature Engineering y KPIs</h4>
    <ul>
      <li>Se construyeron KPIs por operador: <code>missed_rate</code>, <code>avg_wait_time</code> y <code>out_calls</code>.</li>
      <li>Tras exigir ≥50 llamadas entrantes por operador, quedaron 438 operadores válidos.</li>
      <li>Descriptivos clave:
        <ul>
          <li><em>missed_rate</em> medio ≈ 23% (máx. 50%).</li>
          <li><em>avg_wait_time</em> medio ≈ 121 s; existen casos extremos &gt;15 min.</li>
          <li><em>out_calls</em> muy desigual: desde 0 hasta &gt;60k por operador.</li>
        </ul>
      </li>
      <li>Se detectaron registros sin <code>operator_id</code> (vacío) y se etiquetaron como “Unassigned”.</li>
    </ul>

    <h4>Gráficos — KPIs por operador</h4>
    <p><strong>1) Histograma de missed_rate</strong><br>
    • Distribución bimodal: muchos operadores cerca de 0.0 y otro grupo en 0.5.<br>
    • El pico en 0.5 está fuertemente asociado a “Unassigned” (llamadas sin operador).<br>
    <em>Interpretación:</em> conviven operadores con buen desempeño y un bloque afectado por problemas de asignación/enrutamiento.<br>
    <em>(agregar imagen KPI1.png)</em></p>

    <p><strong>2) Histograma de avg_wait_time (cap a 600 s)</strong><br>
    • Distribución sesgada a la derecha: la masa central está entre 20–120 s.<br>
    • Hay cola larga (≥300–600 s), indicador de ineficiencias puntuales y picos de carga.<br>
    <em>Implicación:</em> fijar SLA (p. ej., 80% &lt; 30 s) y alertas para operadores con &gt; 60 s sostenidos.<br>
    <em>(agregar imagen KPI2.png)</em></p>

    <p><strong>3) Histograma de out_calls (escala log)</strong><br>
    • Alta concentración en valores bajos (0–200) y pocos outliers muy altos.<br>
    • Sugiere roles distintos: gran parte casi no realiza outbound; unos pocos concentran campañas.<br>
    <em>Implicación:</em> documentar roles/expectativas y usar KPIs normalizados por tiempo/turno (p. ej., out_calls/día activo).<br>
    <em>(agregar imagen KPI3.png)</em></p>

    <p><strong>4) Dispersión missed_rate vs avg_wait_time</strong><br>
    • Dos bandas (≈0.0 y ≈0.5) y correlación débil e inversa.<br>
    • Un alto missed_rate no implica mayor espera: hay misses “rápidos” por abandono o enrutamiento.<br>
    <em>Implicación:</em> priorizar mejoras de enrutamiento y cobertura en picos antes de atribuirlo al desempeño individual.<br>
    <em>(agregar imagen KPI4.png)</em></p>

    <p><strong>5) Boxplot de out_calls por plan (A/B/C)</strong><br>
    • Medianas bajas con gran dispersión (ceros y outliers).<br>
    • Consistente con el análisis: Plan A &gt; Plan B en outbound; Plan C es heterogéneo.<br>
    <em>Implicación:</em> ajustar objetivos outbound por plan/rol, evitando comparaciones directas sin contexto.<br>
    <em>(agregar imagen KPI5.png)</em></p>

    <h4>Inefficiency Score</h4>
    <ul>
      <li>Se creó un índice ponderado:
        <ul>
          <li>0.4 * missed_rate_norm</li>
          <li>0.4 * wait_time_norm</li>
          <li>0.2 * (1 – out_calls_norm)</li>
        </ul>
      </li>
      <li>Umbral de ineficiencia: score &gt; 0.70 (ajustable según SLA/negocio).</li>
      <li>El Top 20 está dominado por registros “Unassigned”, con:
        <ul>
          <li>missed_rate cercano a 50%,</li>
          <li>esperas &gt; 1,000 s,</li>
          <li>muy pocas llamadas salientes.</li>
        </ul>
      </li>
      <li>Interpretación: el mayor foco de ineficacia responde a un problema de enrutamiento/asignación del sistema más que a bajo desempeño individual.</li>
      <li>Implicación operativa: priorizar la corrección de “Unassigned” y mantener el filtro de exposición mínima para evaluaciones justas por operador.</li>
    </ul>

    <h4>Pruebas de Hipótesis:</h4>
    <p><strong>H1:</strong> Operadores con mayor proporción de llamadas perdidas presentan mayor tiempo de espera promedio.<br>
    • <em>Prueba:</em> Spearman (correlación no paramétrica) entre missed_rate y avg_wait_time<br>
    <strong>Resultado:</strong><br>
    • <em>H1 — Missed rate vs. tiempo de espera</em><br>
    ρ = -0.132, p = 0.0058 → correlación significativa, débil e inversa.<br>
    <em>Interpretación:</em> más llamadas perdidas no implica esperas más largas; muchos “misses” parecen abandonos rápidos o fallas de enrutamiento.<br>
    <em>(Se agrega imagen H1.png)</em></p>

    <p><strong>H2:</strong> Operadores asignados a clientes con tarifa B realizan menos llamadas salientes que los de tarifa A.<br>
    • <em>Prueba:</em> Mann–Whitney U (dos colas, no paramétrica) sobre out_calls entre grupos A vs. B<br>
    <strong>Resultado:</strong><br>
    • <em>H2 — Outbound en Plan A vs. Plan B</em><br>
    p = 0.0005 → diferencia significativa.<br>
    <em>Conclusión:</em> operadores en Plan A realizan más llamadas salientes que en Plan B.<br>
    <em>(Se agrega imagen H2.png)</em></p>

    <p><strong>H3:</strong> El rendimiento de operadores difiere significativamente entre llamadas internas y externas (tiempo de espera).<br>
    • <em>Prueba:</em> Kruskal–Wallis (no paramétrica) sobre wait_time en entrantes internas vs. Externas<br>
    <strong>Resultado:</strong><br>
    • <em>H3 — Internas vs. externas (wait time)</em><br>
    p &lt; 0.0001 → diferencia significativa.<br>
    <em>Conclusión:</em> las llamadas externas presentan mayores tiempos de espera que las internas.<br>
    <em>(Se agrega imagen H3.png)</em></p>

    <h4>Hallazgos clave:</h4>
    <ol>
      <li><strong>Crecimiento de volumen</strong><br>
        • El tráfico aumentó con fuerza entre agosto y noviembre de 2019, con picos &gt;15k llamadas/día.<br>
        • Probable efecto de campañas intensivas o expansión acelerada de clientes.</li>
      <li><strong>Clientes y planes</strong><br>
        • Solo 307 de 732 clientes tuvieron actividad en el periodo.<br>
        • El Plan A concentra ~50% del volumen; le siguen C y B.</li>
      <li><strong>Eficiencia de operadores</strong><br>
        • De 1,093 operadores detectados, 438 cumplen la exposición mínima (≥50 entrantes).<br>
        • Missed rate promedio: 23% (alto).<br>
        • Tiempo de espera promedio: 121 s, con casos &gt;15 min.<br>
        • Out_calls: distribución muy desigual (de 0 a &gt;60k por operador).</li>
      <li><strong>Operadores ineficaces</strong><br>
        • El Inefficiency Score ubica un grupo crítico dominado por “Unassigned” (llamadas sin operador).<br>
        • Indica un problema de enrutamiento/asignación más que de desempeño individual.</li>
      <li><strong>Pruebas de hipótesis</strong><br>
        • H1: correlación significativa pero débil e inversa entre missed y espera (ρ = -0.132).<br>
        • H2: Plan A &gt; Plan B en llamadas salientes (p &lt; 0.001).<br>
        • H3: las externas presentan mayor espera que las internas (p &lt; 0.001).</li>
    </ol>

    <h4>Recomendaciones prácticas:</h4>
    <ul>
      <li>Corregir enrutamiento “Unassigned”. Principal foco de ineficacia y origen de gran parte de los misses.</li>
      <li>Capacitación focalizada. Coaching/redistribución para operadores con missed_rate &gt; 20% o avg_wait_time &gt; 60 s.</li>
      <li>Optimizar el Plan B. Alinear roles/objetivos outbound o revisar expectativas contractuales.</li>
      <li>Definir SLAs por plan. Ej.: 80% de llamadas atendidas en &lt; 30 s.</li>
      <li>Dimensionamiento de personal. Refuerzos en picos (oct–nov) y ajuste de turnos.</li>
      <li>Monitoreo continuo. Dashboard en Tableau con volumen diario, KPIs por operador y Watchlist.</li>
    </ul>
  </div>

  <!-- AB Test -->
  <div class="card" id="abtest">
    <h3>🅰️🅱️ AB Test — App Typography</h3>
    <p><strong>Objetivo:</strong> Detección de ineficiencias y missed calls por operador y routing. Reglas de enrutamiento y priorización para mejorar la calidad del servicio.</p>

    <h4>Preparación de los datos</h4>
    <p>Renombramos las columnas para que tengan nombres más descriptivos:</p>
    <ul>
      <li><code>event</code>: tipo de evento realizado</li>
      <li><code>user_id</code>: identificador único de usuario</li>
      <li><code>timestamp</code>: marca temporal en formato UNIX</li>
      <li><code>experiment</code>: ID del experimento (246 y 247 = control, 248 = prueba)</li>
    </ul>
    <p>También convertimos el timestamp a formato de fecha legible y separamos la fecha en una columna aparte.</p>

    <h4>Exploración general de los datos</h4>
    <ul>
      <li>Eventos totales: 244126</li>
      <li>Usuarios únicos: 7551</li>
      <li>Promedio de eventos por usuario: 32.33</li>
      <li>Rango de fechas: 2019-07-25 a 2019-08-07</li>
    </ul>
    <p><em>(agregar imagen AB1.png)</em></p>

    <h4>Completitud de los datos</h4>
    <p>Al analizar el histograma de eventos por fecha, se observa un cambio brusco a partir del 1 de agosto de 2019, donde el volumen de eventos supera los 10,000 diarios de forma consistente. Esto indica que los datos antes de esta fecha podrían estar incompletos o corresponder a pruebas. Por lo tanto, se considera como punto de partida confiable el 1 de agosto de 2019.</p>

    <h4>Impacto del filtrado</h4>
    <ul>
      <li>Eventos excluidos: 2,828</li>
      <li>Usuarios excluidos: 17</li>
    </ul>
    <p>La pérdida es mínima en relación al total, por lo que se justifica su eliminación para asegurar la calidad del análisis.</p>

    <h4>Verificación de grupos experimentales</h4>
    <ul>
      <li>Grupo 246 (Control A)</li>
      <li>Grupo 247 (Control A)</li>
      <li>Grupo 248 (Prueba B)</li>
    </ul>
    <p>Esto garantiza que el análisis del embudo de eventos y el test A/A/B puede continuar sin sesgos por datos incompletos.</p>

    <h4>Embudo:</h4>
    <p>Basándonos en los nombres de los eventos, se propone el siguiente orden secuencial:</p>
    <ol>
      <li>MainScreenAppear – pantalla principal</li>
      <li>OffersScreenAppear – usuario navega por ofertas</li>
      <li>CartScreenAppear – el usuario entra al carrito</li>
      <li>PaymentScreenSuccessful – pago exitoso</li>
    </ol>
    <p>Se calcula cuántos usuarios llegan a cada etapa y la conversión entre cada paso. Esto permite identificar en qué momento se pierden más usuarios.</p>
    <p><em>(agregar imagen grafico1.png)</em></p>

    <h4>Análisis del embudo de conversión</h4>
    <table>
      <thead><tr><th>Etapa</th><th style="text-align:right">Usuarios</th><th style="text-align:right">Conversión desde anterior</th><th style="text-align:right">Conversión desde inicio</th><th style="text-align:right">Caída desde anterior</th></tr></thead>
      <tbody>
        <tr><td>MainScreenAppear</td><td style="text-align:right">7,419</td><td style="text-align:right">-</td><td style="text-align:right">100%</td><td style="text-align:right">-</td></tr>
        <tr><td>OffersScreenAppear</td><td style="text-align:right">4,593</td><td style="text-align:right">61.9%</td><td style="text-align:right">61.9%</td><td style="text-align:right">38.1%</td></tr>
        <tr><td>CartScreenAppear</td><td style="text-align:right">3,734</td><td style="text-align:right">81.3%</td><td style="text-align:right">50.3%</td><td style="text-align:right">18.7%</td></tr>
        <tr><td>PaymentScreenSuccessful</td><td style="text-align:right">3,539</td><td style="text-align:right">94.8%</td><td style="text-align:right">47.7%</td><td style="text-align:right">5.2%</td></tr>
      </tbody>
    </table>
    <ul>
      <li>Mayor caída: ocurre al pasar de MainScreenAppear a OffersScreenAppear con una pérdida del 38.1%.</li>
      <li>Usuarios que completan todo el embudo: 47.7% desde la primera pantalla hasta el pago exitoso.</li>
    </ul>

    <h4>A/B:</h4>
    <p>Resultados del test A/B: comparación entre grupo experimental (248) y grupos de control (246 + 247). Se aplicó una prueba Z de proporciones para los cinco eventos principales. Aquí están los resultados:</p>
    <table>
      <thead><tr><th>Evento</th><th style="text-align:right">Grupo Experimental (%)</th><th style="text-align:right">Grupo Control (%)</th><th style="text-align:right">Z-Stat</th><th style="text-align:right">Valor p</th></tr></thead>
      <tbody>
        <tr><td>Tutorial</td><td style="text-align:right">11.00%</td><td style="text-align:right">11.23%</td><td style="text-align:right">-0.299</td><td style="text-align:right">0.7649</td></tr>
        <tr><td>MainScreenAppear</td><td style="text-align:right">98.27%</td><td style="text-align:right">98.58%</td><td style="text-align:right">-1.049</td><td style="text-align:right">0.2942</td></tr>
        <tr><td>OffersScreenAppear</td><td style="text-align:right">60.35%</td><td style="text-align:right">61.28%</td><td style="text-align:right">-0.782</td><td style="text-align:right">0.4343</td></tr>
        <tr><td>CartScreenAppear</td><td style="text-align:right">48.48%</td><td style="text-align:right">50.11%</td><td style="text-align:right">-1.335</td><td style="text-align:right">0.1818</td></tr>
        <tr><td>PaymentScreenSuccessful</td><td style="text-align:right">46.55%</td><td style="text-align:right">47.19%</td><td style="text-align:right">-0.524</td><td style="text-align:right">0.6004</td></tr>
      </tbody>
    </table>
    <p><strong>Conclusión:</strong> No se detectaron diferencias estadísticamente significativas (todos los valores p &gt; 0.05) entre el grupo experimental y los grupos de control combinados.</p>
    <p><em>(agregar imagen grafico2.png)</em></p>

    <h4>Visualización comparativa de comportamiento por grupo experimental</h4>
    <p>El gráfico anterior muestra la proporción de usuarios que realizaron cada uno de los eventos clave, separados por grupo experimental:</p>
    <ul>
      <li>Grupos 246 y 247: control (fuentes antiguas)</li>
      <li>Grupo 248: experimental (fuente nueva)</li>
    </ul>
    <p><strong>Observaciones clave:</strong></p>
    <ul>
      <li>Las proporciones son muy similares entre todos los grupos para cada evento.</li>
      <li>No se observan diferencias visuales significativas que indiquen un cambio en el comportamiento del usuario por la nueva fuente.</li>
      <li>Esto refuerza visualmente lo que ya fue demostrado estadísticamente en las pruebas Z.</li>
    </ul>
    <p><strong>Conclusión:</strong> El diseño con nueva fuente no afectó negativamente la experiencia de los usuarios en ninguna etapa del embudo ni en los eventos más comunes.</p>

    <h4>Significancia:</h4>
    <p>En este análisis se ha utilizado un nivel de significancia común de α = 0.05 para todas las pruebas de hipótesis estadísticas (Z-tests de proporciones). Esto significa que aceptamos un 5% de probabilidad de obtener un falso positivo por prueba.</p>
    <p><strong>¿Cuántas pruebas realizamos?</strong></p>
    <ul>
      <li>5 eventos entre grupos de control (test A/A)</li>
      <li>5 eventos entre grupo experimental y controles combinados (A/B)</li>
      <li>5 eventos entre grupo experimental y grupo 246</li>
      <li>5 eventos entre grupo experimental y grupo 247</li>
    </ul>
    <p>Total de pruebas realizadas: 20. Con α = 0.05, la probabilidad de tener al menos un falso positivo en 20 pruebas es considerable. Si se hubiera usado α = 0.10, entonces esperaríamos 2 falsos positivos en promedio, incluso si no existiera ningún efecto real.</p>
    <ul>
      <li>Si ninguna de las pruebas dio p &lt; 0.05 (como en este caso), no es necesario ajustar el nivel de significancia: los resultados son robustos.</li>
      <li>Si se hubieran detectado valores p &lt; 0.05, habría que aplicar una corrección por comparaciones múltiples, como:
        <ul>
          <li>Bonferroni: α ajustado = 0.05 / 20 = 0.0025</li>
          <li>Benjamini-Hochberg: más flexible, controla la tasa de falsos descubrimientos.</li>
        </ul>
      </li>
    </ul>

    <h4>Conclusión del Proyecto</h4>
    <ol>
      <li><strong>Embudo de conversión</strong><br>
        • Solo el 47.7% de los usuarios que inician su sesión llegan hasta la compra.<br>
        • La mayor pérdida se da entre la pantalla principal y la de ofertas (−38%), lo que sugiere una posible fricción o desinterés en esa etapa.</li>
      <li><strong>Validez del experimento (test A/A)</strong><br>
        • Los grupos de control (246 y 247) muestran resultados estadísticamente indistinguibles.<br>
        • Esto valida la asignación aleatoria y la confiabilidad del experimento A/B.</li>
      <li><strong>Impacto del cambio de fuente (grupo 248)</strong><br>
        • Se comparó el grupo experimental con los controles de forma combinada e individual.<br>
        • No se detectaron diferencias significativas en la proporción de usuarios que realizan los eventos clave.<br>
        • Se realizaron 20 pruebas estadísticas sin obtener falsos positivos (todos los valores p &gt; 0.05).</li>
    </ol>
    <p><strong>Conclusión final</strong><br>
    El cambio de fuente no tiene un impacto negativo en el comportamiento de los usuarios. Esto fue demostrado tanto visual como estadísticamente.<br>
    <strong>Recomendación:</strong> El equipo de diseño puede implementar el nuevo tipo de fuente con confianza. Se recomienda, sin embargo, investigar más a fondo la etapa de ofertas, donde se pierde el mayor porcentaje de usuarios.</p>
  </div>

  <!-- ICE -->
  <div class="card" id="ice">
    <h3>🎮 ICE — Análisis de Ventas de Videojuegos</h3>
    <p>Identificar los factores clave que determinan el éxito de un videojuego a partir de datos históricos de ventas, reseñas, plataformas, géneros y clasificación ESRB. Esto permitirá a Ice tomar decisiones estratégicas para campañas en 2017.</p>

    <h4>EDA:</h4>
    <ul>
      <li>Se convirtió <code>year_of_release</code> a numérico entero para permitir cálculos por año; muchos valores eran objetos por tener datos faltantes.</li>
      <li>La columna <code>user_score</code> contenía valores como "tbd", que fueron reemplazados con NaN para luego convertir todo a <em>float</em>.</li>
      <li>Convertí estas columnas para asegurar el análisis estadístico y gráfico con ellas.</li>
      <li>Eliminé filas sin <em>name</em> o <em>genre</em> porque son esenciales para identificar el juego y su clasificación.</li>
      <li>No rellené puntuaciones faltantes (<em>user_score</em>, <em>critic_score</em>) porque su ausencia probablemente indica que los juegos no fueron evaluados.</li>
      <li>Los valores 'tbd' fueron tratados como nulos apropiadamente.</li>
    </ul>

    <h4>Analísis de datos:</h4>
    <p><em>(agregar imagen game1.png)</em></p>
    <ul>
      <li>Observamos un fuerte crecimiento desde mediados de los 90s hasta un pico alrededor de 2008-2011.</li>
      <li>Desde 2012, la cantidad de lanzamientos parece disminuir.</li>
      <li>Los datos de 2016 pueden estar incompletos, por lo que el análisis predictivo se debería basar en datos hasta 2015.</li>
    </ul>

    <p><em>(agregar imagen ICE1.png, ICE2.png)</em></p>
    <ul>
      <li>Las plataformas con mayores ventas históricas son PS2, X360, PS3, Wii y DS.</li>
      <li>Algunas plataformas ya están obsoletas en 2016; el segundo gráfico muestra lo más vendible en el mercado actual.</li>
    </ul>

    <p><em>(agregar imagen ICE3.png)</em></p>
    <ul>
      <li>PS4 y XOne dominan claramente el mercado reciente, con ventas muy superiores a otras plataformas. <br>Estas deben ser el foco principal de campañas publicitarias y lanzamientos nuevos.</li>
      <li>3DS y WiiU mantienen una base de usuarios activa, especialmente en mercados como Japón (3DS). <br>Potenciales para nichos específicos o juegos portátiles.</li>
      <li>PSV (PlayStation Vita), aunque con menos ventas, muestra actividad y podría explotarse en regiones específicas o con títulos de nicho.</li>
      <li>PS2, PS3, X360 y Wii muestran ventas bajas o nulas en el periodo reciente, a pesar de haber sido líderes históricos. <br>Son plataformas obsoletas; deben evitarse en campañas nuevas o distribución de productos actuales.</li>
      <li>PC también muestra una caída en ventas de juegos físicos, lo que puede deberse al auge de distribución digital. <br>No debe descartarse del todo, pero su estrategia debe centrarse en digital.</li>
      <li>Otras plataformas clásicas (DS, PSP, GB, etc.) prácticamente no tienen ventas desde 2013. <br>Estas pueden eliminarse completamente del análisis estratégico para 2017.</li>
    </ul>

    <p><em>(agregar imagen game2.png)</em></p>
    <ul>
      <li>La mayoría de los juegos tienen ventas bajas (&lt;1 millón), pero hay muchos títulos con ventas extremadamente altas.</li>
      <li>Plataformas como Wii, PS2 y DS tuvieron juegos exitosos con ventas excepcionales.</li>
      <li>La dispersión sugiere que algunas plataformas producen grandes éxitos, pero la mayoría de los juegos tienen ventas modestas.</li>
    </ul>

    <p><em>(agregar imagen game3.png)</em></p>
    <ul>
      <li>Los géneros más rentables son Action, Sports, y Shooter, tanto por volumen como por total de ventas.</li>
      <li>Sin embargo, algunos géneros como Platform o Role-Playing también tienen grandes éxitos a pesar de menor cantidad de juegos.</li>
      <li>Géneros como Puzzle o Strategy tienen ventas más modestas.</li>
    </ul>

    <h4>Insights:</h4>
    <p><strong>Análisis de Datos:</strong></p>
    <ul>
      <li>Número de lanzamientos: El número de juegos creció hasta 2009 y luego decayó; los datos de 2016 están incompletos. Para analizar tendencias, se usaron datos hasta 2015.</li>
      <li>Plataformas líderes: PS2, X360 y Wii tienen mayores ventas históricas, pero para 2016 las plataformas más prometedoras son PS4, XOne y 3DS.</li>
      <li>Plataformas relevantes: Se priorizó el análisis de plataformas con mayores ventas recientes (2013–2016), no solo históricas, identificando a PS4, XOne, 3DS, WiiU y PSV como las más activas.</li>
      <li>Se identificaron plataformas en declive, como PS2, PS3, Wii y X360, mediante una gráfica comparativa de evolución de ventas.</li>
      <li>Ventas por género: Action, Shooter y Sports lideran en ventas. Sin embargo, Role-Playing muestra gran relevancia en Japón.</li>
      <li>Efecto de las reseñas: Existe correlación positiva entre puntuaciones de críticos y ventas (mayor que la de usuarios), aunque sigue siendo moderada.</li>
    </ul>

    <h4>Conclusión:</h4>
    <ul>
      <li>Priorizar plataformas activas y en crecimiento como PS4, XOne y 3DS para lanzamientos y campañas.</li>
      <li>Evitar plataformas en declive como PS2, PS3, Wii, X360, salvo en catálogos históricos o retro.</li>
      <li>Adaptar géneros y contenido según la región: Role-Playing para JP, Action y Sports para NA/EU.</li>
      <li>Dar mayor atención a las reseñas de críticos, ya que influyen más en las ventas que las de usuarios.</li>
    </ul>
  </div>
</div>

<footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>
