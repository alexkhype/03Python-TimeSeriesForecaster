# Predicción de Taxis Necesarios por Hora

## Tabla de Contenidos
- [Descripción](#Descripción)
- [Datos](#Datos)
- [Análisis](#Análisis)
- [Tecnologías y herramientas](#Tecnologías-y-herramientas)
- [Resultados](#Resultados)
- [Contribuciones](#Contribuciones)
- [Licencia](#Licencia)
- [Contacto](#Contacto)

## Descripción
Este proyecto predice la cantidad de taxis necesarios por hora en aeropuertos para optimizar la disponibilidad de conductores durante las horas pico, usando modelos de machine learning basados en series temporales y remuestreo horario.

## Datos
Se utilizaron XXX conjuntos de datos principales:  
- XXXX **games.csv**: Contiene registros de ventas por juego, plataforma, año, y regiones (Norteamérica, Europa, Japón, y resto del mundo).  
- XXXX **scraping.csv**: Dataset auxiliar para completar datos faltantes.  

Características clave incluyen:  
- XXXX 16,500 registros históricos.  
- XXXX Variables: nombre, plataforma, año, género, clasificación ESRB, ventas por región, calificaciones de críticos y usuarios.  
- XXXX Datos limpios y normalizados para análisis.  

## Análisis
- Se analizó el histórico de órdenes de taxis horario entre marzo y agosto de 2018, identificando tendencias y estacionalidades diarias y semanales.
- Se comprobó estacionariedad con prueba ADF y se seleccionaron variables predictivas clave usando ACF y PACF.
- Se crearon características adicionales como medias móviles y variables de tiempo para mejorar la precisión.
- Se dividió el dataset para una validación robusta evitando información futura en el modelo.
- Se entrenaron y ajustaron múltiples modelos, incluyendo regresión lineal, DecisionTree, RandomForest, LGBM y CatBoost, usando GridSearchCV y validación cruzada específica para series temporales.

## Tecnologías y herramientas
- Python 3.9 para desarrollo y análisis
- Pandas, NumPy para manipulación y análisis de datos
- Matplotlib, sktime para visualización de series temporales
- statsmodels para análisis estadístico y diagnóstico de series temporales
- Scikit-learn, LightGBM, CatBoost, XGBoost para modelado y validación de machine learning
- Jupyter Notebook para desarrollo interactivo y documentación del proyecto

## Resultados
- Modelos de boosting como LGBMRegressor y CatBoostRegressor superaron a los modelos base y de árbol tradicionales en RMSE.
- LGBMRegressor mostró mejor precisión para anticipar picos de demanda en horas críticas.
- CatBoostRegressor ofrece predicciones más estables pero menos sensibles a extremos.
- El modelo base de regresión lineal logró un RMSE de referencia de 46.02.
- La selección del modelo depende de la prioridad: exactitud en picos o estabilidad en predicciones.

## Contribuciones
Bienvenidas sugerencias, correcciones y nuevas visualizaciones. Por favor, abre un issue o pull request para colaborar.

## Licencia
Este proyecto está bajo la licencia MIT.

## Contacto
Nombre: Alejandro M. García  
Email: [alexkhype@gmail.com](mailto:alexkhype@gmail.com)  
LinkedIn: [linkedin.com/in/amggl](https://linkedin.com/in/amggl)
