## Actividad dirigida 3

Esta es la actividad Dirigida 3 que consiste en hacer un ejercicio de programación literaria aprovechando el código que hemos usado en programación con Python donde realizamos web scraping. A continuación pongo el código fuente.

## Código fuente


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored

resultados = []

req = requests.get("https://resultados.elpais.com")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')

tags = soup.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req3 = requests.get("https://elpais.com/opinion")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup3 = BeautifulSoup(req3.text, 'html.parser')

tags = soup3.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')

tags = soup4.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')

tags = soup5.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')

tags = soup6.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')

tags = soup7.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')

tags = soup8.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')

tags = soup9.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')

tags = soup10.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')

tags = soup11.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')

tags = soup12.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')

tags = soup13.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req14 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup14 = BeautifulSoup(req14.text, 'html.parser')

tags = soup14.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')

tags = soup15.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

B

req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')

tags = soup17.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)


os.system("clear")

print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))

print(colored("Igualdad", 'green', attrs=['bold']))

str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))

print(colored("Mujeres", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))

print(colored("Mujer", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))

print(colored("Brecha salarial", 'green', attrs=['bold']))

str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))

print(colored("Machismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))

print(colored("Violencia", 'green', attrs=['bold']))

str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))

print(colored("Maltrato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))

print(colored("Homicidio", 'green', attrs=['bold']))

str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))

print(colored("Género", 'green', attrs=['bold']))

str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))

