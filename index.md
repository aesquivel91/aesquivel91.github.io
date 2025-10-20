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
table{width:100%;border-collapse:collapse;margin:.8rem 0 1.2rem;}
th,td{border:1px solid #e5e7eb;padding:.55rem .7rem;text-align:left;}
th{background:#eef2ff;color:#1e3a8a;}
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
    A lo largo de mi carrera confirmé que los datos no solo describen el pasado: <strong>explican el presente y orientan el futuro</strong>. Combino la experiencia operativa —eficiencia, liderazgo y servicio— con habilidades técnicas en <strong>Python, SQL, Excel y Tableau</strong>, aplicadas en proyectos de <strong>análisis exploratorio, pruebas A/B y visualización interactiva</strong>.
  </p>
  <p>
    Mi enfoque está en <strong>transformar datos en estrategias accionables</strong>, optimizar recursos y contar historias que generen valor tangible para el negocio.
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

    <h4>EDA — Preguntas guía</h4>
    <ol>
      <li>¿Cuántos operadores distintos existen?</li>
      <li>¿Cuántos clientes aparecen en llamadas vs. en la tabla maestra?</li>
      <li>¿Cómo se distribuye <em>direction</em> (in/out)?</li>
      <li>¿Qué porcentaje de llamadas es interna (<code>internal=True</code>)?</li>
      <li>¿Cuál es la tasa de llamadas perdidas (<code>is_missed_call=True</code>)?</li>
      <li>¿Qué planes concentran mayor actividad?</li>
    </ol>

    <p>El análisis inició con una exploración detallada de más de 700 clientes y 1,000 operadores. Los datos revelaron un <strong>missed rate del 39%</strong> y un crecimiento exponencial en el tráfico durante los meses pico (oct–nov). Se identificó al <strong>Plan A</strong> como el más activo, concentrando la mitad del volumen total.</p>

    <h4>Feature Engineering y KPIs</h4>
    <p>
      Se construyeron indicadores clave como <code>missed_rate</code>, <code>avg_wait_time</code> y <code>out_calls</code> para evaluar el desempeño individual de los operadores. Tras aplicar un filtro mínimo de exposición (≥50 llamadas entrantes), quedaron <strong>438 operadores válidos</strong>. Los resultados mostraron un <em>missed rate</em> promedio del 23%, tiempos de espera medios de 121 segundos y grandes diferencias en volumen de llamadas salientes (0 a más de 60 mil).
    </p>

    <div class="imgbox"><img src="assets/img/KPI1.png" alt="Histograma de missed rate"></div>
    <div class="imgbox"><img src="assets/img/KPI2.png" alt="Histograma de avg_wait_time"></div>
    <div class="imgbox"><img src="assets/img/KPI3.png" alt="Histograma de out_calls"></div>

    <h4>Inefficiency Score</h4>
    <p>
      Para sintetizar el rendimiento global se desarrolló un <strong>índice ponderado</strong> que combinó el <em>missed_rate</em>, el <em>wait_time</em> y las <em>out_calls</em>. Este <strong>Inefficiency Score</strong> permitió visualizar a los operadores menos eficientes, revelando que el mayor foco de ineficacia provenía de registros <strong>“Unassigned”</strong>, es decir, llamadas sin operador asignado.
    </p>

    <div class="imgbox"><img src="assets/img/H1.png" alt="Correlación Missed vs Tiempo"></div>
    <div class="imgbox"><img src="assets/img/H2.png" alt="Comparación Plan A vs B"></div>
    <div class="imgbox"><img src="assets/img/H3.png" alt="Internas vs Externas"></div>

    <h4>Hallazgos clave</h4>
    <ul>
      <li>El tráfico creció +1500% entre agosto y noviembre.</li>
      <li>El Plan A concentró el 50% de las llamadas activas.</li>
      <li>Se identificaron 438 operadores con exposición suficiente; el 23% presenta alto *missed rate*.</li>
      <li>El problema principal no es humano, sino de **enrutamiento** (operadores “Unassigned”).</li>
    </ul>

    <h4>Recomendaciones prácticas</h4>
    <ul>
      <li>Corregir el sistema de enrutamiento para eliminar llamadas “Unassigned”.</li>
      <li>Focalizar capacitaciones en operadores con *missed_rate* > 20%.</li>
      <li>Definir SLA claros (ej. 80% de llamadas atendidas en <30s).</li>
      <li>Implementar un dashboard en Tableau con monitoreo en tiempo real y alertas automáticas.</li>
    </ul>

    <p><strong>Stack:</strong> Python · pandas · seaborn · scipy · statsmodels  
    <a href="https://github.com/aesquivel91/telecom-inefficiency-analysis" target="_blank">→ Ver en GitHub</a></p>
  </div>

  <!-- A/B Test -->
  <div class="card" id="abtest">
    <h3>🅰️🅱️ AB Test — App Typography</h3>
    <p>
      Este experimento evaluó el impacto de un cambio tipográfico en la experiencia de usuario. A través de un test A/A/B se analizaron más de 240 mil eventos y 7,500 usuarios, buscando diferencias en conversión dentro del embudo de uso de una app.
    </p>

    <div class="imgbox"><img src="assets/img/grafico1.png" alt="Embudo de conversión"></div>
    <p>
      El embudo evidenció que el 47.7% de los usuarios completan la compra, con la mayor pérdida entre la pantalla principal y la sección de ofertas (-38%). Este hallazgo sugiere posibles puntos de fricción en la navegación o en la relevancia de las promociones.
    </p>

    <div class="imgbox"><img src="assets/img/grafico2.png" alt="Comparativa de grupos"></div>
    <p>
      Los resultados del test mostraron que no hubo diferencias estadísticamente significativas entre el grupo experimental (fuente nueva) y los grupos de control. Los valores p en todos los eventos fueron > 0.05, validando que el cambio no afectó negativamente el comportamiento de los usuarios.
    </p>

    <h4>Conclusión</h4>
    <p>
      El rediseño tipográfico no impactó de forma negativa el flujo de conversión, lo que permitió a los diseñadores implementarlo con confianza. La siguiente oportunidad de mejora identificada fue la optimización de la sección de ofertas, donde se concentra la mayor pérdida de usuarios.
    </p>

    <p><strong>Stack:</strong> Python · scipy · statsmodels · experimentación  
    <a href="https://github.com/aesquivel91/ab-test-app-typography" target="_blank">→ Ver en GitHub</a></p>
  </div>

  <!-- ICE -->
  <div class="card" id="ice">
    <h3>🎮 ICE — Análisis de Ventas de Videojuegos</h3>
    <p>
      Este proyecto analizó más de 16 años de ventas globales de videojuegos, evaluando factores como género, plataforma, puntuaciones y clasificación ESRB. El objetivo fue identificar los elementos que predicen el éxito comercial y orientar decisiones estratégicas para campañas futuras.
    </p>

    <div class="imgbox"><img src="assets/img/ICE1.png" alt="Evolución de lanzamientos"></div>
    <div class="imgbox"><img src="assets/img/ICE2.png" alt="Plataformas líderes"></div>
    <div class="imgbox"><img src="assets/img/ICE3.png" alt="Ventas por género"></div>

    <h4>Hallazgos principales</h4>
    <ul>
      <li>Las plataformas más prometedoras en 2016 fueron **PS4, XOne y 3DS**, mientras que PS2, PS3 y Wii entraron en declive.</li>
      <li>Los géneros **Action, Sports y Shooter** lideraron en ventas globales; **Role-Playing** destacó en Japón.</li>
      <li>Las reseñas de críticos mostraron una correlación positiva más fuerte con las ventas que las de usuarios.</li>
      <li>Las campañas futuras deberían enfocarse en plataformas activas y adaptar contenido según la región.</li>
    </ul>

    <p><strong>Stack:</strong> Python · pandas · plotly  
    <a href="#" title="Repositorio próximamente">→ Ver en GitHub</a></p>
  </div>
</div>

<footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>

