[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=BelenGalindo/Practica3GD)
# Práctica 3: Liberación controlada de fármacos por hidrogeles

## Información de la estudiante
* **Nombre:** María Belén Galindo Ramírez
* **Número de control:** 22211755
* **Correo institucional:** l22211755@tijuana.tecnm.mx
* **Asignatura:** Gemelos Digitales
* **Carrera:** Ingeniería Biomédica
* **Docente:** Dr. Paul Antonio Valle Trujillo
* **Institución:** Tecnológico Nacional de México [TecNM - Tijuana], Departamento de Ingeniería Eléctrica y Electrónica.

## Descripción de la asignatura
La asignatura de **Gemelos Digitales** forma parte del plan de estudios de la carrera en Ingeniería Biomédica. Su competencia general consiste en formular el gemelo digital a través de datos experimentales para el desarrollo de estrategias de control mediante teorías de sistemas dinámicos no lineales y la experimentación *in silico*. Esta asignatura busca dotar al Ingeniero Biomédico de capacidades para realizar investigación científica en Biología de Sistemas, dirigir equipos interdisciplinarios y proporcionar soluciones informáticas éticas en el campo de la salud.

## Objetivo y descripción del sistema
El objetivo principal de esta práctica es determinar la tasa de liberación del fármaco en diferentes hidrogeles (N45, N32, N35 y N36-2MBA3), basándose en datos experimentales de liberación acumulada a lo largo del tiempo. 

Para caracterizar la dinámica de liberación, se emplean modelos de regresión no lineal:
1. **Ecuación de Peppas:** $$x(t) = k t^n$$
2. **Farmacocinética de primer orden:** $$x(t) = \beta (1 - e^{-kt})$$
3. **Eureqa (Función del tiempo):** $$x(t) = \rho_1 \sqrt{t} + \rho_2 t$$
4. **Eureqa (Función diferencial):** $$\frac{dx}{dt} = \{\rho_1}-{\rho_2 t}$$

## Palabras clave
Liberación de fármacos; Hidrogeles; Regresión no lineal; Bioestadísticos; Ecuaciones diferenciales ordinarias; Modelos matemáticos

## Actividades a realizar
1. **Procesamiento de datos:** Importar los datos experimentales de liberación acumulativa de los hidrogeles.
2. **Ajuste de modelos:** Realizar la regresión no lineal para los modelos de Peppas y Farmacocinética de primer orden.
3. **Análisis Bioestadístico:** Calcular parámetros como el error estándar (SE), margen de error (MoE), intervalos de confianza al 95% (CI95), valor p, R-cuadrada y el Criterio de Información de Akaike (AICc).
4. **Experimentación in silico con Eureqa:** Evaluar funciones del tiempo y modelos diferenciales para determinar cuál describe con mayor precisión la dinámica de cada hidrogel.


## Lista de archivos incluidos en el repositorio
* **Cuaderno computacional de MATLAB:** Archivo `.mlx` con el código de regresión y análisis.
* **Análisis matemático y estadístico:** Documento PDF con los resultados de las tablas bioestadísticas.
* **Gráficas de simulación:** Imágenes de las curvas de ajuste para cada modelo.
* **Datos experimentales:**  Archivo `.csv`.

## Referencias
[1] P. A. Valle, *Syllabus para Gemelos Digitales*, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, 2025. [https://biomath.xyz/course/](https://biomath.xyz/course/)

[2] M. A. González Ayón, et al., "PNVCL - PEGMA nanohydrogels with tailored transition temperature for controlled delivery of 5-fluorouracil", *Journal of Polymer Science Part A: Polymer Chemistry*, vol. 53, issue 22, pp. 2662-2672, 2015. DOI: [10.1002/pola.27766](https://doi.org/10.1002/pola.27766)