print(colored("Asesinato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))

print(colored("Sexo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))

```

## Instalamos librerías para realizar el web scraping 


```python
pip install requests bs4 pandas termcolor
```

    Requirement already satisfied: requests in c:\users\katia\anaconda3\lib\site-packages (2.27.1)
    Requirement already satisfied: bs4 in c:\users\katia\anaconda3\lib\site-packages (0.0.1)
    Requirement already satisfied: pandas in c:\users\katia\anaconda3\lib\site-packages (1.4.2)
    Requirement already satisfied: termcolor in c:\users\katia\anaconda3\lib\site-packages (1.1.0)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\katia\anaconda3\lib\site-packages (from requests) (2021.10.8)
    Requirement already satisfied: charset-normalizer~=2.0.0 in c:\users\katia\anaconda3\lib\site-packages (from requests) (2.0.4)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\katia\anaconda3\lib\site-packages (from requests) (1.26.9)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\katia\anaconda3\lib\site-packages (from requests) (3.3)
    Requirement already satisfied: beautifulsoup4 in c:\users\katia\anaconda3\lib\site-packages (from bs4) (4.11.1)
    Requirement already satisfied: pytz>=2020.1 in c:\users\katia\anaconda3\lib\site-packages (from pandas) (2021.3)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\katia\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\katia\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: six>=1.5 in c:\users\katia\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Requirement already satisfied: soupsieve>1.2 in c:\users\katia\anaconda3\lib\site-packages (from beautifulsoup4->bs4) (2.3.1)
    Note: you may need to restart the kernel to use updated packages.
    

## Librerías
Hay algunas librerías que vienen con Python y otras no, estas librerías requieren instalarlas, otras no.

## Librerías internas

 - [csv](https://docs.python.org/3/library/csv.html) : Es un archivo con el que podemos almacenar datos con una forma tabular estructurada de (fila,columna).
 - [re](https://docs.python.org/3/library/re.html ) :Este módulo llamado re, tiene funciones que permiten trabajar con expresiones regulares y cadenas.
 - [time](https://docs.python.org/es/3/library/time.html) : Con time podemos utilizar sus funciones manipular la fecha y hora.
 - [os](https://docs.python.org/3/library/os.html) : Os muestra en Python las funcionalidades del sistema operativo.
 

## Librerías externas
-  [termcolor](https://pypi.org/project/termcolor/) : Es una biblioteca que sirve para imprimir mensajes de colores en el terminal.
- [bs4](https://es.acervolima.com/python-beautifulsoup-encontrar-todas-las-clases/) :Beautiful Soup (bs4) es una biblioteca de la cual podemos obtener datos  en formato HTML y XML
- [requests](https://cosasdedevs.com/posts/web-scraping-con-requests-y-beautifulsoup-en-python/) : Se usa para hacer solicitudes y peticiones a la página de la que extraeremos datos.
- [pandas](https://pypi.org/project/pandas/) Es una herramienta de análisis de datos de código, de lectura rápida en el lenguaje de programación de Python.

## Importación de librerías para que los comandos correspondan


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored
```

## Objetos

Hay que crear un objeto demominado resultados, esto sirvá para añadan los resultados del scrapping.



```python
resultados = []
```

Type() es para organizar información de datos en forma de lista.



```python
type (resultados)
```




    list



## División de los códigos para web scrapping

## Impresión de titulares para el periódico EL PAÍS

La variable para solicitar información de la URL será: req=requests.get ("https://resultados.elpais.com")



```python
req = requests.get("https://resultados.elpais.com")
```

Después escribimos la función type() y esa es la respuesta de request.


```python
type(req)
```




    requests.models.Response



If complementa a: if(req.status_code != 200), que es un código de respuesta que muestra un estado satisfactorio a la solicitud. Luego se extrae el texto HTML del sitio web con BeautifulSoup(req.text, 'html.parser').
Con findAll se guardará las etiquetas, los tags, que es el titular de la web y finalmente con resultados.append(h2.text) se irán añadiendo todos dentro de las lista de titulares que hemos ido seleccionando.


```python
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')
```


```python
tags = soup.findAll("h2")
 
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Bruselas pide restringir desde este verano el consumo de gas ante la crisis energética
    Draghi dimite como primer ministro y aboca a Italia a una nueva crisis política
    Macron prepara un plan de ahorro energético ante una Rusia que usa el gas como “arma de guerra”
    Los nuevos impuestos, en el resto de Europa: cada vez más habituales sobre las eléctricas; muy escasos sobre la banca
    Gestionar el agua
    La importancia de una memoria compartida
    Las lecciones de Jimena
    Yo, ‘mindundi’
    El encanto estival de la eterna Euskadi élfica
    Sciammarella
    El PP anuncia que se abstendrá en la votación del segundo decreto anticrisis del Gobierno
    Feijóo provoca una foto con víctimas del terrorismo en pleno debate de la ley de memoria para sugerir su desacuerdo
    Todas las Españas posibles en 138 propuestas
    Los universitarios miden tres centímetros más que los que solo tienen estudios de primaria
    Sonia Livingstone: “Si envolvemos a nuestros hijos en algodón digital, no aprenderán a sobrellevar los problemas”
    El abogado de la UE da la razón a España frente a Bélgica y abre la puerta a la entrega de Puigdemont 
    Vídeo | Qué esperar de la reunión entre Sánchez y Aragonés
    La Eurocámara solicita a Marlaska que comparezca por la tragedia de Melilla
    El tope a la actualización de los alquileres ahorra hasta 1.000 euros a los inquilinos
    La primera semana de primarias en el Partido Conservador británico confirma el liderazgo de Sunak
    El presidente de Sri Lanka renuncia al cargo tras su huida a Singapur
    La subida de precios dispara las protestas en África
    La oleada de incendios en Portugal deja ya un saldo de 813 fuegos, un fallecido y 135 heridos
    Las llamas expulsaron a los veraneantes de Monsagro
    Peña Nieto pone en venta su vivienda de lujo en Madrid tras conocer que la Fiscalía le investigaba
    ¿Sabe cómo de rico es? Averigue su posición en la escalera del dinero
    La Fiscalía pide seis años de prisión y 21 de inhabilitación para Borràs por prevaricación y falsedad documental
    La Audiencia Nacional impulsa una séptima investigación contra la excúpula de ETA
    Aumentan a tres los detenidos por la muerte de la mujer arrojada a una alcantarilla en Málaga
    El Bono Joven Cultural se pone en marcha a finales de julio  
    La paradoja de la obesidad: ¿Por qué si los indicadores empeoran los españoles dicen sentirse más sanos?
    Armie Hammer, de estrella de Hollywood y acusaciones caníbales a vender casas en las islas Caimán
    Bill Gates donará toda su fortuna a la fundación filantrópica que creó
    Cómo aliviar el dolor de piernas por el calor y cuándo hay que preocuparse por las varices
    Dónde comprar los 10 mejores helados artesanos en España
    La ola de calor se recrudece con cinco avisos rojos en Galicia, Andalucía, Extremadura y las dos Castillas
    Así se huye del calor en Madrid: casi 10 grados de diferencia entre Callao y Madrid Río
    El rincón más fresco de Barcelona: el paraje de Collserola con hasta 10 grados menos que el Raval
    “La clave contra el racismo es la empatía”
    Las infinitas posibilidades de un tablero de ajedrez
    “No hay pensamiento sin tiempo para pensar”
    Descubierto un autorretrato de Van Gogh oculto en la parte de atrás de un lienzo fechado en 1885
    La segunda muerte de Vicente Aleixandre, la segunda ruina de Velintonia
    ¿Necesita mi cuerpo tener relaciones sexuales?
    Descubierto el principio matemático detrás de los escutoides, las formas geométricas de moda
    El 20% de las playas españolas quiere ser “libre de humo” pero solo en una minoría está prohibido fumar
    Vídeo | El antídoto de Fito contra los momentos de bajón
    Ucrania y Rusia logran los primeros avances en la negociación para desbloquear el cereal ucranio
    Un tribunal de Manhattan condena a un exinformático de la CIA por la filtración de documentos a WikiLeaks
    Daniel Ortega acelera la implantación del régimen de partido único en Nicaragua 
    Biden reafirma en Israel el “compromiso inquebrantable” con su seguridad
    Amancio Ortega compra un rascacielos de viviendas en Nueva York por 500 millones
    Pidcock triunfa en Alpe d’Huez y Vingegaard afianza el liderato en el Tour de Francia
    Xavi gana el pulso por Dembélé 
    Damaris Egurrola, la futbolista que se fue dos veces de España
    El Mundial de Atletismo vuelve a su esencia
    Saint Andrews es el golf
    Gustavo Gimeno será el nuevo director musical del Teatro Real en 2025
    Muere el periodista Eugenio Scalfari, fundador del diario italiano ‘La Repubblica’, a los 98 años
    Donna Leon: “Los trabajadores de un almacén de Amazon son los esclavos de hoy”
    Del miedo y la rabia al arrepentimiento, la maternidad en imágenes
    Ahora el enemigo es ‘woke’: cómo la concienciación social se convirtió en objeto de burla
    No hacerlo todo juntos: claves para que agosto no se convierta en el mes de los divorcios
    Kate Moss vuelve a ser musa de Zara: la modelo llena de glamur la última campaña de la firma
    “¿Qué tal si te ahorcas?”: el misterio sin resolver de ‘The Girl from Plainville’
    Aurelio Morales, el hombre que dejó una estrella Michelin para tomar impulso y ganar tres
    “Papá, mamá, ¿cuándo llegamos?”: seis sencillos consejos para viajar con niños 
    Un servicio médico en cualquier lugar y momento
    Jóvenes repobladores: comprar una casa en un pueblo de menos de 5.000 habitantes y recibir una ayuda del Gobierno
    “Tomo seis pastillas al día para aguantar”: así es trabajar limpiando hoteles masificados en verano
    Carme Elías: “Me siento más ligera que nunca, como si la vida me hubiera preparado para este momento”
    La escalada vertiginosa de notas en Bachillerato: los sobresalientes de los que llegan a Selectividad se doblan en seis años
    Vídeo | Qué hay detrás de las imágenes del telescopio ‘James Webb’
    Matanza de Uvalde: un vídeo revela la irrupción del asesino y la inacción de la policía 
    Un piloto aficionado logra un aterrizaje de emergencia en una carretera de Carolina del Norte 
    Los homicidios en Chile escalan casi un 30% en el primer semestre de 2022
    Alemania autoriza la puesta en marcha de sus centrales de carbón ya jubiladas para ahorrar gas 
    Europol sitúa el extremismo violento de derechas entre las principales amenazas a la seguridad en la UE
    El PP cede a Vox un puesto en la Mesa del Parlamento andaluz y espera a cambio “generosidad”
    Aitana Mas mantendrá a los cargos imputados en el caso de Mónica Oltra y apela a la presunción de inocencia
    Obituario | Tomás S. Vives y la construcción jurídica de la democracia
    La Audiencia Nacional abre juicio oral a Iberdrola por manipular el precio de la luz
    Los supermercados Dia venden un 8,5% más en el primer semestre, con más peso de las marcas propias
    Gobierno y grandes caseros discrepan sobre la manera de sumar 30.000 alquileres sociales
    El Constitucional amplía el acceso a la justicia gratuita a personas discapacitadas por un accidente
    ‘Un nuevo modelo de residencias para las próximas generaciones de personas mayores: que sean como casas’, por Gustavo García
    Kevin Spacey se declara “no culpable” de los delitos de abusos sexuales que se le imputan en el Reino Unido
    Becas para ricos mezcladas con aborto
    Estudiar en el extranjero, una inversión que mejora la empleabilidad y las competencias interpersonales
    Gabriela Ossenbach, experta en manuales escolares: “Con los libros de texto se puede crear fácilmente alarma social, pero no está justificada”
    Estos serán los tutores legales del mar Menor encargados de su representación y gobernanza
    Absuelto un conductor que se dio a la fuga tras arrollar a un ciclista: “Te sientes atropellado por el coche y la justicia”
    El Constitucional anula parte de la ley de Castilla y León que permitía cazar al lobo 
    Alberto Ascherio: “Sin el virus de la enfermedad del beso, el riesgo de esclerosis múltiple es casi cero”
    ¿Dónde están los objetos que ha fotografiado el ‘James Webb’?
    Rosaly Lopes, la persona que más volcanes ha descubierto: “Puede haber vida en Titán” 
    Japón, Taiwán y China: una lección democrática de los chips
    Google News está de vuelta en España: qué es y cómo exprimirlo al máximo
    Jorge Stolfi: “Soy catedrático de informática. Como mis colegas, sé que la tecnología de bitcoin es basura”
    El Real Madrid de baloncesto cierra su primer fichaje: Dzanan Musa
    España postula las sedes para el Mundial de fútbol de 2030
    Los penalti-córners de Australia condenan a España en el Mundial de hockey hierba
    Un crimen entre plantas y aristócratas cierra la saga policiaca de José María Guelbenzu
    El cine del Sahel lucha por que se escuche su voz
    El Liceo cierra la temporada con la ‘Norma’ de Bellini envuelta en más de mil crucifijos
    Los audios y la España que no tuitea
    “¿Qué harías tú?”: de cómo Kim Wexler y Jimmy McGill encarnaron el amor no romántico en televisión’, por Laura Fernández
    ‘El caso Hartung’ o la calidad de las series nórdicas’, por Ángel S. Harguindey
    Edurne cancela su gira por un problema de salud
    Khloé Kardashian espera su segundo hijo con su expareja, Tristan Thompson, por vientre de alquiler
    Louboutin: “Llevo 30 años haciendo zapatos de tacón para hombres. La moda sin género no es nueva para mí”
    La bala perdida que encontró a Mirlande: “Apenas tenía un hilo de vida cuando llegó”
    La importancia de aprender en la propia lengua en un país que tiene 12 oficiales
    El multigalardonado director de fotografía que consiguió trabajo en la cola de un cine 
    Andaluz no: ‘Andalûh’
    «Me cansé de señores mirando como si no hubiese más pechos en el mundo»: así es hoy la batalla del toples en España
    De Olivia de Havilland a Raquel Welch: el biquini estuvo solo permitido a las grandes divas
    Róisín Murphy: “Los gays entienden la opresión de las mujeres. No se detienen ante nada”
    Rebecca Makkai: “Solo los extremistas creen que no se puede escribir desde otros puntos de vista”
    Ocho pueblos bonitos y fresquitos en España para escapar de la ola de calor
    24 horas en la austriaca Bregenz, el lugar donde ver una ópera flotante y comer un ‘schnitzel’
    Maneras de vivir después de muerto
    Perder el tiempo, ganar la vida: un elogio de la distracción
    El banquero más poderoso del mundo: “Las cosas pueden ir mucho peor”
    Vecinos al borde de un ataque de nervios: morosos que usan la piscina, trasteros que son despensas y ruidos diarios
    Granito y nación: el papel de los monumentos a los caídos por Dios y por España 
    Cómo el cine transformó a las diosas mitológicas en superheroínas
    Florentino Pérez recibe su nuevo coche oficial
    ‘Renting’ o ‘leasing’: ¿cuál es la mejor opción para conductores particulares?
    Judías con chermoula, aceitunas y picatostes
    Cómo hacer fideuá como si fueras de Gandía
    Guélfand reina en León por 2º año seguido, a los 54, tras más de cuatro horas trepidantes
    Videoanálisis | Una gran oportunidad perdida para sacar el ajedrez a la calle
    Cada día nuevos crucigramas, sudokus y sopas de letras
    Renueva colchón con estos de Ikea que ahora tienen 50 euros de rebaja
    Probamos las mejores planchas para pelo corto: la mejor, la más barata
    Nueve sartenes sin teflón ni tóxicos para renovar tu cocina con hasta un 38% de rebaja
    Los mejores aires acondicionados portátiles para sobrellevar el calor
    Este bañador de hombre con secado rápido es el más vendido en Amazon 
    Caos aeroportuario en Europa: estos son los destinos con más retrasos y cancelaciones
    La Comunidad de Madrid quiere cobrar 400 euros a una mujer por el tiempo que dejó la residencia para irse con sus hijas
    Un diputado pide la palabra, Batet le da tres minutos y nadie vio venir lo que iba a pasar
    Juguetes más rotos que nunca
    Lorazepam y circo. De Twitch a Ferreras, entretener para un mundo feliz
    El Señor de los Anillos: Los Anillos de Poder ilumina la Tierra Media con su épico segundo tráiler
    

## Realizamos los mismos pasos para los siguientes titulares

## Impresión de titulares de la sección de Opinión de EL PAÍS


```python
req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Mario Draghi dimite como primer ministro y aboca a Italia a una nueva crisis política 
    La primera semana de primarias en el Partido Conservador británico confirma el liderazgo de Sunak
    El presidente de Sri Lanka renuncia al cargo tras su huida a Singapur
    Pactos con el diablo
    Lo que el Indo-Pacífico le debe a Abe
    La guerra de Ucrania durará
    Goodbye, Boris?
    Shinzo Abe transformó y transformará Japón
    Macron prepara un plan de ahorro energético ante una Rusia que usa el gas como “arma de guerra”
    El irresistible ascenso de Penny Mordaunt en las primarias del Partido Conservador del Reino Unido
    La subida de precios dispara las protestas en África
    La oleada de incendios en Portugal deja ya un saldo de 813 fuegos, un fallecido y 135 heridos
    Biden reafirma en Israel el “compromiso inquebrantable” con su seguridad
    Ucrania y Rusia logran los primeros avances en la negociación para desbloquear el cereal ucranio
    Bruselas reclama a Hungría y Polonia pasos decididos para cumplir con los valores europeos 
    Seis candidatos se disputarán el liderazgo conservador en el Reino Unido con el exministro Sunak como favorito
    Alemania autoriza la puesta en marcha de sus centrales de carbón ya jubiladas para ahorrar gas 
    El Gobierno de Sri Lanka impone el estado de emergencia en la isla tras la huida del presidente
    El campo argentino se alza contra el Gobierno de Alberto Fernández
    El campo argentino se alza contra el Gobierno de Alberto Fernández
    John Bolton, exasesor de Trump, admite que ayudó a organizar golpes de Estado en otros países
    La muerte de un turista en un accidente empaña la relación entre Argentina y Bolivia
    Matanza de Uvalde: un vídeo revela la irrupción del asesino y la inacción de la policía 
    El comité del 6 de enero prueba que Trump planeó días antes la marcha al Capitolio 
    

## Impresión de titulares de la sección de España en el EL PAÍS


```python
req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')

tags = soup4.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    El abogado de la UE da la razón a España frente a Belgica y abre la puerta a la entrega de Puigdemont
    ¿Y ahora qué? Plazos, condiciones y escenarios del futuro judicial de Puigdemont
    Todas las Españas posibles en 138 propuestas
    Ante la crisis, ¿gestionas o lideras?
    El almirante Cervera y el honor de España
    El Gran Retroceso
    Santa Bárbara y la cultura de la defensa
    ¿Es posible disentir de esta retórica belicista?
    El PSOE da de plazo al Poder Judicial hasta el 13 de septiembre para renovar el Constitucional
    Sánchez logra apoyos a su plan fiscal pero Podemos y otros socios piden más
    La Comisión Europea avisa de que el bloqueo del Poder Judicial empieza a afectar al funcionamiento de la justicia
    Feijóo provoca una foto con víctimas del terrorismo en pleno debate de la ley de memoria para sugerir su desacuerdo
    La Audiencia Nacional impulsa una séptima investigación contra la excúpula de ETA
    Un tribunal ordena investigar a dos guardias civiles por supuesta complicidad con un confidente condenado por narcotráfico
    Aumentan a tres los detenidos por la muerte de la mujer arrojada a una alcantarilla en Málaga
    El PP cede a Vox un puesto en la Mesa del Parlamento andaluz y espera a cambio “generosidad”
    El incendio de la comarca de Las Hurdes se reactiva en una zona “crítica”
    La Eurocámara solicita a Marlaska que comparezca por la tragedia de Melilla
    Un organismo marroquí culpa a las autoridades españolas de no socorrer a los migrantes muertos en Melilla
    Un paraíso en el que avistar más de 20 especies de cetáceos
    El secreto de Fuerteventura se hace viral: la ‘playa de las palomitas’
    Un vino para triunfar entre los mileniales
    Artesanía y cultura que conquista a las ‘influencers’
    Más allá de la capital. El triunfo de la vida rural madrileña
    

## Impresión de titulares de la sección de economía de EL PAÍS


```python
req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')

tags = soup5.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Bruselas pide restringir desde este verano el consumo de gas ante la crisis energética 
    Bruselas eleva al 8,1% la previsión de inflación para España en 2022, pero mantiene la estimación de PIB en el 4%
    El tope a la actualización del alquiler ahorra hasta 1.000 euros a los inquilinos
    Amancio Ortega compra un rascacielos de viviendas en Nueva York por 500 millones
    Respuestas urgentes para proteger a los latinoamericanos de la crisis mundial de los precios de los alimentos
    Paridad inquietante
    El Supremo, contra los consumidores
    Las Bolsas y la ‘Quinta’ de Chaikovski
    Empresas grandes y sueldos diferentes
    Los nuevos impuestos, en el resto de Europa: cada vez más habituales sobre las energéticas; muy escasos sobre la banca
    BBVA alerta de una moderada caída de la actividad a final de año
    El Gobierno prohibirá a la banca y las energéticas que repercutan los impuestos extraordinarios a los ciudadanos 
    Los supermercados Dia venden un 8,5% más en el primer semestre, con más peso de las marcas propias
    Ketonico o cómo hacer negocio con la dieta keto
    El sector de la cerveza aumentó sus ventas un 9% en 2021, pero se mantiene por debajo del nivel prepandemia
    El banquero de inversión que ha lanzado un comparador de residencias de mayores con el que factura 2,5 millones de euros
    Ifema Madrid recupera las cifras prepandemia 
    El teletrabajo tras la pandemia
    La inflación de Estados Unidos se descontrola, escala hasta un nuevo récord del 9,1% y mete presión a la Fed
    El INE confirma el peor dato de inflación en 37 años tras una subida de los carburantes del 40%
    Jamie Dimon, el banquero más poderoso del mundo: “Los problemas económicos no son pasajeros. Las cosas pueden ir mucho peor”
    Ezentis se asoma al precipicio
    Vecinos al borde de un ataque de nervios: morosos que usan la piscina, trasteros que son despensas y ruidos diarios
    Caso Laso: ¿Me pueden echar tras sufrir un infarto?
    Remite el riesgo de estanflación
    Caos aeroportuario en Europa: estos son los destinos con más retrasos y cancelaciones
    El efecto Letizia (e hijas) en las marcas de moda españolas
    Cellnex reactiva su estrategia de crecimiento tras el adiós a Deutsche
    Los grandes analistas ya disparan la inflación media de 2022 por encima del 8%
    El préstamo pedido por un matrimonio sólo lo paga el cónyuge que lo utilizó
    No se puede desheredar a un familiar con el que no se tiene relación, según el Supremo
    Líos en la piscina comunitaria: normas y sentencias para un chapuzón seguro
    Estudiar en el extranjero, una inversión que mejora la empleabilidad y las competencias interpersonales
    Música que transforma vidas y esboza futuros
    El futuro probable de una sociedad insostenible
    La hora del bienestar corporativo
    Cancerberos del bienestar de la empresa
    Cómo garantizar la seguridad en un mundo de amenazas híbridas
    ¿Cuáles son los dilemas éticos del uso de la inteligencia artificial?
    Las aventuras de un par de calcetines que dan empleo a todo un pueblo
    Cultura financiera como punto de partida para volver a empezar
    ¿Puede convertirse España en una de las potencias logísticas del futuro?
    Por qué digitalizar una pyme aporta más empleo
    ‘Coopetir’: la actitud DFactory
    Así serán las ciudades de la (nueva) última milla
    Cinco errores habituales al digitalizar un negocio 
    PERTE Agroalimentario: ¿cómo acceder a los fondos europeos?
    Fondos soberanos: ¿Cómo funcionan las cajas fuertes de los estados más ricos?
    ¿Crisis de deuda mundial a la vista?
    El método Muñoz para triunfar en cada reto que se propone
    Gloria Ramos, cuando el afán de superación acaba en la alfombra roja 
    Ocho ‘startups’ innovadoras con nombre propio
    Hotmart y su plataforma 360 para creadores de contenidos
    

## Impresión de titulares de la sección sociedad de EL PAÍS


```python
req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')

tags = soup6.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    El 20% de las playas españolas quieren ser “libres de humos”, pero solo en una minoría está prohibido fumar
    Estos serán los tutores legales del mar Menor encargados de su representación y gobernanza
    Un nuevo modelo de residencias para las próximas generaciones de personas mayores: que sean como casas
    Un nuevo modelo de residencias para las próximas generaciones de personas mayores: que sean como casas
    Becas para ricos mezcladas con aborto
    Educación híbrida: de la emergencia a la transformación 
    Jóvenes atrapados en el efecto cicatriz
    Un campus privado de Santander fracasa en su intento de frenar la criba de calidad universitaria
    Kevin Spacey se declara “no culpable” de los delitos de abusos sexuales que se le imputan en el Reino Unido
    El Constitucional amplía las posibilidades de acceder a la justicia gratuita a personas discapacitadas por un accidente
    El Constitucional anula parte de la ley de Castilla y León que permitía cazar al lobo 
    Un sevillano que solicitó la eutanasia recurre al suicidio ante la falta de protocolos claros de la Junta de Andalucía
    Las becas de Ayuso hacen saltar por los aires los tensos juegos de alianzas y equilibrios en la enseñanza privada de Madrid
    Las claves de una ola de calor que desafía todos los récords de intensidad, extensión y duración
    Los sanfermines de este año registran su primera denuncia por violación
    Pamplona sale a la calle contra la violación denunciada el sábado en San Fermín
    Hong Kong impondrá un brazalete electrónico para controlar las cuarentenas en casa de positivos de coronavirus
    El Tribunal Supremo avala el indulto parcial de Juana Rivas
    Residuos para mover el mundo
    Se buscan profesionales en economía circular
    ¿Por qué hablar de VIH en el Orgullo y no en los sanfermines?
    Mitos, falsedades, bulos y realidades sobre el VIH 40 años después
    Qué son las evidencias científicas y por qué están revolucionando la educación
    Munic, el joven redimido por el trap
    ¿Cuándo unos kilos de más empiezan a ser un problema serio?
    Interactivo | Los 14 cambios en los aeropuertos españoles que no ves y que ya están ocurriendo
    Encontrar empleo pese a los obstáculos. Por dónde empezar la búsqueda
    La fórmula de Carboneros para evitar el éxodo rural: trabajar cuidando a los vecinos 
    Consejos y cuidados para el primer verano con un gatito o un perrito
    ¿Qué tienen en común perros y gatos cuando son cachorros?
    La guía definitiva para alimentarnos mejor (y cuidar nuestra salud y la del planeta)
    El metro como refugio. De los andenes de Madrid en 1936 a los de Kiev en 2022
    La salud mental de los refugiados: cómo abrirse para cerrar las heridas
    Yogures con menos azúcar, paso firme hacia la alimentación infantil del futuro
    Conectada con el mercado laboral y tecnológica: así es la universidad del presente
    Así es la formación más abierta y flexible, a prueba de crisis
    

## Impresión de titulares para la sección educación de EL PAÍS


```python
req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')

tags = soup7.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Un campus privado de Santander fracasa en su intento de frenar la criba de calidad universitaria
    Becas para ricos mezcladas con aborto
    Las becas de Ayuso hacen saltar por los aires los tensos juegos de alianzas y equilibrios en la enseñanza privada de Madrid
    La importancia de aprender en la propia lengua en un país que tiene 12 oficiales
    Estudiar en el extranjero, una inversión que mejora la empleabilidad y las competencias interpersonales
    El deporte ya no es solo deporte: el sector atrae todo tipo de perfiles profesionales
    Educación híbrida: de la emergencia a la transformación 
    Gabriela Ossenbach, experta en manuales escolares: “Con los libros de texto se puede crear fácilmente alarma social, pero no está justificada”
    La libertad guiando (dicen) a la escuela
    Intento de rebelión de los directores de primaria de Cataluña por los nuevos horarios de septiembre
    La escalada vertiginosa de notas en Bachillerato: los sobresalientes de los que llegan a Selectividad se doblan en seis años
    Sin currículos
    La escuela concertada ante las desigualdades: el debate pendiente
    La equidad frente a las políticas educativas de privatización en Andalucía
    No hay lunes al sol en la Universidad
    El nuevo sistema para evaluar los conocimientos digitales de los profesores valdrá en toda España
    Ofrecer comedor gratis en todos los colegios públicos es “alcanzable y urgente”: costaría 1.664 millones al año, según la ONG Educo  
    Una fórmula para que la escuela pública compita mejor con la concertada
    La pérdida de alumnos por el descenso de la natalidad está afectando con más fuerza a la escuela pública que a la concertada
    La escalada vertiginosa de notas en Bachillerato: los sobresalientes de los que llegan a Selectividad se doblan en seis años
    El caso de Georgia, en EE UU: becar sin importar la renta agranda la desigualdad
    El techo de cristal del grado medio de FP: candidatos demasiado preparados se quedan con los puestos
    La implantación del nuevo Bachillerato general fracasa pese a su demanda potencial: “Creímos que lo pedirían seis alumnos y lo han hecho 27”
    Toni Solano, director de instituto: “Veo mal a los niños, necesitan muchísima ayuda”
    Ayuso se apunta ahora el tanto de la bajada de tasas universitarias, pese a que las llevó a los tribunales para no reducirlas
    Una historia en la que caben Alaska, García Lorca, Suárez y Popper: la Universidad Internacional Menéndez Pelayo cumple 90 años 
    Subirats reinterpreta la ley de Universidades: freno a la precariedad, facilidades para los alumnos extranjeros y ciencia abierta
    Las universitarias desertan del grado de Matemáticas ahora que tiene pleno empleo. ¿Por qué?
    “La clave contra el racismo es la empatía”
    Las infinitas posibilidades de un tablero de ajedrez
    “No hay pensamiento sin tiempo para pensar”
    

## Impresión de la sección de titulares de medio ambiente para EL PAÍS


```python
req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')

tags = soup8.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Estos serán los tutores legales del mar Menor encargados de su representación y gobernanza
    Alemania autoriza la puesta en marcha de sus centrales de carbón ya jubiladas para ahorrar gas 
    El Constitucional anula parte de la ley de Castilla y León que permitía cazar al lobo 
    Las claves de una ola de calor que desafía todos los récords de intensidad, extensión y duración
    Absuelto un conductor que se dio a la fuga tras arrollar a un ciclista: “Te sientes atropellado por el coche y la justicia”
    El incendio en la comarca cacereña de Las Hurdes sigue sin control tras el desalojo de 400 personas
    La ola de calor alcanza su cenit con avisos rojos en Andalucía y Extremadura por 44° y en Galicia por 42°
    Juan Carlos Blanco: “Ahora es casi imposible encontrar un cuento sobre un lobo malo”
    Si convence a un tercio de sus vecinos puede poner placas solares en la azotea: “El autoconsumo colectivo es imparable”
    El Papa urge a los jóvenes a comer menos carne “para salvar el medio ambiente”
    Segunda ola calor del verano: al menos cuatro días con máximas de hasta 46° y noches tórridas a más de 25°
    Un plan de retirada  
    Crisis energética y precios del carbono
    La lección del martín pescador para afrontar la crisis ecológica
    Estocolmo+50: mirar atrás para tomar impulso
    Ríos imposibles: las 171.000 barreras que rompen el curso de agua en España
    La UE abraza las renovables para romper la dependencia de Rusia
    La lucha en un pueblo de Teruel para salvar su última montaña
    ¿Qué aire respiran los niños de Madrid y Barcelona? En el 46% de los colegios se supera la contaminación permitida
    “La clave contra el racismo es la empatía”
    Las infinitas posibilidades de un tablero de ajedrez
    “No hay pensamiento sin tiempo para pensar”
    

## Impresión de la sección de titulares de Ciencia de EL PAÍS


```python
req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')

tags = soup9.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Los universitarios miden tres centímetros más que los que solo tienen estudios de primaria
    Con el pasado por delante desde la sierra de Atapuerca
    Descubierto el principio matemático detrás de los escutoides, las formas geométricas de moda
    Planetas brumosos y galaxias ultradifusas: el telescopio ‘James Webb’ comienza a responder preguntas fantásticas
    ¿Dónde están los objetos que ha fotografiado el ‘James Webb’?
    Las nuevas imágenes del telescopio ‘James Webb’ muestran planetas gigantes, estrellas agonizantes y galaxias chocando a altísima velocidad
    El telescopio ‘James Webb’ desvela miles de galaxias en el universo profundo, en su primera imagen a todo color
    Alberto Ascherio, médico: “Si no tienes el virus de la enfermedad del beso, tu riesgo de desarrollar esclerosis múltiple es prácticamente cero”
    Óscar Marín, neurocientífico: “Variando pequeñas piezas de la corteza cerebral se generan capacidades de superhéroe”
    La ingeniera que enseña a nuestro cuerpo a autorrepararse: “Hemos regenerado piel, cartílagos y vasos sanguíneos, pero todavía tenemos que hacer más”
    Los Premios SEIO-Fundación BBVA 2022 reconocen cinco contribuciones españolas de alto impacto en la ciencia de datos
    El tabú de la menopausia: “Hay vergüenza, preocupa ser identificadas como viejas o incapaces”
    El ‘James Webb’ se prepara para su gran hito: las primeras imágenes
    Mar Castellanos, neuróloga: “El ictus afecta cada vez más a personas en edad laboral. Las enfermedades cardiovasculares son una epidemia”
    ¿Es la consciencia una ilusión intrascendente?
    Óvulos que se agotan y declive del esperma: todo lo que ignoramos sobre fertilidad hasta el momento de querer hijos
    Planetas brumosos y galaxias ultradifusas: el telescopio ‘James Webb’ comienza a responder preguntas fantásticas
    Las mentes humanas detrás de las mentes artificiales
    Matemáticas para describir los remolinos, los taxis del océano
    Reaparece la tesis de María Wonenburger, la pionera matemática española que permaneció décadas en el olvido
    Técnicas criptográficas que se fundamentan en lo impredecible
    Alrededor de la mesa
    Fracciones egipcias
    El problema del huerto
    Con el pasado por delante desde la sierra de Atapuerca
    La cola vestigial, el apéndice oculto del hombre que venció a Napoleón en Waterloo
    Molinos y gigantes, adelantos tecnológicos y el síndrome bicicleta
    El síndrome del hombre lobo y la realidad lógica de su fábula
    La locura como juego; más allá del Quijote y de las novelas de Pérez Galdós
    ¿Son mejores las hormonas bioidénticas?
    ¿Qué surgió antes, el ARN o el ADN?
    ¿Por qué se sabe que los núcleos de la Tierra rotan?
    ¿Qué son los mini reactores nucleares?
    Invitados indeseables por Navidad: el muérdago y otras plagas que evitar durante las fiestas
    Las ‘apps’ nutricionales o cómo comer bien no debería depender de uno mismo
    Malnutrición invisible: el impacto de la pobreza en la salud infantil
    El óxido de etileno, la sustancia cancerígena que ha obligado a retirar miles de alimentos en la UE
    Que no te líen con los ingredientes: aceites y grasas de mala calidad nutricional
    

## Impresión de titulares de la sección cultura de El País


```python
req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')

tags = soup10.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    La segunda muerte de Vicente Aleixandre, la segunda ruina de Velintonia
    Gustavo Gimeno será el nuevo director musical del Teatro Real en 2025
    Descubierto un autorretrato de Van Gogh oculto en la parte de atrás de un lienzo fechado en 1885
    El libro que vendrá
    Fallecimiento de José Guirao: Con las alas de la cultura
    Muerte de José Guirao: Poner nombre a los árboles 		 
    Fallecimiento de José Guirao: A tu sonrisa, Pepe
    El Bono Joven Cultural se pone en marcha a finales de julio  
    Muere el periodista Eugenio Scalfari, fundador del diario italiano ‘La Repubblica’, a los 98 años
    El cine del Sahel lucha por que se escuche su voz
    Un crimen entre plantas y aristócratas cierra la saga policiaca de José María Guelbenzu
    Donna Leon: “Los trabajadores de un almacén de Amazon son los esclavos de hoy”
    Dos generaciones de periodistas ante la crisis de la profesión: “Ningún tiempo pasado fue mejor”
    Irán encarcela a Jafar Panahi, Mohammad Rasoulof y Mostafa Al-Ahmad, tres de sus cineastas más aclamados
    La cancelación del festival Diversity deja a Valencia sin la actuación de Iggy Pop, Christina Aguilera y Karol G 
    Los promotores del Hermitage de Barcelona reclaman 141 millones de euros al Ayuntamiento
    Carmen Calvo, premio Julio Gónzalez 2022: “Falta premiar a muchas mujeres”
    Cuando el teatro es XXL: ¿quién teme una obra de 13 horas?
    El Guggenheim de Bilbao afronta una ola de críticas por un cuadro idéntico a un fotograma
    Marta D. Riezu y ‘Agua y jabón’, el triunfo de lo de toda la vida
    Cuándo un gallego te dice que sí, aunque esté pensando que no. La retranca gallega y otros misterios que descubrir en el Camino Inglés
    El último atardecer de Europa se ve solo desde este lugar. Un viaje hacia el infinito por el Camino de Fisterra-Muxía
    Lorca, en la ciudad al margen
    El Pirineo oscense, para entrar a vivir
    Toda la lectura del verano, en el bolsillo
    Longsellers: los libros más vendidos a lo largo de la historia
    Libros para descubrir el mundo recomendados por Benjamín Prado
    Descubre la muestra de Paret en el Museo del Prado
    ‘¡Chakapum!’, un espectáculo de El Terrat
    Disfruta en cines de 'Un escándalo de Estado'
    Descubre el 'Museo Oculto' del Reina Sofía
    Octavo encierro de San Fermín 2022, en imágenes
    Un herido leve y cinco contusiones en el octavo, rápido y último encierro de San Fermín
    La importancia de caer de pie
    Seis contusionados en un rapidísimo séptimo encierro de San Fermín
    

## Imprsión para la sección de Babelia de EL PAÍS


```python
req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')

tags = soup11.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    La maternidad en imágenes: del miedo y la rabia a la aceptación
    Granito y nación: el papel de los monumentos a los caídos por Dios y por España 
    Cómo el cine transformó a las diosas mitológicas en superheroínas
    Tristes, drogados, periféricos: la nueva literatura que refleja el dolor de los polígonos
    La fuga de Siberia de Trotsky, la revelación de Marta D. Riezu y otros libros de la semana
    El desvío experimental de Perfume Genius, los salmos de Nick Cave y otros discos del mes
    Jardines secretos en la jungla de asfalto: cómo resistir a la especulación plantando un árbol
    Los nuevos diaristas son vendedores de vidas
    La ‘Safo’ de Christina Rosenvinge no convence
    La gran música eleva a una compañía de danza inmadura
    Trampantojo: De veraneo
    Un clavo quita otro, quizás
    Músicas ocultas
    Lo que siento (no se olviden de Ucrania) 
    No eran marcianos, eran humanos
    ‘La máquina de proyectar sueños’, un retorno a la infancia delicioso y temible
    ‘Veinte años de Sol’ o cómo olvidar el pasado con un implante en el cerebro
    ‘La fuga de Siberia en un trineo de renos’, de Trotsky: aventuras de un comunista en plena huida 
    ‘Magallanes & Co.’, los preparativos y aventuras de la primera vuelta al mundo
    Silvia Agüero: “De no ser escritora habría sido vendedora ambulante”
    Antoni Muntadas: “Supe que me dedicaría al arte cuando dejé de pintar”
    Manuel Estrada: “Me agrada que una portada guste más después de leer el libro”
    Óscar Esquivias: “No hace falta ser creyente para leer la Biblia”
    Amelia Castilla: “Los ritos nos ayudan a hacer viable el trance de la muerte”
    

## Impresión de titulares para la sección de deportes de EL PAÍS


```python
req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')

tags = soup12.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

```

    Pidcock triunfa en Alpe d’Huez y Vingegaard afianza el liderato en el Tour de Francia
    Las 200 subidas más rápidas a Alpe d’Huez: solo Pantani bajó de los 37 minutos en la era del dopaje 
    Xavi gana el pulso por Dembélé 
    Con Tiger Woods nunca se sabe
    Las tribulaciones de Cristiano Ronaldo pasan por Qatar  
    Cuánto tarda en hervir un Tour
    El tenis es, ante todo, repetición
    Damaris Egurrola, la futbolista que se fue dos veces de España
    Saint Andrews es el golf
    El Real Madrid de baloncesto cierra su primer fichaje: Dzanan Musa
    España postula las sedes para el Mundial de fútbol de 2030
    El Mundial de Atletismo vuelve a su esencia
    Los penalti-córners de Australia condenan a España en el Mundial de hockey hierba
    Vingegaard derrota a Pogacar en la primera gran etapa del Tour de Francia
    Último día de amarillo en los Alpes para Pogacar
    Antoine Blondin: 21 curvas de tinta y épica
    Raphinha eleva la nota media del Barça
    Toma y daca por Alex Palou
    Suzuki oficializa su marcha del Mundial de MotoGP
    Aitana Bonmatí: “Tenemos que ser más exigentes”
    “Si no tenemos en quién mirarnos es muy difícil saber qué queremos ser”
    “Nunca acepto un no por respuesta”
    La nadadora que dejó de competir para hacer campeones de básquet
    Crónica de dos ciudades moldeadas por la misma pasión 
    La Noruega quebrada de Hegerberg, ante el espejo
    Eurocopa femenina 2022 | España cae ante Alemania y se jugará el pase a cuartos ante Dinamarca
    Golpe de realidad para España ante Alemania
    La UEFA: “La Superliga fracasó porque los aficionados europeos aprecian el sistema actual”
    El vigor de Guélfand a los 54
    Luis León ataca, pero la etapa del Tour de Francia la gana Cort y Pogacar no suelta el amarillo
    El campeón olímpico Mo Farah revela que fue víctima de tráfico ilegal y explotación en Reino Unido
    El viaje de Jon Rahm a Saint Andrews: de la furgoneta a Seve
    

## Impresión de titulares para la sección de tecnología de EL PAÍS


```python
req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')

tags = soup13.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    “Si envolvemos a nuestros hijos en algodón digital, no aprenderán a sobrellevar los problemas”
    El hidrógeno aspira a reemplazar al petróleo y el gas en el abastecimiento local de energía
    Japón, Taiwán y China: una lección democrática de los chips
    Google News está de vuelta en España: qué es y cómo exprimirlo al máximo
    Dialexis (‘mater ex machina’)
    La ingeniera que enseña a nuestro cuerpo a autorrepararse: “Hemos regenerado piel, cartílagos y vasos sanguíneos, pero todavía tenemos que hacer más”
    La inteligencia artificial de Google es capaz de aprender como un bebé
    Las activistas que dejaron sin anuncios a la web de Steve Bannon van ahora a por Fox News
    “¿Quieres cobrar tu salario en streaming?” Por qué los proyectos cripto son tan difíciles de entender
    El misterio de la carta del soldado alemán
    El porqué de los desafíos criptográficos: conocerte a ti mismo, conocer a tu enemigo
    Con el relax del verano se acentúan los peligros cibernéticos: así puede protegerse durante las vacaciones
    Meta presenta un traductor capaz de operar en tiempo real con 200 idiomas
    “Soy catedrático de informática. Como mis colegas, sé que la tecnología de bitcoin es basura”
    El sector biotecnológico supera las cifras de 2020 y capta 180 millones de euros de inversión privada
    En defensa de la procrastinación. Elogio del tiempo perdido (frente al que las redes te roban)
    Instagram, el mejor de los mundos posibles
    Del terrorismo youtuber al influencer rabioso: el odio inunda la red
    Cronodiversidad. ¿Por qué el tiempo cada vez va más rápido?
    El impacto de la tecnología en la hostelería: de la comanda digital al pago con código QR
    Herramientas que ayudan a crecer a las empresas (más allá de los pagos)
    Cinco razones por las que este ‘smartphone’ es sencillamente tentador
    La cámara de este ‘smartphone’ es pura magia
    Ciberseguridad para todos los públicos, en siete capítulos
    Un campus de programación para adquirir todas las habilidades ‘tech’
    

## Impresión de la sección de titulares para la sección gente de EL PAÍS


```python
req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')

tags = soup15.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Armie Hammer, de estrella de Hollywood y acusaciones caníbales a vender multipropiedades en las islas Caimán
    Ana de Armas y el prejuicio latino: “Creí que era una joven poco sofisticada”, reconoce sobre ella Jamie Lee Curtis
    Khloé Kardashian espera su segundo hijo con su expareja, Tristan Thompson, por vientre de alquiler
    Kate Moss vuelve a ser musa de Zara: la modelo llena de glamur y nocturnidad la última campaña de la firma
    Edurne cancela su gira por un problema de salud
    Aurelio Morales, el hombre que dejó una estrella Michelin para tomar impulso y ganar tres
    Deslenguada y cazafortunas: reivindicando a la primera Barbie de la historia en tiempos de ‘Barbiecore’
    Mickey Rourke, sobre Tom Cruise: “Lleva interpretando el mismo papel 35 años. No le tengo respeto”
    Christian Louboutin: “Llevo 30 años haciendo zapatos de tacón para hombres. La moda sin género no es algo nuevo para mí”
    Jason Alexander se declara no culpable de acechar a Britney Spears tras irrumpir en su boda y se enfrenta a cinco años de cárcel
    Charlene de Mónaco, guía turística en el palacio real de Montecarlo
    La DJ B Jones, de las noches en la carretera al olimpo de la música electrónica: “Ahora somos el centro de la fiesta” 
    Marilyn Monroe hizo ricos a muchos hombres mientras se empobrecía: “No tuvo ni para un funeral decente”
    La cumbre de la alpargata
    Pietro Beccari: “El desfile de Sevilla es uno de los mejores, si no el mejor, que ha hecho Maria Grazia Chiuri en Dior”
    El espectáculo (teatral) debe continuar en la alta costura de París
    Realismo, entretenimiento y democracia: la alta costura se deshace por fin de sus estereotipos en París
    Nostalgia ‘retro’, punto multicolor y otras pistas para vestir este verano
    La cocinera que trasladó las flores del jarrón al plato
    En verano, el mejor queso del mundo se hace helado
    El placer de lo rancio y otros gustos y aromas que recuerdan la niñez
    Trece aperitivos
    

## Impresión de titulares para la sección EPS de EL PAÍS


```python
req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')

tags = soup17.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    No hacerlo todo juntos: claves para que agosto no se convierta en el mes de los divorcios
    El multigalardonado director de fotografía que consiguió trabajo en la cola de un cine 
    Un servicio médico en cualquier lugar y momento
    Andaluz no: ‘Andalûh’
    Carme Elías: “Me siento más ligera que nunca, como si la vida me hubiera preparado para este momento”
    El resurgir del turismo
    Orgullo con todas las letras
    El restaurante madrileño en el que la cocina gaditana y la francesa se enamoraron
    ¿Dónde está exactamente el origen del mal?
    Las heridas abiertas de la infancia en Irak
    Pietro Beccari: “El desfile de Sevilla es uno de los mejores, si no el mejor, que ha hecho Maria Grazia Chiuri en Dior”
    El hombre que persigue la gaita más antigua del mundo
    La uva más denostada de  Castilla-La Mancha resurge de sus cenizas
    Hyundai Ioniq 6: la tecnología al servicio del automóvil
    El engaño a los ojos
    Reír a lágrima viva
    Las fiestas de la sangre
    Libros sin Feria
    Harina enriquecida para acabar con el “hambre oculta”
    Lugares de esperanza para salvar los océanos
    Los guardianes del clima que llevan medio siglo leyendo las advertencias de los glaciares
    Epidemia de violencia: claves del negocio de las armas en Estados Unidos
    Los ejecutivos voladores y la ética medioambiental
    Ibiza, entre la noche desenfrenada y el turismo tranquilo 
    Luz Casal: “Tengo el alma rockera. Nada ha doblegado mi rebeldía”
    Rashid Johnson: “Los pensadores y creadores negros estamos cansados de que nos nieguen un espacio autónomo”
    Sergio Hernández: “En el mundo, la gente ya no quiere verdades, quiere mentiras”
    Elvira Sastre: “No hay que perdonarlo todo”
    La trinidad del taco perfecto: “Buena tortilla, delicioso relleno y una salsa sabrosa”
    La casa de Nina Urgell Cloquell, un piso en el que las paredes hablan
    Garbanzos verdes y puchero
    Bikôkô y Julio Peña, dos estrellas en ebullición  
    Cuando Chufy encontró a Rossy: dos amigas, una isla y una colección de moda
    República Dominicana, donde la vida fluye por el río infinito
    Retrato Robot 
    Ilusiones hipnóticas
    El poder del hormigón
    ‘Fantasías en el Prado’, por Alberto García-Alix
    

## Titulares con las palabras más buscadas

En esta parte usaremos os.system(clear) para se haga una limpieza después de realizar el web scrapping.


```python
os.system("clear")
```




    1




```python
print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))

print(colored("Igualdad", 'green', attrs=['bold']))

str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))

