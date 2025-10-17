---
layout: default
title: "Andrés Esquivel Díaz"
---

<style>
/* ====== Estilo rápido y limpio para galería tipo malegoma ====== */
:root{
  --bg:#f7fafc; --ink:#0f172a; --muted:#64748b; --brand:#0ea5e9; --brand-2:#0284c7;
  --card:#ffffff; --shadow:0 1px 8px rgba(0,0,0,.08);
}
*{box-sizing:border-box;}
body{background:var(--bg); color:var(--ink);}
h1,h2,h3{margin:.2rem 0 1rem;}
.container{max-width:1000px; margin:0 auto; padding:1rem;}
.hero{ text-align:center; padding:2.5rem 1rem 1rem; }
.hero h1{font-size:2.2rem;}
.hero p{color:var(--muted);}
.btn-row a{
  display:inline-block; padding:.6rem 1rem; margin:.25rem .35rem;
  border-radius:10px; text-decoration:none; font-weight:700;
  background:var(--brand); color:#fff;
}
.btn-row a:hover{background:var(--brand-2);}
.section{margin:2.2rem 0;}
.badges a img{margin-right:6px; vertical-align:middle;}

.grid{display:grid; gap:18px; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));}
.card{
  background:var(--card); border-radius:14px; padding:16px; box-shadow:var(--shadow);
  transition: transform .15s ease, box-shadow .15s ease;
}
.card:hover{ transform: translateY(-4px); box-shadow:0 10px 24px rgba(2,132,199,.18);}
.thumb{ width:100%; height:160px; object-fit:cover; border-radius:10px; border:1px solid #e5e7eb;}
.small{ color:var(--muted); font-size:.96rem; line-height:1.45;}
.kpis{display:flex; gap:8px; flex-wrap:wrap; margin:.5rem 0 .2rem;}
.kpi{ background:#eef2f7; color:#334155; padding:4px 10px; border-radius:999px; font-size:.85rem;}
.meta{display:flex; justify-content:space-between; align-items:center; margin-top:.6rem;}
.meta .stack{ font-size:.85rem; color:#475569;}
.meta .links a{ text-decoration:none; font-weight:700; color:var(--brand);}
.meta .links a:hover{ color:var(--brand-2);}
footer{ text-align:center; color:#94a3b8; margin:2rem 0 1rem; }
</style>

<div class="container hero">
  <h1>Andrés Esquivel Díaz</h1>
  <p>Data Analyst — Python · SQL · Tableau · A/B Testing</p>
  <div class="badges">
    <a href="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white"><img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" alt="Python"></a>
    <a href="https://img.shields.io/badge/SQL-316192?logo=postgresql&logoColor=white"><img src="https://img.shields.io/badge/SQL-316192?logo=postgresql&logoColor=white" alt="SQL"></a>
    <a href="https://img.shields.io/badge/Tableau-E97627?logo=tableau&logoColor=white"><img src="https://img.shields.io/badge/Tableau-E97627?logo=tableau&logoColor=white" alt="Tableau"></a>
    <a href="https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white"><img src="https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white" alt="Jupyter"></a>
  </div>
  <div class="btn-row">
    <a href="https://www.linkedin.com/in/andres-esquivel-diaz-08691337/" target="_blank">LinkedIn</a>
    <a href="https://github.com/aesquivel91" target="_blank">GitHub</a>
    <a href="mailto:andresesquiveldata@gmail.com">Email</a>
    <a href="#projects">Ver proyectos</a>
  </div>
</div>

<div class="container">
 ## Sobre mí

Soy **Licenciado con certificación en Análisis de Datos**, con una trayectoria de **13+ años liderando operaciones, análisis y optimización de procesos** en el sector hotelero de lujo.  
Mi transición al mundo del análisis de datos surge del interés por **convertir la intuición operativa en decisiones respaldadas por evidencia**.

Combino la experiencia práctica en eficiencia, liderazgo y servicio con habilidades técnicas en **Python, SQL, Excel y Tableau**, aplicadas en proyectos de **análisis exploratorio, pruebas A/B y visualización interactiva**.  
Mi enfoque está en **transformar datos en estrategias accionables**, optimizar recursos y contar historias con datos que generen valor real para el negocio.


## Habilidades

**Lenguajes y herramientas técnicas**
- 🐍 Python (pandas, numpy, matplotlib, seaborn, plotly)
- 💾 SQL (consultas, joins, CTEs, KPIs desde bases relacionales)
- 📊 Tableau, Power BI y Excel avanzado (dashboards, storytelling con datos)
- 🧠 A/B Testing, análisis de hipótesis, estadística inferencial (scipy, statsmodels)
- ⚙️ Git, GitHub, Jupyter Notebook, Anaconda, Streamlit

**Competencias analíticas**
- Exploratory Data Analysis (EDA) para detectar patrones y oportunidades  
- Creación de reportes ejecutivos y métricas clave de negocio  
- Limpieza, transformación y validación de datos  
- Presentación de resultados con enfoque narrativo y visual

**Soft skills**
- Liderazgo y trabajo colaborativo  
- Comunicación clara con equipos multidisciplinarios  
- Atención al detalle, organización y pensamiento crítico


  ## Proyectos destacados {#projects}

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
        <div class="kpi">EDA</div><div class="kpi">Hipótesis</div><div class="kpi">Visualización</div>
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
        <div class="kpi">Embudo</div><div class="kpi">A/A/B</div><div class="kpi">Significancia</div>
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
        <div class="kpi">Streamlit</div><div class="kpi">EDA</div><div class="kpi">UI</div>
      </div>
      <div class="meta">
        <span class="stack">Python · Streamlit · pandas</span>
        <span class="links">
          <a href="https://github.com/aesquivel91/Aplicacion_Analisis_de_vehiculos_usados" target="_blank">GitHub</a>
        </span>
      </div>
    </div>

    <!-- 4) ICE (extraído de tu notebook) -->
    <div class="card">
      <img class="thumb" src="assets/img/ice.png" alt="ICE game sales">
      <h3>🎮 ICE — Análisis de Ventas de Videojuegos</h3>
      <p class="small">
        Ventas globales por género/plataforma, reseñas y ESRB para detectar patrones de éxito.  
        Recomendaciones de <em>mix</em> y segmentación regional.
      </p>
      <div class="kpis">
        <div class="kpi">EDA</div><div class="kpi">Segmentación</div><div class="kpi">Insight de mercado</div>
      </div>
      <div class="meta">
        <span class="stack">Python · pandas · plotly</span>
        <span class="links">
          <!-- Si ya tienes repo público del ICE, cámbialo aquí -->
          <a href="#" title="Repo próximamente">GitHub</a>
        </span>
      </div>
    </div>

  </div>

## Experiencia

### 🏨 Hospitalidad 
**Operations & Reservations Manager | 2010–2024**

- Dirigí equipos de hasta 20 colaboradores en operaciones y atención al cliente, garantizando **niveles de satisfacción superiores al 95%**.  
- Implementé controles de desempeño y reportes que redujeron **tiempos operativos en un 30%**.  
- Diseñé herramientas de seguimiento y análisis de KPIs para optimizar presupuestos y forecast de ocupación.  
- Coordiné estrategias entre departamentos (Rooms, Sales, F&B) aplicando un enfoque **data-driven** para la toma de decisiones.

### 🎯 Transición a Data Analytics (2025–Presente)
- Formación intensiva en **Python, SQL, estadística y visualización de datos** (TripleTen Bootcamp).  
- Desarrollo de proyectos aplicados como:
  - **Telecom Inefficiency Analysis:** detección de operadores ineficientes mediante análisis exploratorio.  
  - **AB Test App Typography:** evaluación del impacto visual en el embudo de conversión.  
  - **Aplicación de Análisis de Vehículos Usados:** app interactiva para explorar tendencias del mercado automotriz.

🚀 Actualmente enfocado en combinar mi **visión operativa estratégica** con el **análisis de datos**, para mejorar procesos, optimizar recursos y aportar valor analítico a decisiones de negocio.


  ---
  <footer>© 2025 Andrés Esquivel Díaz · Hecho con GitHub Pages</footer>
</div>
