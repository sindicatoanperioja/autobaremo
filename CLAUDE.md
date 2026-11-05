# Autobaremo

Calculadora para que cada docente se autobaremara el Concurso de Traslados 2026-2027 de La Rioja. ANPE La Rioja. Una sola página (`index.html`), sin dependencias salvo Google Fonts.

- Fuente del baremo: Anexo XI de la Resolución 88/2026 (BOR n.º 208, 28-10-2026) y el resumen del baremo de ANPE La Rioja (unidad compartida, no se sube). Fin de plazo y fecha de referencia: 26-11-2026.
- El cálculo vive entre `/*ENGINE-START*/` y `/*ENGINE-END*/` (función `calcular`). El formulario se genera desde `APARTADOS`.
- Topes: apartado 3 máx. 10; 4 máx. 30 (4.3 máx. 10); 5 máx. 15 (5.1 máx. 9, 5.2 máx. 3, 5.4 máx. 3); 6 máx. 15 (6.1 máx. 8, 6.2 y 6.3 máx. 2,5). Apartados 1 y 2 sin máximo.
- Idiomas: dos listas separadas, 3.3 solo EOI o DLSE y 5.5 solo otros certificados ACLES. Un solo certificado por idioma entre las dos (el de nivel más alto).
- Interinos cuentan en 1.2 y 4 (criterio del resumen de ANPE).
- Identidad de ANPE La Rioja, la misma paleta y cabecera que Retribuciones. Textos humanizados (ver instrucciones globales).
- Repo público en github.com/sindicatoanperioja/autobaremo, publicado con GitHub Pages en https://traslados.cursosanperioja.es (archivo CNAME; DNS: CNAME traslados → sindicatoanperioja.github.io). No subir rutas de la unidad Z: ni enlaces privados. Cada commit va seguido de `git push`.
- Tiempo: por defecto años y meses (`S.am`); quien quiera mete periodos con fechas (`S.modo[campo] = "fechas"`, lista en `S[campo]`). Solo con fechas se detectan solapes: en un mismo campo se rechazan; entre 4.1, 4.2 y 4.3 y entre 1.1, 1.2.2 y 1.2.3 se quitan los días del que menos puntúa.
- Sin selector de cuerpo: Catedrático es un interruptor en el apartado 2. "Expectativa" = funcionario de carrera sin destino definitivo (1.1.2).
- «Cómo se justifica» de cada mérito: objeto `DOCS` (columna de documentos del Anexo XI y base 15 de la convocatoria). El resumen general va en «Qué hay que presentar».
- Visitas: Cloudflare Web Analytics (sin cookies), script al final del body; el panel está en la cuenta de Cloudflare del sindicato.
