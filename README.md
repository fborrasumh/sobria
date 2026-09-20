# SobrIA

**Humanizador de manuscritos académicos en un único fichero HTML.** Le quita a un texto la retórica inflada de la IA sin tocar ni un dato.

👉 **[Abrir la aplicación](https://fborrasumh.github.io/sobria/)**

Reproduce en el navegador el skill [`humanizer_academic`](https://github.com/matsuikentaro1/humanizer_academic) de Kentaro Matsui (MIT), basado a su vez en [`blader/humanizer`](https://github.com/blader/humanizer) y en la guía [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), adaptada a la literatura médica y científica.

## Qué hace

- **Lee el manuscrito** desde Markdown, texto, Word (.docx) o PDF, o pegado directamente. Los ficheros se procesan en el navegador; al modelo solo viaja el texto.
- **Aplica los 34 patrones** del skill, activables uno a uno y agrupados por familia. Los ocho que solo tienen sentido en inglés se desactivan automáticamente con textos en español.
- **Empieza por el ritmo de frase** (patrón 34) antes que por el vocabulario: según las pruebas del autor del skill con detectores locales, la reestructuración del ritmo explica en torno al 90 % de la mejora alcanzable.
- **Dos pasadas**: borrador y autoauditoría («¿qué sigue delatando este texto como generado?»), con comprobaciones finales obligatorias de rayas largas, cohesión de párrafo y ritmo.
- **Mide las huellas en el navegador**, antes y después: variabilidad de la longitud de frase, rachas de aperturas nominales, vocabulario característico de la IA por mil palabras, rayas largas, muletillas, reformulaciones y frases de evaluación vacías.
- **Guardia de integridad**: comprueba que todas las cifras, valores p, intervalos y citas del original siguen presentes en el resultado, y avisa de los que no encuentra.
- **Comparación párrafo a párrafo** con marcas de corrección, informe de cambios y exportación a Markdown, Word y PDF.
- **Calibración de voz opcional**: pegando dos o tres párrafos propios anteriores a 2023, las sustituciones se ajustan al repertorio de conectores y a la longitud de frase del autor en lugar de a un «humano genérico».

## Uso

Abre la aplicación, introduce tu clave de OpenAI (se guarda solo en tu navegador, en `localStorage`, compartida con el resto del catálogo) y elige el modelo. No hay servidor: todo ocurre entre tu navegador y la API de OpenAI.

## Para qué no sirve

SobrIA **no sirve para eludir detectores de IA ni marcas de procedencia**, y **no exime de declarar el uso de IA** donde la revista, la convocatoria o la universidad lo exijan. Un texto escrito por una IA sigue siendo un texto escrito por una IA después de pasar por aquí: lo que cambia es que deja de sonar a plantilla, no quién lo escribió. Revisa siempre el resultado frente al original antes de firmarlo.

## Referencias

- Matsui K. Delving Into PubMed Records: How AI-Influenced Vocabulary has Transformed Medical Writing since ChatGPT. *Perspect Med Educ*. 2025;14(1):882-890. [doi:10.5334/pme.1929](https://doi.org/10.5334/pme.1929)
- Fitchett D, Inzucchi SE, Cannon CP, et al. Empagliflozin Reduced Mortality and Hospitalization for Heart Failure Across the Spectrum of Cardiovascular Risk in the EMPA-REG OUTCOME Trial. *Circulation*. 2019;139(11):1384-1395. (CC-BY-4.0; origen de los ejemplos del skill)

## Autoría y licencia

Fernando Borrás Rocher · Universidad Miguel Hernández de Elche · [ORCID 0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

Parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/). Licencia MIT.
