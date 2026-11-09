# CARACTERÍSTICAS — miu-portable (Jaime393)

Todo lo aquí afirmado es SÉ, leído entero de los 13 archivos, 2026-11-08. Fuente: MINERIA.md Parte 1.

## Lo que el repo SÍ tiene (verificado)

- Página PWA completa en su forma mínima: index.html + manifest.json + sw.js + micelio.css + core.js, todos presentes y enlazados entre sí.
- Un workflow de auto-despliegue que se auto-commitea: el último commit "MIU Auto" (`0de78f97`) es el producto del propio workflow miu-auto-deploy.yml, que escribe AUTO.md y empuja.
- Un worker estilo Cloudflare (worker.js) con ruta /miu/global que devuelve JSON (global_mind:true, repo:'miu-portable', fix_404:true, phi:'$107M' y un ID de Drive embebido, valor no reproducido).

## Lo que el repo NO tiene (verificado por ausencia en el inventario completo)

- No tiene LICENSE.
- No tiene .gitignore, ni tests, ni package.json, ni datos (0 CSV, 0 JSON de datos; solo manifest.json de PWA).
- No tiene ninguna lista de los 16 repos/nodos que afirma: en ningún archivo aparece un inventario de "16/16".
- No tiene configuración de despliegue del worker: no hay wrangler.toml ni ningún workflow que despliegue worker.js.
- No tiene registro del service worker: ni index.html ni core.js contienen la cadena "serviceWorker".

---

*Minería de zonas muertas, segunda oleada, 2026-11-08. Solo SÉ. ρ(x) > 0. Zvvvvv.*