print(colored("Mujeres", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))

print(colored("Mujer", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))

print(colored("Brecha salarial", 'green', attrs=['bold']))

str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))

print(colored("Machismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))

print(colored("Violencia", 'green', attrs=['bold']))

str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))

print(colored("Maltrato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))

print(colored("Homicidio", 'green', attrs=['bold']))

str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))

print(colored("Género", 'green', attrs=['bold']))

str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))

print(colored("Asesinato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))

print(colored("Sexo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))

```

    [1m[34mA continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:[0m
    [1m[32mFeminismo[0m
    
    [1m[32mIgualdad[0m
    La escuela concertada ante las desigualdades: el debate pendiente
    El caso de Georgia, en EE UU: becar sin importar la renta agranda la desigualdad
    [1m[32mMujeres[0m
    Róisín Murphy: “Los gays entienden la opresión de las mujeres. No se detienen ante nada”
    Carmen Calvo, premio Julio Gónzalez 2022: “Falta premiar a muchas mujeres”
    [1m[32mMujer[0m
    Aumentan a tres los detenidos por la muerte de la mujer arrojada a una alcantarilla en Málaga
    Róisín Murphy: “Los gays entienden la opresión de las mujeres. No se detienen ante nada”
    La Comunidad de Madrid quiere cobrar 400 euros a una mujer por el tiempo que dejó la residencia para irse con sus hijas
    Aumentan a tres los detenidos por la muerte de la mujer arrojada a una alcantarilla en Málaga
    Carmen Calvo, premio Julio Gónzalez 2022: “Falta premiar a muchas mujeres”
    [1m[32mBrecha salarial[0m
    
    [1m[32mMachismo[0m
    
    [1m[32mViolencia[0m
    Epidemia de violencia: claves del negocio de las armas en Estados Unidos
    [1m[32mMaltrato[0m
    
    [1m[32mHomicidio[0m
    Los homicidios en Chile escalan casi un 30% en el primer semestre de 2022
    [1m[32mGénero[0m
    Louboutin: “Llevo 30 años haciendo zapatos de tacón para hombres. La moda sin género no es nueva para mí”
    Christian Louboutin: “Llevo 30 años haciendo zapatos de tacón para hombres. La moda sin género no es algo nuevo para mí”
    [1m[32mAsesinato[0m
    
    [1m[32mSexo[0m
    
    

## Conclusión

Con la ayuda de la web scraping  podemos obtener información de forma sencilla. Este sistema automatia los sitios webs y nos permite ahorrar tiempo invertido en nuestras búsquedas y obtención de datos. Como hemos podido observar el ejemplo con el diario El País, hemos logrado obtener de forma precisa datos e información adecuada automáticamente bajo un sistema de códigos.
La idea de utilizar estas herramientas es automatizar la búsqueda y crear un sistema de códigos  fuente para acortar tiempo. Lo complejo es comprender el uso de los códigos, cuándo y cómo emplearlos.
