# Perspectiva CE2024 – Sinaloa

## Descripción general
Este repositorio concentra los insumos analíticos y de comunicación utilizados para documentar la estructura social, laboral y empresarial de Sinaloa con base en los Censos Económicos 2024 (CE2024) y otras fuentes oficiales. Aquí encontrarás el cuaderno fuente que genera las láminas, el resumen ejecutivo con los hallazgos principales y materiales gráficos listos para difusión.

## Contenido del repositorio
- `Resumen ejecutivo.md`: Documento narrativo con conclusiones temáticas sobre demografía, mercado laboral, tejido empresarial, valor agregado, adopción tecnológica y financiamiento.
- `generacion_unitaria_actualizada.ipynb`: Cuaderno de Jupyter que produce las visualizaciones (diapositivas) y consolida tablas auxiliares; utiliza `pandas`, `numpy`, `matplotlib`, `requests`, `openpyxl`, `xlrd`, `PyPDF2`, `python-dotenv`, entre otras dependencias estándar.
- `salida/`: Carpeta con las imágenes PNG numeradas (diapositivas 03–73) que se derivan del cuaderno y sirven para presentaciones o reportes.
- `infografia_sinaloa_ce2024.html`: Infografía web interactiva que resume los indicadores clave y puede publicarse o compartirse en navegadores modernos.

## Principales hallazgos
- La jefatura femenina pasó de 20.3 % en 2000 a 35.4 % en 2020, ubicando a Sinaloa entre los estados con mayor participación de mujeres como cabeza de hogar.
- La derechohabiencia a servicios de salud creció de 53 % a 80.8 % entre 2000 y 2020; el IMSS concentra la mitad de las afiliaciones, aunque persiste un rezago cercano a una quinta parte de la población sin cobertura.
- El mercado laboral muestra baja desocupación (2.2 % vs 2.7 % nacional en 2025-II) y menor informalidad (46.6 % vs 54.8 %), con predominio del sector servicios y de trabajadores asalariados.
- Los Censos Económicos 2024 registran 153,100 unidades económicas que emplean a 842,332 personas; 93.4 % son microempresas y la actividad se concentra en cinco municipios.
- El valor agregado, la inversión y la infraestructura tecnológica se concentran en establecimientos medianos y grandes, lo que revela brechas productivas respecto a la base microempresarial.
- El crédito bancario sigue siendo limitado para las pymes por requisitos de garantías, trámites complejos, cultura de autofinanciamiento y percepción de riesgo; se sugieren esquemas de acompañamiento y fondos de garantía.

## Cómo reproducir el análisis
### Requisitos
1. Python 3.10+.
2. Entorno virtual recomendado (`python -m venv .venv` y activar según sistema).
3. Instalación de dependencias:
   ```bash
   pip install pandas numpy matplotlib requests openpyxl xlrd python-dotenv PyPDF2
   ```
   Ajusta la lista si tu entorno ya cuenta con paquetes equivalentes.

### Pasos
1. Actualiza las variables de entorno o el archivo `.env` si se requiere acceso autenticado a fuentes externas.
2. Abre `generacion_unitaria_actualizada.ipynb` en Jupyter Lab/Notebook y ejecuta todas las celdas en orden; esto actualizará los PNG dentro de `salida/`.
3. Verifica los pendientes anotados en la primera celda del cuaderno (diapositivas 53, 42 y 21 marcadas para revisión) antes de publicar la versión final.

## Productos de comunicación
- **Resumen ejecutivo**: síntesis narrativa para tomadores de decisión (`Resumen ejecutivo.md`).
- **Láminas**: archivos PNG numerados dentro de `salida/` listos para presentaciones.
- **Infografía interactiva**: archivo HTML (`infografia_sinaloa_ce2024.html`) optimizado para navegadores y dispositivos móviles. Para compartirlo, súbelo a un servidor estático o abre el archivo localmente en tu navegador.

## Fuentes de datos destacadas
- Resultados definitivos de los Censos Económicos 2024 (INEGI) y Perspectiva de Sinaloa CE2024.
- Indicadores del ITAEE, ocupación y empleo del INEGI y del IMSS.
- Publicaciones de análisis de organismos estatales (CODESIN, Sinaloa en Números) y medios especializados (El Economista, Olegario.mx).
- Documentos de referencia sobre normatividad económica y adopción tecnológica (Secretaría de Economía, México ¿Cómo Vamos?, TNE, entre otros).
- Consulta el listado completo en las referencias vinculadas dentro de `Resumen ejecutivo.md`.

## Próximos pasos sugeridos
- Validar las diapositivas marcadas como “se debe checar” dentro del cuaderno para asegurar consistencia de datos.
- Corregir la codificación de caracteres del `Resumen ejecutivo.md` (guardar en UTF-8) para recuperar acentos y caracteres especiales en todos los visores.
- Integrar controles automatizados (por ejemplo, scripts de verificación) si se planea actualizar periódicamente los indicadores CE2024.
