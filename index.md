---
layout: default
title: "Andrés Esquivel Díaz"
---

<style>
/* ====== Elimina el banner del theme Cayman ====== */
.page-header { display: none !important; }

/* ====== Banner personalizado azul neutro ====== */
.hero-banner {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  background: linear-gradient(90deg, #1e3a8a 0%, #3b82f6 100%);
  color: white;
  padding: 2.5rem 1rem 1.8rem;
  border-radius: 0 0 30px 30px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.hero-banner img {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 1rem;
  box-shadow: 0 0 0 4px #fff, 0 0 0 6px rgba(255,255,255,0.3);
}

.hero-banner h1 {
  font-size: 2rem;
  font-weight: 800;
  margin: 0.4rem 0;
  color: #ffffff;
}

.hero-banner p {
  font-size: 1rem;
  color: #e2e8f0;
  margin: 0;
}

.hero-buttons {
  margin-top: 1rem;
}

.hero-buttons a {
  display: inline-block;
  padding: 0.6rem 1rem;
  margin: 0.3rem;
  border-radius: 8px;
  background: #ffffff;
  color: #1e3a8a;
  font-weight: 600;
  text-decoration: none;
  transition: background 0.2s ease, color 0.2s ease;
}

.hero-buttons a:hover {
  background: #dbeafe;
  color: #1e40af;
}
</style>

<!-- ====== HERO BANNER ====== -->
<div class="hero-banner">
  <img src="assets/img/andy.jpg" alt="Foto de Andrés Esquivel Díaz">
  <h1>Andrés Esquivel Díaz</h1>
  <p>Data Analyst | Python · SQL · Tableau · A/B Testing</p>
  <div class="hero-buttons">
    <a href="https://www.linkedin.com/in/andres-esquivel-diaz-08691337/" target="_blank">LinkedIn</a>
    <a href="https://github.com/aesquivel91" target="_blank">GitHub</a>
    <a href="mailto:a_esquivel_69@hotmail.com">Email</a>
    <a href="#projects">Ver proyectos</a>
    </div>
</div>


<!-- ======== SOBRE MÍ ======== -->
<div class="container">
  <h2>Sobre mí</h2>
  <p>
    Soy <strong>Licenciado con certificación en Análisis de Datos</strong>, con una trayectoria de <strong>13+ años liderando operaciones,          análisis y optimización de procesos</strong> en el sector hotelero de lujo.  
 <p>
    Combino la experiencia práctica en eficiencia, liderazgo y servicio con habilidades técnicas en <strong>Python, SQL, Excel y                    Tableau</strong>, aplicadas en proyectos de <strong>análisis exploratorio, pruebas A/B y visualización interactiva</strong>.  
    Mi enfoque está en <strong>transformar datos en estrategias accionables</strong>, optimizar recursos y contar historias con datos que           generen valor real para el negocio.
  </p>
  <p>
    Combino habilidades técnicas en <strong>Python, SQL, Excel y Tableau</strong> con un enfoque estratégico orientado a la eficiencia.
    Me apasiona contar historias con datos, descubrir oportunidades de mejora y respaldar decisiones con evidencia cuantitativa.
  </p>
</div>

<!-- ======== HABILIDADES ======== -->
<div class="container">
  <h2>Habilidades</h2>
  <ul>
    <li>🐍 <strong>Python</strong> (pandas, numpy, matplotlib, seaborn, plotly)</li>
    <li>💾 <strong>SQL</strong> (joins, CTEs, KPIs, consultas optimizadas)</li>
    <li>📊 <strong>Tableau / Power BI / Excel avanzado</strong> — dashboards e informes ejecutivos</li>
    <li>🧠 <strong>A/B Testing y estadística</strong> (scipy, statsmodels)</li>
    <li>⚙️ <strong>Git, GitHub, Jupyter Notebook, Streamlit</strong></li>
  </ul>
</div>

<!-- ======== PROYECTOS ======== -->
<div class="container">
  <h2 id="projects">Proyectos destacados</h2>

  <div class="grid">
    <!-- 1) TELECOM -->
    <div class="card">
      <h3>📞 Telecom Inefficiency Analysis</h3>
      <p class="small">
        Detección de ineficiencias y <em>missed calls</em> por operador y routing.
        Reglas de enrutamiento y priorización para mejorar la calidad del servicio.
      </p>
      <div class="kpis">
        <div class="kpi">EDA</div><div class="kpi">Hipótesis</div><div class="kpi">Visualización</div>
      </div>
      <div class="meta">
        <span class="stack">Python · pandas · seaborn</span>
        <span class="links"><a href="https://github.com/aesquivel91/telecom-inefficiency-analysis" target="_blank">GitHub</a></span>
      </div>
    </div>

    <!-- 2) A/B TYPOGRAPHY -->
    <div class="card">
      <h3>🅰️🅱️ AB Test — App Typography</h3>
      <p class="small">
        Test A/A/B para evaluar el impacto tipográfico en el embudo de conversión.
        Resultados estables sin detrimento de métricas, con validación estadística.
      </p>
      <div class="kpis">
        <div class="kpi">Embudo</div><div class="kpi">A/B</div><div class="kpi">Significancia</div>
      </div>
      <div class="meta">
        <span class="stack">Python · scipy · statsmodels</span>
        <span class="links"><a href="https://github.com/aesquivel91/ab-test-app-typography" target="_blank">GitHub</a></span>
      </div>
    </div>

    <!-- 3) VEHÍCULOS -->
    <div class="card">
      <h3>🚗 Aplicación Análisis de Vehículos Usados</h3>
      <p class="small">
        App interactiva en Streamlit que permite explorar listados de autos usados en EE.UU.
        Filtros por precio, año y marca para descubrir patrones de mercado.
      </p>
      <div class="kpis">
        <div class="kpi">Streamlit</div><div class="kpi">EDA</div><div class="kpi">UI</div>
      </div>
      <div class="meta">
        <span class="stack">Python · Streamlit · pandas</span>
        <span class="links"><a href="https://github.com/aesquivel91/Aplicacion_Analisis_de_vehiculos_usados" target="_blank">GitHub</a></span>
      </div>
    </div>

    <!-- 4) ICE -->
    <div class="card">
      <h3>🎮 ICE — Análisis de Ventas de Videojuegos</h3>
      <p class="small">
        Ventas globales por género y plataforma, reseñas y ESRB para detectar patrones de éxito.
        Recomendaciones de <em>mix</em> y segmentación regional.
      </p>
      <div class="kpis">
        <div class="kpi">EDA</div><div class="kpi">Segmentación</div><div class="kpi">Insights</div>
      </div>
      <div class="meta">
        <span class="stack">Python · pandas · plotly</span>
        <span class="links"><a href="#" title="Repo próximamente">GitHub</a></span>
      </div>
    </div>
  </div>
</div>

<!-- ======== EXPERIENCIA ======== -->
<div class="container">
  <h2>Experiencia</h2>

  <h3>🏨 Hospitalidad</h3>
  <p><strong>Operations & Reservations Manager | 2010–2024</strong></p>
  <ul>
    <li>Dirigí equipos de hasta 20 colaboradores, logrando <strong>95%+ de satisfacción</strong>.</li>
    <li>Implementé reportes que redujeron <strong>tiempos operativos en 30%</strong>.</li>
    <li>Diseñé KPIs para forecast y control presupuestal.</li>
    <li>Coordiné estrategias entre áreas con enfoque <strong>data-driven</strong>.</li>
  </ul>

  <h3>🎯 Transición a Data Analytics (2025–Presente)</h3>
  <ul>
    <li>Formación intensiva en <strong>Python, SQL, estadística y visualización</strong> (TripleTen Bootcamp).</li>
    <li>Desarrollo de proyectos: <em>Telecom Inefficiency</em>, <em>AB Test Typography</em>, <em>Vehículos Usados</em>.</li>
  </ul>
</div>

<footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>

