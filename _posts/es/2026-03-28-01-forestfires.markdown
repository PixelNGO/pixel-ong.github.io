---
title: Detección satelital de incendios y quemas en Patagonia
lang: es
subtitle: ''
layout: default
modal-id: 4
date: 2026-03-28
img: ''
thumbnail: alerces-after-thumbnail.png
alt: ''
project-date: Marzo 2026
client: Interno
category: Monitoreo Ambiental
description: "Los incendios en Patagonia son una problemática ambiental creciente, con un aumento sostenido en su frecuencia y magnitud en los últimos años. El fenómeno responde a múltiples causas (naturales y antrópicas) y sus efectos se ven agravados por el cambio climático y por el recorte presupuestario en las herramientas de prevención y manejo del fuego. En este contexto, desde Píxel aportamos a la identificación de las áreas de vegetación quemada durante el verano 2025-2026 y estimamos la severidad de los incendios en la zona del Parque y la Reserva Nacional Los Alerces y sus alrededores (provincia de Chubut, Argentina), a partir de información satelital. Los resultados muestran que la superficie de vegetación afectada por incendios (mayoritariamente bosques) alcanzó 42.500 ha, lo que equivale a cerca del 4% de la superficie del Parque Nacional y al 14% de la Reserva.
<br>
<br>
Nuestro enfoque combinó fuentes satelitales diversas, incluyendo datos ópticos multiespectrales y productos derivados del infrarrojo térmico. Para delimitar el área de vegetación afectada por los incendios utilizamos en primer lugar los focos de calor (potenciales incendios) registrados entre el 25 de noviembre de 2025 y el 10 de marzo de 2026, obtenidos del sistema FIRMS de la NASA. Luego, calculamos el Índice Normalizado de Área Quemada (NBR por sus siglas en inglés) en imágenes Sentinel-2 adquiridas por la European Space Agency, correspondientes al momento anterior (25/11/2025) y el posterior a los incendios (10/03/2026). El NBR se calcula como la relación entre los valores de la banda del infrarrojo cercano (NIR) y del infrarrojo de onda corta (SWIR) y permite resaltar las áreas afectadas por el fuego en incendios de gran extensión. A continuación, calculamos el diferencial del NBR (dNBR), el cual representa el cambio en la vegetación entre ambas fechas. Así, valores más altos de dNBR indican una mayor severidad del daño a la vegetación . Finalmente, para mejorar la estimación de la vegetación afectada eliminamos las zonas con sombras y nubes mediante la banda SCL de las imágenes Sentinel-2, así como las zonas no vegetadas a partir del mapa de coberturas y uso de suelo de MapBiomas del año 2024 (Proyecto MapBiomas Argentina).
<br>
<br>
El mapa final presenta las áreas de vegetación quemadas del Parque Nacional Los Alerces y su entorno, clasificadas de acuerdo al grado de severidad del incendio (de bajo a alto). La metodología desarrollada se puede replicar en otras áreas de interés y, en conjunto con conocimiento ecológico-ambiental, es posible analizar el impacto sobre distintos tipos de vegetación y áreas urbanas.
<br>
<br>
Si desea acceder a una versión rasterizada del mapa, puede descargarla <strong><a href='https://drive.google.com/drive/folders/1rmh7yFz496JyDFhoQgQ28zojtd1_mRlp?usp=sharing'>aquí</a></strong>.
<br>
<img src='/img/portfolio/mapa.jpg' class='img-responsive img-centered' alt=''>
<br>
<br>
<div class='before-after-slider' id='slider-alerces'>
  <img src='/img/portfolio/alerces-after.png' alt='Imagen posterior al incendio'>
  <div class='ba-before' id='ba-before-alerces'>
    <img src='/img/portfolio/alerces-before.png' alt='Imagen anterior al incendio'>
  </div>
  <div class='ba-divider' id='ba-divider-alerces'>
    <div class='ba-handle'>
      <svg width='16' height='16' viewBox='0 0 16 16' fill='none' xmlns='http://www.w3.org/2000/svg'>
        <path d='M5 8L2 5M5 8L2 11M5 8H1' stroke='#555' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/>
        <path d='M11 8L14 5M11 8L14 11M11 8H15' stroke='#555' stroke-width='1.5' stroke-linecap='round' stroke-linejoin='round'/>
      </svg>
    </div>
  </div>
  <span class='ba-label ba-label-before'>Antes</span>
  <span class='ba-label ba-label-after'>Después</span>
