# Autobaremo

Calculadora para que cada docente se autobaremara el Concurso de Traslados 2026-2027 de La Rioja. ANPE La Rioja. Una sola página (`index.html`), sin dependencias salvo Google Fonts.

- Fuente del baremo: Anexo XI de la Resolución 88/2026 (BOR n.º 208, 28-10-2026) y el resumen del baremo de ANPE La Rioja (unidad compartida, no se sube). Fin de plazo y fecha de referencia: 26-11-2026.
- El cálculo vive entre `/*ENGINE-START*/` y `/*ENGINE-END*/` (función `calcular`). El formulario se genera desde `APARTADOS`.
- Topes: apartado 3 máx. 10; 4 máx. 30 (4.3 máx. 10); 5 máx. 15 (5.1 máx. 9, 5.2 máx. 3, 5.4 máx. 3); 6 máx. 15 (6.1 máx. 8, 6.2 y 6.3 máx. 2,5). Apartados 1 y 2 sin máximo.
- Idiomas: un solo certificado por idioma (el de nivel más alto), en 3.3 si es de EOI o DLSE y en 5.5 si es otro ACLES.
- Interinos cuentan en 1.2 y 4 (criterio del resumen de ANPE).
- Identidad de ANPE La Rioja, la misma paleta y cabecera que Retribuciones. Textos humanizados (ver instrucciones globales).
- Repo público en github.com/sindicatoanperioja/autobaremo, publicado con GitHub Pages (https://sindicatoanperioja.github.io/autobaremo/). No subir rutas de la unidad Z: ni enlaces privados. Cada commit va seguido de `git push`.
