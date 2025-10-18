---
layout: default
title: "Andrés Esquivel Díaz"
---

<style>
/* ====== Estilo profesional neutro y azul ====== */
:root {
  --bg: #f8fafc;
  --ink: #0f172a;
  --muted: #475569;
  --brand: #1e3a8a;       /* Azul oscuro profesional */
  --brand-light: #3b82f6; /* Azul brillante */
  --card: #ffffff;
  --shadow: 0 1px 8px rgba(0,0,0,.08);
}

* { box-sizing: border-box; }
body {
  background: var(--bg);
  color: var(--ink);
  font-family: 'Inter', 'Segoe UI', Roboto, sans-serif;
  line-height: 1.6;
}

h1, h2, h3 {
  margin: .5rem 0 1rem;
}

.container {
  max-width: 1000px;
  margin: 0 auto;
  padding: 1rem;
}

/* === HERO SECTION === */
.hero {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 3rem 1rem 2rem;
  background: linear-gradient(180deg, #e0f2fe 0%, #ffffff 100%);
  border-bottom: 3px solid var(--brand-light);
  border-radius: 0 0 20px 20px;
}

.hero img {
  width: 140px;
  height: 140px;
  border-radius: 50%;
  object-fit: cover;
  box-shadow: 0 0 0 4px #fff, 0 0 0 8px var(--brand-light);
  margin-bottom: 1rem;
}

.hero h1 {
  font-size: 2.3rem;
  font-weight: 800;
  color: var(--brand);
  margin-bottom: .3rem;
}

.hero p {
  color: var(--muted);
  font-size: 1.1rem;
  margin-bottom: 1rem;
}

.btn-row a {
  display: inline-block;
  padding: .6rem 1.1rem;
  margin: .3rem .35rem;
  border-radius: 10px;
  text-decoration: none;
  font-weight: 600;
  background: var(--brand);
  color: #fff;
  transition: all 0.2s ease;
}

.btn-row a:hover {
  background: var(--brand-light);
}

/* === GRID & CARDS === */
.grid {
  display: grid;
  gap: 18px;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
}

.card {
  background: var(--card);
  border-radius: 14px;
  padding: 16px;
  box-shadow: var(--shadow);
  transition: transform .15s ease, box-shadow .15s ease;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 10px 24px rgba(30,58,138,.15);
}

.thumb {
  width: 100%;
  height: 160px;
  object-fit: cover;
  border-radius: 10px;
  border: 1px solid #e2e8f0;
}

.small {
  color: var(--muted);
  font-size: .96rem;
  line-height: 1.45;
}

.kpis {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
  margin: .5rem 0 .2rem;
}

.kpi {
  background: #e2e8f0;
  color: #1e293b;
  padding: 4px 10px;
  border-radius: 999px;
  font-size: .85rem;
}

.meta {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: .6rem;
}

.meta .stack {
  font-size: .85rem;
  color: #475569;
}

.meta .links a {
  text-decoration: none;
  font-weight: 700;
  color: var(--brand);
}

.meta .links a:hover {
  color: var(--brand-light);
}

footer {
  text-align: center;
  color: #64748b;
  margin: 2.5rem 0 1rem;
  font-size: .9rem;
}
</style>

<div class="container hero">
  <h1>Andrés Esquivel Díaz</h1>
  <p>Data Analyst — Python · SQL · Tableau · A/B Testing</p>
  <div class="badges">
    <a href="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
      <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" alt="Python">
    </a>
    <a href="https://img.shields.io/badge/SQL-316192?logo=postgresql&logoColor=white">
      <img src="https://img.shields.io/badge/SQL-316192?logo=postgresql&logoColor=white" alt="SQL">
    </a>
    <a href="https://img.shields.io/badge/Tableau-E97627?logo=tableau&logoColor=white">
      <img src="https://img.shields.io/badge/Tableau-E97627?logo=tableau&logoColor=white" alt="Tableau">
    </a>
    <a href="https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white">
      <img src="https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white" alt="Jupyter">
    </a>
  </div>
  <div class="btn-row">
    <a href="https://www.linkedin.com/in/andres-esquivel-diaz-08691337/" target="_blank">LinkedIn</a>
    <a href="https://github.com/aesquivel91" target="_blank">GitHub</a>
    <a href="mailto:a_esquivel_69@hotmail.com">Email</a>
    <a href="#projects">Ver proyectos</a>
  </div>
</div>

<div class="container">
  <h2>Sobre mí</h2>
  <p>
    Soy <strong>Licenciado con certificación en Análisis de Datos</strong>, con una trayectoria de
    <strong>13+ años liderando operaciones, análisis y optimización de procesos</strong> en el sector hotelero de lujo.
    Mi transición al mundo del análisis de datos surge del interés por
    <strong>convertir la intuición operativa en decisiones respaldadas por evidencia</strong>.
  </p>
  <p>
    Combino la experiencia práctica en eficiencia, liderazgo y servicio con habilidades técnicas en
    <strong>Python, SQL, Excel y Tableau</strong>, aplicadas en proyectos de
    <strong>análisis exploratorio, pruebas A/B y visualización interactiva</strong>.
    Mi enfoque está en <strong>transformar datos en estrategias accionables</strong>, optimizar recursos y contar
    historias con datos que generen valor real para el negocio.
  </p>

  <h2>Habilidades</h2>
  <h3>Lenguajes y herramientas técnicas</h3>
  <ul>
    <li>🐍 Python (pandas, numpy, matplotlib, seaborn, plotly)</li>
    <li>💾 SQL (consultas, joins, CTEs, KPIs desde bases relacionales)</li>
    <li>📊 Tableau, Power BI y Excel avanzado (dashboards, storytelling con datos)</li>
    <li>🧠 A/B Testing, análisis de hipótesis, estadística inferencial (scipy, statsmodels)</li>
    <li>⚙️ Git, GitHub, Jupyter Notebook, Anaconda, Streamlit</li>
  </ul>

  <h3>Competencias analíticas</h3>
  <ul>
    <li>Exploratory Data Analysis (EDA) para detectar patrones y oportunidades</li>
    <li>Creación de reportes ejecutivos y métricas clave de negocio</li>
    <li>Limpieza, transformación y validación de datos</li>
    <li>Presentación de resultados con enfoque narrativo y visual</li>
  </ul>

  <h3>Soft skills</h3>
  <ul>
    <li>Liderazgo y trabajo colaborativo</li>
    <li>Comunicación clara con equipos multidisciplinarios</li>
    <li>Atención al detalle, organización y pensamiento crítico</li>
  </ul>

  <h2 id="projects">Proyectos destacados</h2>

  <div class="grid">
    <!-- 1) TELECOM -->
    <div class="card">
      <img class="thumb" src="assets/img/telecom.png" alt="Telecom">
      <h3>📞 Telecom Inefficiency Analysis</h3>
      <p class="small">
        Detección de ineficiencias y <em>missed calls</em> por operador y routing.
        Reglas de enrutamiento y priorización para mejorar la calidad del servicio.
      </p>
      <div class="kpis">
        <div class="kpi">EDA</div>
        <div class="kpi">Hipótesis</div>
        <div class="kpi">Visualización</div>
      </div>
      <div class="meta">
        <span class="stack">Python · pandas · seaborn</span>
        <span class="links">
          <a href="https://github.com/aesquivel91/telecom-inefficiency-analysis" target="_blank">GitHub</a>
        </span>
      </div>
    </div>

    <!-- 2) A/B TYPOGRAPHY -->
    <div class="card">
      <img class="thumb" src="assets/img/abtest.png" alt="A/B Typography">
      <h3>🅰️🅱️ AB Test — App Typography</h3>
      <p class="small">
        Test A/A/B para evaluar el impacto tipográfico en el embudo de conversión.
        Resultados estables sin detrimento de métricas, con validación estadística.
      </p>
      <div class="kpis">
        <div class="kpi">Embudo</div>
        <div class="kpi">A/A/B</div>
        <div class="kpi">Significancia</div>
      </div>
      <div class="meta">
        <span class="stack">Python · scipy · statsmodels</span>
        <span class="links">
          <a href="https://github.com/aesquivel91/ab-test-app-typography" target="_blank">GitHub</a>
        </span>
      </div>
    </div>

    <!-- 3) APP VEHÍCULOS -->
    <div class="card">
      <img class="thumb" src="assets/img/cars.png" alt="Used cars app">
      <h3>🚗 Aplicación Análisis de Vehículos Usados</h3>
      <p class="small">
        App en Streamlit para explorar listados de autos usados en EE.UU.
        Filtros por precio, año y marca para detectar patrones e insights de mercado.
      </p>
      <div class="kpis">
        <div class="kpi">Streamlit</div>
        <div class="kpi">EDA</div>
        <div class="kpi">UI</div>
      </div>
      <div class="meta">
        <span class="stack">Python · Streamlit · pandas</span>
        <span class="links">
          <a href="https://github.com/aesquivel91/Aplicacion_Analisis_de_vehiculos_usados" target="_blank">GitHub</a>
        </span>
      </div>
    </div>

    <!-- 4) ICE -->
    <div class="card">
      <img class="thumb" src="assets/img/ice.png" alt="ICE game sales">
      <h3>🎮 ICE — Análisis de Ventas de Videojuegos</h3>
      <p class="small">
        Ventas globales por género/plataforma, reseñas y ESRB para detectar patrones de éxito.
        Recomendaciones de <em>mix</em> y segmentación regional.
      </p>
      <div class="kpis">
        <div class="kpi">EDA</div>
        <div class="kpi">Segmentación</div>
        <div class="kpi">Insight de mercado</div>
      </div>
      <div class="meta">
        <span class="stack">Python · pandas · plotly</span>
        <span class="links">
          <!-- Cambia el href cuando publiques el repo del ICE -->
          <a href="#" title="Repo próximamente">GitHub</a>
        </span>
      </div>
    </div>
  </div>

  <h2>Experiencia</h2>

  <h3>🏨 Hospitalidad</h3>
  <p><strong>Operations & Reservations Manager | 2010–2024</strong></p>
  <ul>
    <li>Dirigí equipos de hasta 20 colaboradores en operaciones y atención al cliente, logrando <strong>95%+ de satisfacción</strong>.</li>
    <li>Implementé reportes y controles que redujeron <strong>tiempos operativos en 30%</strong>.</li>
    <li>Diseñé KPIs para optimizar presupuestos y forecast de ocupación.</li>
    <li>Coordiné estrategias entre Rooms, Sales y F&amp;B con enfoque <strong>data-driven</strong>.</li>
  </ul>

  <h3>🎯 Transición a Data Analytics (2025–Presente)</h3>
  <ul>
    <li>Formación intensiva en <strong>Python, SQL, estadística y visualización</strong> (TripleTen).</li>
    <li>Proyectos: <em>Telecom Inefficiency Analysis</em>, <em>AB Test App Typography</em>,
      <em>Aplicación de Análisis de Vehículos Usados</em>.</li>
  </ul>

  <hr>
  <footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>
</div>
