---
layout: default
title: "Andrés Esquivel Díaz"
---

<style>
/* Oculta el banner del theme Cayman */
.page-header{ display:none !important; }

/* Paleta neutros + azules */
:root{
  --bg:#f8fafc; --ink:#0f172a; --muted:#475569;
  --brand:#1e3a8a; --brand2:#3b82f6; --card:#ffffff;
  --shadow:0 1px 10px rgba(2,132,199,.10);
}
*{box-sizing:border-box;}
body{background:var(--bg); color:var(--ink); font-family: Inter, "Segoe UI", Roboto, sans-serif; line-height:1.6;}
h1,h2,h3{color:var(--brand); margin:.4rem 0 1rem;}
.container{max-width:1100px; margin:0 auto; padding:1rem;}

/* Banner propio */
.hero{
  display:flex; flex-direction:column; align-items:center; text-align:center;
  background:linear-gradient(90deg, #1e3a8a 0%, #3b82f6 100%); color:#fff;
  padding:2.2rem 1rem 1.6rem; border-radius:0 0 26px 26px;
  box-shadow:0 6px 18px rgba(0,0,0,.08);
}
.hero img{width:120px; height:120px; border-radius:50%; object-fit:cover;
  box-shadow:0 0 0 4px #fff, 0 0 0 8px rgba(255,255,255,.35); margin-bottom:1rem;}
.hero h1{color:#fff; font-weight:800; font-size:2rem; margin:.2rem 0;}
.hero p{color:#e2e8f0; margin:0;}
.hero .btns a{
  display:inline-block; padding:.55rem 1rem; margin:.35rem .35rem; border-radius:10px;
  background:#fff; color:#1e3a8a; text-decoration:none; font-weight:600;
}
.hero .btns a:hover{background:#dbeafe; color:#1e40af;}

/* Secciones y tarjetas */
.section{margin:2.2rem 0;}
.card{background:var(--card); border-radius:14px; box-shadow:var(--shadow); padding:18px 18px;}
.grid{display:grid; gap:18px; grid-template-columns:repeat(auto-fit,minmax(300px,1fr));}
.kpis{display:flex; gap:8px; flex-wrap:wrap; margin:.4rem 0 .6rem;}
.kpi{background:#e2e8f0; color:#1e293b; padding:4px 10px; border-radius:999px; font-size:.85rem;}
.meta{display:flex; justify-content:space-between; align-items:center; margin-top:.6rem; color:#475569; font-size:.95rem;}
.meta a{color:var(--brand2); text-decoration:none; font-weight:700;}
.meta a:hover{color:var(--brand);}
.imgbox{margin:.6rem 0 1rem; border:1px solid #e5e7eb; border-radius:12px; overflow:hidden; background:#fff;}
.imgbox img{width:100%; height:auto; display:block;}
ul{margin-top:.4rem;}
/* Tablas simples */
table{width:100%; border-collapse:collapse; margin:.5rem 0 1rem; font-size:.95rem;}
th,td{border:1px solid #e5e7eb; padding:.55rem .6rem; text-align:left;}
th{background:#eef2ff; color:#1e3a8a;}
footer{text-align:center; color:#94a3b8; margin:2.2rem 0 1rem;}
</style>

<!-- Hero -->
<div class="hero">
  <img src="assets/img/andy.jpg" alt="Foto de Andrés Esquivel Díaz">
  <h1>Andrés Esquivel Díaz</h1>
  <p>Data Analyst | Python · SQL · Tableau · A/B Testing</p>
  <div class="btns">
    <a href="https://www.linkedin.com/in/andres-esquivel-diaz-08691337/" target="_blank">LinkedIn</a>
    <a href="https://github.com/aesquivel91" target="_blank">GitHub</a>
    <a href="mailto:andresesquiveldata@gmail.com">Email</a>
    <a href="#projects">Ver proyectos</a>
  </div>
</div>

<!-- Sobre mí -->
<div class="container section card">
  <h2>Sobre mí</h2>
  <p>
    Soy <strong>Licenciado con certificación en Análisis de Datos</strong>, con una trayectoria de
    <strong>13+ años liderando operaciones, análisis y optimización de procesos</strong> en el sector hotelero de lujo.
  </p>
  <p>
    Combino la experiencia práctica en eficiencia, liderazgo y servicio con habilidades técnicas en <strong>Python, SQL, Excel y Tableau</strong>,
    aplicadas en proyectos de <strong>análisis exploratorio, pruebas A/B y visualización interactiva</strong>. Mi enfoque está en
    <strong>transformar datos en estrategias accionables</strong>, optimizar recursos y contar historias con datos que generen valor real para el negocio.
  </p>
</div>

<!-- Habilidades -->
<div class="container section card">
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

  <!-- Proyecto 1: Telecom -->
  <div class="card" id="telecom">
    <h3>📞 Telecomunicaciones: Identificar operadores ineficaces</h3>
    <p><strong>Objetivo:</strong> Detectar operadores ineficaces para decisiones de capacitación, redistribución de carga y dimensionamiento.</p>

    <h4>EDA — Preguntas guía</h4>
    <ol>
      <li>¿Cuántos operadores distintos existen?</li>
      <li>¿Cuántos clientes aparecen en llamadas vs. en la tabla maestra?</li>
      <li>¿Cómo se distribuye <em>direction</em> (in/out)?</li>
      <li>¿Qué porcentaje de llamadas es interna (<code>internal=True</code>)?</li>
      <li>¿Cuál es la tasa de llamadas perdidas en entrantes (<code>is_missed_call=True</code>)?</li>
      <li>¿Qué planes concentran mayor actividad?</li>
    </ol>

    <h4>Hipótesis</h4>
    <ul>
      <li><strong>H1:</strong> Operadores con mayor proporción de llamadas perdidas presentan mayor tiempo de espera promedio.  
        <em>Prueba:</em> Spearman entre <code>missed_rate</code> y <code>avg_wait_time</code>.</li>
      <li><strong>H2:</strong> Operadores asignados a clientes con tarifa B realizan menos llamadas salientes que los de tarifa A.  
        <em>Prueba:</em> Mann–Whitney U sobre <code>out_calls</code> (A vs. B).</li>
      <li><strong>H3:</strong> El rendimiento difiere entre llamadas internas y externas (tiempo de espera).  
        <em>Prueba:</em> Kruskal–Wallis sobre <code>wait_time</code> (internas vs. externas).</li>
    </ul>

    <h4>Visualización</h4>
    <div class="imgbox"><img src="assets/img/H1.png" alt="H1 — Missed rate vs tiempo de espera"></div>
    <div class="imgbox"><img src="assets/img/H2.png" alt="H2 — Outbound en Plan A vs Plan B"></div>
    <div class="imgbox"><img src="assets/img/H3.png" alt="H3 — Internas vs Externas (wait time)"></div>

    <h4>Hallazgos clave</h4>
    <ul>
      <li><strong>Crecimiento de volumen:</strong> picos &gt;15k llamadas/día (ago–nov 2019).</li>
      <li><strong>Clientes y planes:</strong> 307 de 732 clientes con actividad; Plan A ≈ 50% del volumen.</li>
      <li><strong>Eficiencia:</strong> 1,093 operadores; 438 con ≥50 entrantes. Missed rate prom. 23%, espera media 121 s.</li>
      <li><strong>Ineficacia:</strong> “Unassigned” concentra gran parte de los misses → problema de enrutamiento.</li>
      <li><strong>Pruebas:</strong> H1 ρ = −0.132; H2 A &gt; B en salientes (p &lt; .001); H3 externas &gt; internas (p &lt; .001).</li>
    </ul>

    <h4>Recomendaciones prácticas</h4>
    <ul>
      <li>Corregir enrutamiento “Unassigned”.</li>
      <li>Coaching a operadores con <code>missed_rate &gt; 20%</code> o <code>avg_wait_time &gt; 60s</code>.</li>
      <li>Optimizar el Plan B (roles/objetivos outbound).</li>
      <li>Definir SLAs por plan (p.ej., 80% atendidas &lt; 30s).</li>
      <li>Dimensionamiento por picos (oct–nov) y turnos.</li>
      <li>Dashboard en Tableau con KPIs por operador + Watchlist.</li>
    </ul>

    <div class="meta">
      <span>Python · pandas · seaborn · scipy · statsmodels</span>
      <span><a href="https://github.com/aesquivel91/telecom-inefficiency-analysis" target="_blank">GitHub</a></span>
    </div>
  </div>

  <!-- Proyecto 2: A/B Typography -->
  <div class="card" id="abtest">
    <h3>🅰️🅱️ AB Test — App Typography</h3>
    <p><strong>Objetivo:</strong> Detección de ineficiencias y missed calls por operador y routing. Reglas de enrutamiento y priorización para mejorar la calidad del servicio.</p>

    <h4>Embudo</h4>
    <p>Orden de eventos:</p>
    <ol>
      <li><code>MainScreenAppear</code> – pantalla principal</li>
      <li><code>OffersScreenAppear</code> – navegación de ofertas</li>
      <li><code>CartScreenAppear</code> – carrito</li>
      <li><code>PaymentScreenSuccessful</code> – pago exitoso</li>
    </ol>
    <p>Se calcula la llegada a cada etapa y la conversión entre pasos (identificación de fuga). </p>
    <div class="imgbox"><img src="assets/img/grafico1.png" alt="Embudo de conversión"></div>

    <h4>A/B</h4>
    <p>Comparación entre grupo experimental (248) y controles (246 + 247). Prueba Z de proporciones en 5 eventos:</p>
    <table>
      <thead>
        <tr>
          <th>Evento</th><th>Experimental (%)</th><th>Control (%)</th><th>Z-Stat</th><th>p-value</th>
        </tr>
      </thead>
      <tbody>
        <tr><td>Tutorial</td><td>11.00%</td><td>11.23%</td><td>-0.299</td><td>0.7649</td></tr>
        <tr><td>MainScreenAppear</td><td>98.27%</td><td>98.58%</td><td>-1.049</td><td>0.2942</td></tr>
        <tr><td>OffersScreenAppear</td><td>60.35%</td><td>61.28%</td><td>-0.782</td><td>0.4343</td></tr>
        <tr><td>CartScreenAppear</td><td>48.48%</td><td>50.11%</td><td>-1.335</td><td>0.1818</td></tr>
        <tr><td>PaymentScreenSuccessful</td><td>46.55%</td><td>47.19%</td><td>-0.524</td><td>0.6004</td></tr>
      </tbody>
    </table>
    <p><strong>Conclusión:</strong> No hay diferencias estadísticamente significativas (todos p &gt; .05).</p>
    <div class="imgbox"><img src="assets/img/grafico2.png" alt="Resultados A/B"></div>

    <h4>Significancia</h4>
    <p>Se usó <strong>α = 0.05</strong>. Se realizaron 20 pruebas (A/A y A/B). Como ningún p &lt; .05, no se requiere corrección por múltiples comparaciones. Si hubiera habido significancia, usar: Bonferroni (α/20) o Benjamini–Hochberg.</p>

    <h4>Conclusión</h4>
    <p>El cambio de fuente no impacta negativamente el comportamiento de usuarios. </p>

    <h4>Recomendación</h4>
    <p>Se puede implementar el nuevo tipo de fuente con confianza. Investigar más la etapa de <em>Offers</em>, que concentra la mayor fuga.</p>

    <div class="meta">
      <span>Python · scipy · statsmodels</span>
      <span><a href="https://github.com/aesquivel91/ab-test-app-typography" target="_blank">GitHub</a></span>
    </div>
  </div>

  <!-- Proyecto 3: ICE -->
  <div class="card" id="ice">
    <h3>🎮 ICE — Análisis de Ventas de Videojuegos</h3>
    <p><strong>Objetivo:</strong> Identificar factores de éxito (ventas, reseñas, plataformas, géneros, ESRB) para decisiones estratégicas en 2017.</p>

    <h4>EDA</h4>
    <ul>
      <li>Conversión de <code>year_of_release</code> a entero; limpieza de <code>user_score</code> (“tbd” → NaN → float).</li>
      <li>Eliminación de filas sin <em>name</em> o <em>genre</em>; no se imputaron <em>scores</em> ausentes.</li>
      <li>Tratamiento de datos faltantes para permitir análisis estadístico y gráfico correcto.</li>
    </ul>

    <h4>Segmentación</h4>
    <ul>
      <li><strong>PS4</strong> y <strong>XOne</strong> dominan el mercado reciente → foco de campañas y lanzamientos.</li>
      <li><strong>3DS/WiiU</strong> activos en nichos (JP). <strong>PSV</strong> con potencial específico.</li>
      <li>Plataformas históricas (PS2, PS3, X360, Wii) en declive → evitar para campañas nuevas.</li>
      <li><strong>PC</strong>: caída en ventas físicas (auge digital) → priorizar estrategia digital.</li>
    </ul>

    <div class="imgbox"><img src="assets/img/ICE1.png" alt="ICE gráfico 1"></div>
    <div class="imgbox"><img src="assets/img/ICE2.png" alt="ICE gráfico 2"></div>
    <div class="imgbox"><img src="assets/img/ICE3.png" alt="ICE gráfico 3"></div>

    <h4>Insights</h4>
    <ul>
      <li>Lanzamientos crecieron hasta 2009; análisis de tendencias con datos hasta 2015 por incompletitud 2016.</li>
      <li>Históricamente lideran PS2, X360 y Wii; en 2016 las más prometedoras: PS4, XOne y 3DS.</li>
      <li>Ventas por género: Action, Shooter y Sports dominan; en JP pesa Role-Playing.</li>
      <li>Críticos influyen más que usuarios (correlación positiva moderada con ventas).</li>
      <li>Perfiles regionales: NA/EU prefieren consolas domésticas; JP portátiles y RPG.</li>
    </ul>

    <h4>Conclusión</h4>
    <ul>
      <li>Priorizar PS4, XOne y 3DS para 2017.</li>
      <li>Evitar plataformas en declive salvo catálogo retro.</li>
      <li>Adaptar géneros por región (RPG en JP; Action/Sports en NA/EU).</li>
      <li>Dar más peso a reseñas de críticos en la estrategia comercial.</li>
    </ul>

    <div class="meta">
      <span>Python · pandas · plotly</span>
      <span><a href="#" title="Repo próximamente">GitHub</a></span>
    </div>
  </div>
</div>

<footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>