</div>
<p class='ba-hint'>Deslizá para comparar</p>
<style>
  .before-after-slider {
    position: relative;
    width: 100%;
    margin: 1rem auto;
    user-select: none;
    overflow: hidden;
    border-radius: 8px;
    cursor: col-resize;
    border: 1px solid rgba(0,0,0,0.12);
    aspect-ratio: 1386 / 924;
  }
  .before-after-slider {
    aspect-ratio: 1386 / 924;
  }
  .before-after-slider > img {
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 95%;
    object-fit: cover;
    object-position: center;
    pointer-events: none;
    display: block;
  }
  .ba-before {
    position: absolute;
    top: 0; left: 0; bottom: 0;
    overflow: hidden;
    width: 50%;
  }
  .ba-before img {
    width: 100%;
    max-width: none;
    height: 95%;
    object-fit: cover;
    object-position: left center;
    pointer-events: none;
  }
  .ba-divider {
    position: absolute;
    top: 0; bottom: 0;
    left: 50%;
    width: 2px;
    background: #fff;
    transform: translateX(-50%);
    pointer-events: none;
  }
  .ba-handle {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 36px;
    height: 36px;
    border-radius: 50%;
    background: #fff;
    border: 1px solid rgba(0,0,0,0.2);
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .ba-label {
    position: absolute;
    bottom: 10px;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 0.08em;
    text-transform: uppercase;
    padding: 3px 8px;
    border-radius: 4px;
    color: #fff;
    background: rgba(0,0,0,0.5);
    pointer-events: none;
  }
  .ba-label-before { left: 10px; }
  .ba-label-after  { right: 10px; }
  .ba-hint {
    text-align: center;
    font-size: 12px;
    color: #888;
    margin-top: 6px;
    letter-spacing: 0.03em;
  }
</style>
<script>
(function() {
  var wrap = document.getElementById('slider-alerces');
  var beforePane = document.getElementById('ba-before-alerces');
  var divider = document.getElementById('ba-divider-alerces');
  if (!wrap) return;
  var dragging = false;
  function setPos(x) {
    var rect = wrap.getBoundingClientRect();
    var pct = Math.min(Math.max((x - rect.left) / rect.width, 0.02), 0.98);
    beforePane.style.width = (pct * 100) + '%';
    divider.style.left = (pct * 100) + '%';
  }
  wrap.addEventListener('mousedown', function(e) { dragging = true; setPos(e.clientX); });
  wrap.addEventListener('touchstart', function(e) { dragging = true; setPos(e.touches[0].clientX); }, {passive: true});
  document.addEventListener('mousemove', function(e) { if (dragging) setPos(e.clientX); });
  document.addEventListener('touchmove', function(e) { if (dragging) setPos(e.touches[0].clientX); }, {passive: true});
  document.addEventListener('mouseup', function() { dragging = false; });
  document.addEventListener('touchend', function() { dragging = false; });
})();
</script>
<br>

<strong>Referencias</strong>
<br>
- García, M. J .L., & Caselles, V. (1991). Mapping burns and natural reforestation using thematic mapper data. Geocarto International 6, 31–37. 
<br>
- Key, C., & Benson, N. (2005). Landscape assessment: Ground measure of severity, the Composite Burn Index; and remote sensing of severity, the Normalized Burn Index. En D. Lutes, R. Keane, J. Caratti, C. Key, N. Benson, S. Sutherland, & Gangi, L. (Eds.), FIREMON: Fire effects monitoring and inventory system. General Technical Report RMRS-GTR-164-CD LA. (pp. 1−51) Rocky Mountains Research Station: USDA Forest Service.
<br>
- MapBiomas  Argentina  (2024).  Proyecto MapBiomas Argentina- Colección 2 de los Mapas Anuales de Cobertura y Uso del Suelo en Argentina, accedido el 16 de marzo de 2026 a través del enlace: <strong><a href='https://plataforma.argentina.mapbiomas.org/coverage/coverage_lclu?tl[id]=1&tl[themeKey]=coverage&tl[subthemeKey]=coverage_lclu&tl[pixelValues][]=27&tl[pixelValues][]=15&tl[pixelValues][]=9&tl[pixelValues][]=21&tl[pixelValues][]=19&tl[pixelValues][]=36&tl[pixelValues][]=3&tl[pixelValues][]=4&tl[pixelValues][]=6&tl[pixelValues][]=34&tl[pixelValues][]=33&tl[pixelValues][]=77&tl[pixelValues][]=63&tl[pixelValues][]=12&tl[pixelValues][]=11&tl[pixelValues][]=66&tl[pixelValues][]=73&tl[pixelValues][]=24&tl[pixelValues][]=25&tl[legendKey]=default&tl[year]=2024&t[regionKey]=argentina&t[ids][]=17-1-1&t[divisionCategoryId]=2'>MapBiomas</a></strong>. 
<br>
- NASA's Fire Information for Resource Management System, 2021. MODIS Collection 61 NRT Hotspot Active Fire Detections MCD14DL distributed from NASA FIRMS.  <strong><a href='doi:10.5067/FIRMS/MODIS/MCD14DL.NRT.0061'>doi:10.5067/FIRMS/MODIS/MCD14DL.NRT.0061</a></strong>. Plataforma en línea: <strong><a href='https://firms.modaps.eosdis.nasa.gov/map/#d:2026-01-02..2026-02-01;@-71.45,-42.61,9.41z'>Fire Map - NASA | LANCE | FIRMS</a></strong>"
---
