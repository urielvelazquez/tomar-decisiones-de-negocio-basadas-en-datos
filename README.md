### ¿Qué funciona realmente? Un estudio de priorización de ideas y pruebas A/B en Marketing

#### Objetivo del proyecto
Evaluar y priorizar hipótesis de crecimiento y analizar los resultados de una prueba A/B con base en datos reales de usuarios, con el fin de:

- Determinar las estrategias con mayor impacto potencial en los ingresos

- Validar la efectividad de cambios en el comportamiento de compra

- Tomar decisiones basadas en datos para optimizar campañas de marketing y experiencia del usuario

#### Lenguaje de programación, librerías y habilidades 
![Python](https://img.shields.io/badge/PYTHON-%232A5D9F.svg?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/PANDAS-%232A5D9F.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NUMPY-%232A5D9F.svg?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SCIPY-%232A5D9F.svg?style=for-the-badge&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/MATPLOTLIB-%232A5D9F.svg?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/SEABORN-%232A5D9F.svg?style=for-the-badge&logo=seaborn&logoColor=white)
![Limpieza de Datos](https://img.shields.io/badge/LIMPIEZA%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Priorizar hipótesis](https://img.shields.io/badge/PRIORIZAR%20HIPÓTESIS-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis de pruebas A/B](https://img.shields.io/badge/ANÁLISIS%20DE%20PRUEBAS%20A%2FB-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Visualización de Datos](https://img.shields.io/badge/VISUALIZACIÓN%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)

#### Preguntas clave
- ¿Qué hipótesis muestran mayor potencial según los frameworks ICE y RICE, y cómo cambia su priorización?

- ¿Cuál es la diferencia estadísticamente significativa en la conversión y tamaño promedio de pedido entre los grupos A y B?

- ¿Debería detenerse o continuar la prueba A/B con base en los resultados obtenidos y las anomalías detectadas?

#### Metodología
- **Preprocesamiento de datos:** Se limpiaron y ajustaron los datos: se corrigieron tipos, se eliminaron duplicados y se trataron valores faltantes.

- **Priorizar hipótesis:** Se aplicaron los frameworks ICE (Impact, Confidence, Effort) y RICE (Reach, Impact, Confidence, Effort) para evaluar y priorizar las hipótesis propuestas por el departamento de marketing.

- **Análisis de pruebas A/B:** Se analizaron los datos para calcular las tasas de conversión diarias por grupo y se aplicaron pruebas de hipótesis estadísticas sobre conversiones y tamaños de pedidos con y sin datos filtrados.

#### Conclusión general
- Los datos sin procesar y los filtrados revelaron diferencias estadísticamente significativas en la conversión entre los grupos.

- Ni los datos sin procesar ni los filtrados revelaron diferencias estadísticamente significativas en el tamaño promedio de los pedidos entre los grupos.

- La gráfica que muestra la `diferencia relativa para las tasas de conversión` entre los grupos dice que los resultados del Grupo B son mejores y parecen mantenerse en ese sentido a lo largo del periodo.

- La gráfica que muestra la `diferencia relativa en el tamaño de pedido promedio acumulado` entre los grupos dice que los resultados del Grupo B son mejores día tras día y actualmente son un 30% más altos que los del Grupo A.

Basándose en estos hechos, hay que parar la prueba y considerar al Grupo B como líder. No tiene sentido continuar, ya que la probabilidad de que el Grupo B resulte ser mejor que el Grupo A es real.

#### Diccionario de datos
**Datos utilizados en la primera parte del proyecto**

La tabla `hypotheses` (contiene hipótesis sobre cómo aumentar los ingresos de una tienda online):

- `Hypotheses:` breves descripciones de las hipótesis.

- `Reach:` alcance del usuario, en una escala del uno a diez.

- `Impact:` impacto en los usuarios, en una escala del uno al diez.

- `Confidence:` confianza en la hipótesis, en una escala del uno al diez.

- `Effort:` los recursos necesarios para probar una hipótesis, en una escala del uno al diez. Cuanto mayor sea el valor Effort, más recursos requiere la prueba.

**Datos utilizados en la segunda parte del proyecto**

La tabla `orders` (datos sobre pedidos):

- `transactionId:` identificador de pedido.

- `visitorId:` identificador del usuario que realizó el pedido.
  
- `date:` fecha del pedido.

- `revenue:` ingresos del pedido.

- `group:` el grupo del test A/B al que pertenece el usuario.

La tabla `visits` (contiene información sobre las visitas diarias al sitio web):

- `date:` la fecha.

- `group:` grupo de la prueba A/B.

- `visits:` el número de visitas en la fecha especificada en el grupo de pruebas A/B especificado.

**Nota:** Asegúrate de preprocesar los datos. Es posible que haya errores en los datasets originales; por ejemplo, algunos de los visitantes podrían haber entrado tanto en el grupo A como en el grupo B.
