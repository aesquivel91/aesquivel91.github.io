---
layout: default
title: "Andrés Esquivel Díaz"
---

<style>
/* ===== Reset del banner del theme ===== */
.page-header { display: none !important; }

/* ===== Paleta neutra + azul profesional ===== */
:root {
  --bg:#f8fafc; --ink:#0f172a; --muted:#475569;
  --brand:#1e3a8a; --brand2:#2563eb; --card:#ffffff;
  --shadow:0 2px 10px rgba(2,132,199,.10);
}
body {
  background: var(--bg);
  color: var(--ink);
  font-family: Inter, "Segoe UI", Roboto, sans-serif;
  line-height: 1.65;
}
h1,h2,h3,h4 { color: var(--brand); margin: .4rem 0 1rem; }
.container { max-width: 1100px; margin: 0 auto; padding: 1rem; }

/* ===== Hero ===== */
.hero {
  display: flex; flex-direction: column; align-items: center; text-align: center;
  background: linear-gradient(90deg, #1e3a8a 0%, #2563eb 100%);
  color: #fff; padding: 2.5rem 1rem 2rem;
  border-radius: 0 0 26px 26px;
  box-shadow: 0 6px 18px rgba(0,0,0,.08);
}
.hero img {
  width: 120px; height: 120px; border-radius: 50%;
  object-fit: cover;
  box-shadow: 0 0 0 4px #fff, 0 0 0 8px rgba(255,255,255,.3);
  margin-bottom: 1rem;
}
.hero h1 { color: #fff; font-weight: 800; font-size: 2rem; margin: .2rem 0; }
.hero p { color: #e2e8f0; margin: 0; }
.hero .btns a {
  display: inline-block; padding: .55rem 1rem; margin: .3rem;
  border-radius: 10px; background: #fff; color: var(--brand);
  text-decoration: none; font-weight: 600;
}
.hero .btns a:hover { background: #dbeafe; color: var(--brand2); }

/* ===== Secciones ===== */
.section { margin: 2.2rem 0; }
.card {
  background: var(--card); border-radius: 14px;
  box-shadow: var(--shadow); padding: 22px 26px;
}
ul, ol { margin-top: .4rem; padding-left: 1.2rem; }

/* ===== Proyectos ===== */
.project { margin-bottom: 2.5rem; }
.project h3 { font-size: 1.4rem; color: var(--brand2); }
.imgbox { margin: .8rem 0 1.2rem; border-radius: 12px; overflow: hidden; border: 1px solid #e5e7eb; }
.imgbox img { width: 100%; height: auto; display: block; }
.kpis { display:flex; gap:8px; flex-wrap:wrap; margin:.4rem 0 .6rem; }
.kpi { background:#e2e8f0; color:#1e293b; padding:4px 10px; border-radius:999px; font-size:.85rem; }
.meta { display:flex; justify-content:space-between; align-items:center; margin-top:.6rem; color:#475569; font-size:.95rem; }
.meta a { color:var(--brand2); text-decoration:none; font-weight:700; }
.meta a:hover { color:var(--brand); }

/* ===== Índice flotante ===== */
.toc {
  position: fixed; right: 20px; top: 40%; background: rgba(255,255,255,.9);
  border: 1px solid #cbd5e1; border-radius: 12px; padding: .8rem 1rem;
  box-shadow: var(--shadow); font-size: .9rem; line-height: 1.4;
}
.toc h4 { color: var(--brand); margin-bottom: .4rem; font-size: .95rem; }
.toc a { display: block; color: var(--muted); text-decoration: none; margin: .15rem 0; }
.toc a:hover { color: var(--brand2); }
footer { text-align:center; color:#94a3b8; margin:2.2rem 0 1rem; }
</style>

<!-- ===== Hero ===== -->
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

<!-- ===== Índice flotante ===== -->
<div class="toc">
  <h4>Secciones</h4>
  <a href="#sobre-mi">Sobre mí</a>
  <a href="#habilidades">Habilidades</a>
  <a href="#projects">Proyectos</a>
  <a href="#telecom">📞 Telecom</a>
  <a href="#abtest">🅰️🅱️ A/B Test</a>
  <a href="#ice">🎮 ICE Games</a>
</div>

<!-- ===== SOBRE MÍ ===== -->
<div class="container section card" id="sobre-mi">
  <h2>Sobre mí</h2>
  <p>
    Soy <strong>Licenciado con certificación en Análisis de Datos</strong>, con más de <strong>13 años de experiencia liderando operaciones,
    análisis y optimización de procesos</strong> en el sector hotelero de lujo.
  </p>
  <p>
    Mi transición al mundo del <strong>Data Analytics</strong> surge del deseo de transformar la intuición operativa en decisiones
    basadas en evidencia. Combino mi visión estratégica, enfoque en eficiencia y liderazgo con habilidades técnicas en <strong>Python, SQL,
    Excel y Tableau</strong> para resolver problemas complejos, encontrar patrones ocultos y traducir datos en <strong>acciones medibles y rentables</strong>.
  </p>
  <p>
    Mi objetivo es <strong>impulsar la toma de decisiones data-driven</strong>, optimizar recursos y crear narrativas visuales que
    conecten los datos con la estrategia de negocio.
  </p>
</div>

<!-- ===== HABILIDADES ===== -->
<div class="container section card" id="habilidades">
  <h2>Habilidades</h2>
  <ul>
    <li>🐍 <strong>Python</strong> — pandas, numpy, matplotlib, seaborn, plotly</li>
    <li>💾 <strong>SQL</strong> — joins, CTEs, KPIs y consultas optimizadas</li>
    <li>📊 <strong>Tableau / Power BI / Excel avanzado</strong> — dashboards, storytelling y reportes ejecutivos</li>
    <li>🧠 <strong>A/B Testing y estadística</strong> — scipy, statsmodels, pruebas Z, U, Kruskal–Wallis</li>
    <li>⚙️ <strong>Git, GitHub, Jupyter Notebook, Streamlit</strong></li>
  </ul>
</div>

<!-- ===== PROYECTOS ===== -->
<div class="container section" id="projects">
  <h2>Proyectos destacados</h2>

  <!-- Proyecto 1 -->
  <div class="project card" id="telecom">
    <h3>📞 Telecomunicaciones — Detección de operadores ineficaces</h3>
    <p>
      <strong>Objetivo:</strong> Identificar operadores ineficaces para orientar decisiones de capacitación, redistribución de carga y optimización del servicio.
    </p>
    <p>
      Se realizó un <strong>análisis exploratorio (EDA)</strong> sobre más de 700 clientes y 1,000 operadores, evaluando llamadas entrantes, salientes y tiempos de espera.
      A través de pruebas estadísticas (Spearman, Mann–Whitney U, Kruskal–Wallis) se determinaron patrones de desempeño e ineficiencia.
    </p>

    <h4>Visualizaciones</h4>
    <div class="imgbox"><img src="assets/img/H1.png" alt="Missed rate vs tiempo de espera"></div>
    <div class="imgbox"><img src="assets/img/H2.png" alt="Outbound Plan A vs Plan B"></div>
    <div class="imgbox"><img src="assets/img/H3.png" alt="Internas vs externas wait time"></div>

    <h4>Principales hallazgos</h4>
    <ul>
      <li>El tráfico de llamadas creció significativamente entre agosto y noviembre de 2019, superando 15k llamadas diarias.</li>
      <li>Solo 307 de 732 clientes mostraron actividad; el <strong>Plan A</strong> concentró cerca del 50% del volumen total.</li>
      <li>El <strong>missed rate promedio fue 23%</strong> y el tiempo medio de espera 121 s, revelando áreas críticas de mejora.</li>
      <li>Los registros “Unassigned” explican gran parte de la ineficiencia, evidenciando problemas de enrutamiento.</li>
    </ul>

    <h4>Impacto y recomendaciones</h4>
    <ul>
      <li>Reconfigurar el enrutamiento y reducir la proporción de llamadas sin operador asignado.</li>
      <li>Capacitación focalizada en operadores con tasas de espera altas (&gt;60s) o missed_rate &gt;20%.</li>
      <li>Definir <strong>SLAs específicos</strong> por plan de cliente (ej. 80% llamadas atendidas &lt;30s).</li>
      <li>Implementar dashboard en Tableau para monitoreo continuo y alertas.</li>
    </ul>

    <div class="meta">
      <span>Python · pandas · seaborn · scipy</span>
      <span><a href="https://github.com/aesquivel91/telecom-inefficiency-analysis" target="_blank">Ver en GitHub</a></span>
    </div>
  </div>

  <!-- Proyecto 2 -->
  <div class="project card" id="abtest">
    <h3>🅰️🅱️ A/B Test — App Typography</h3>
    <p>
      <strong>Objetivo:</strong> Evaluar si un cambio en la tipografía de una aplicación afecta el comportamiento de los usuarios a lo largo del embudo de conversión.
    </p>
    <p>
      Se diseñó un <strong>test A/A/B</strong> con más de 2,400 usuarios para medir diferencias entre grupos de control y experimental.
      Se analizaron eventos clave: navegación, carrito y pago exitoso, mediante pruebas Z de proporciones.
    </p>

    <h4>Embudo de conversión</h4>
    <div class="imgbox"><img src="assets/img/grafico1.png" alt="Embudo conversión"></div>

    <h4>Resultados</h4>
    <div class="imgbox"><img src="assets/img/grafico2.png" alt="Resultados A/B"></div>
    <p>
      No se observaron diferencias estadísticamente significativas (<em>p&gt;0.05</em>) entre grupos, confirmando la estabilidad del rendimiento tras el cambio visual.
    </p>

    <h4>Conclusión e impacto</h4>
    <ul>
      <li>El cambio de tipografía no afecta negativamente el flujo de usuarios ni la conversión final.</li>
      <li>El equipo de diseño puede <strong>implementar el nuevo estilo</strong> sin riesgo para las métricas clave.</li>
      <li>Se recomienda profundizar en la etapa de <em>OffersScreen</em>, donde se detecta mayor abandono.</li>
    </ul>

    <div class="meta">
      <span>Python · scipy · statsmodels · A/B Testing</span>
      <span><a href="https://github.com/aesquivel91/ab-test-app-typography" target="_blank">Ver en GitHub</a></span>
    </div>
  </div>

  <!-- Proyecto 3 -->
  <div class="project card" id="ice">
    <h3>🎮 ICE — Análisis de ventas de videojuegos</h3>
    <p>
      <strong>Objetivo:</strong> Identificar los factores que determinan el éxito de un videojuego a partir de datos históricos de ventas, reseñas, plataformas y géneros.
      Este estudio orienta las decisiones estratégicas de la tienda <em>Ice</em> para campañas comerciales en 2017.
    </p>

    <h4>Exploración y limpieza de datos</h4>
    <p>
      Se transformaron columnas clave (<code>year_of_release</code>, <code>user_score</code>) para permitir análisis estadístico.
      Se eliminaron filas con valores faltantes en nombre o género, garantizando consistencia en los resultados.
    </p>

    <h4>Segmentación y visualización</h4>
    <ul>
      <li><strong>PS4</strong> y <strong>XOne</strong> lideran el mercado reciente; deben ser el foco de nuevas campañas.</li>
      <li><strong>3DS</strong> y <strong>WiiU</strong> mantienen relevancia en Japón; oportunidades en nichos portátiles.</li>
      <li><strong>PC</strong> muestra caída en ventas físicas por digitalización; adaptar estrategia al formato online.</li>
    </ul>

    <div class="imgbox"><img src="assets/img/ICE1.png" alt="Ventas por plataforma"></div>
    <div class="imgbox"><img src="assets/img/ICE2.png" alt="Tendencias por género"></div>
    <div class="imgbox"><img src="assets/img/ICE3.png" alt="Ventas regionales"></div>

    <h4>Conclusiones e insights</h4>
    <ul>
      <li>Las plataformas activas y en crecimiento (PS4, XOne, 3DS) deben concentrar la inversión publicitaria.</li>
      <li>Los géneros <strong>Action, Shooter y Sports</strong> son los más rentables en NA y EU; <strong>Role-Playing</strong> domina en Japón.</li>
      <li>Las reseñas de críticos correlacionan más con ventas que las de usuarios → priorizar prensa especializada.</li>
      <li>Las plataformas en declive (PS2, PS3, Wii, X360) deben reservarse para catálogos retro.</li>
    </ul>

    <div class="meta">
      <span>Python · pandas · plotly</span>
      <span><a href="#" title="Repositorio próximamente">GitHub</a></span>
    </div>
  </div>
</div>

<footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>

