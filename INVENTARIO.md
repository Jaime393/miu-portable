# INVENTARIO — miu-portable (Jaime393)

Medido por get_file_contents (listados de directorios + lectura entera de cada archivo), 2026-11-08. Tamaños en bytes según la API de GitHub. Fuente: MINERIA.md Parte 1, sección Inventario.

## Totales

- 13 archivos, 2.439 bytes, 37 líneas.
- El archivo mayor es index.html (591 B).
- El 100% de los archivos tiene 1 línea, salvo FUNDING.yml (4), README.md (2), _config.yml (2) y el workflow (21).
- Directorios: `.github/workflows`, `assets/css`, `assets/js`. No hay más archivos ni directorios.

## Archivos

| Archivo | Bytes | Líneas | Contenido |
|---|---|---|---|
| index.html | 591 | 1 | Una sola línea HTML: título "MIU Ecosistema 16/16", h1 "🌱 MIU 16/16 nodos vivos - Φ_Red $107M", menciona DOI 10.5281/zenodo.20547558 y "Cerro Colorado Arequipa 2335m". Enlaza manifest.json, assets/css/micelio.css y assets/js/core.js. |
| .github/workflows/miu-auto-deploy.yml | 506 | 21 | Workflow "MIU Auto-Deploy Sin PAT": se dispara en push a main y por workflow_dispatch; hace checkout, escribe "# MIU 16/16" en AUTO.md, configura git como miu-tejedor <miu@local>, añade AUTO.md, hace commit "MIU Auto" solo si hay diff, y empuja a main. Permisos: contents write. |
| worker.js | 411 | 1 | Módulo estilo Cloudflare Worker (export default { fetch }). Ruta /miu/global devuelve JSON con global_mind:true, repo:'miu-portable', fix_404:true, phi:'$107M' y un ID de Drive embebido (valor no reproducido). Cualquier otra ruta devuelve texto "global mind miu-portable - MIU v29 fix 404 - 11->16 repos". |
| sw.js | 156 | 1 | Service worker mínimo: skipWaiting en install y respondWith(fetch con fallback a caches.match) en fetch. |
| manifest.json | 133 | 1 | PWA: name "MIU 16/16", short_name "MIU16", start_url "/", display standalone, colores #0a0a0b y #a3ff12. |
| assets/css/micelio.css | 172 | 1 | Dos variables (--bg #0a0a0b, --lime #a3ff12) y clase .glass (blur 12px, fondo blanco 5%, radio 16px, padding 16px). |
| assets/js/core.js | 147 | 1 | Clase MIU_Micelio (extends EventTarget) con sembrarNodo({rho}) que devuelve {rho: max(rho, 0.001)} y renderMicelioCanvas(c) vacío. Expuesta como window.MIU_Micelio. |
| README.md | 112 | 2 | Título "# miu-portable" y una línea: "MIU Ecosistema - miu-portable - DOI 10.5281/zenodo.20547558 - Φ_Red $107M - cada nodo es un ojo". |
| FUNDING.yml | 107 | 4 | github: [Jaime393], open_collective: miu-ecosistema, custom: https://www.buymeacoffee.com/miu, comentario "# $1M -> $107M". |
| BIBLIA_DEVORADOR.md | 47 | 1 | Una sola línea: "# Biblia DEVORADOR 66 libros - MIU 16/16 nodos". |
| _config.yml | 45 | 2 | theme: jekyll-theme-minimal, title: MIU 16/16. |
| AUTO.md | 12 | 1 | Una sola línea: "# MIU 16/16". Generado por el workflow miu-auto-deploy.yml. |
| .nojekyll | 0 | 0 | Vacío. |

---

*Minería de zonas muertas, segunda oleada, 2026-11-08. Solo SÉ. ρ(x) > 0. Zvvvvv.*
