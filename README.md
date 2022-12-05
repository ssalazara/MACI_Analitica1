# MACI_Analitica1

# Tarea 1. 

## Web scraping, Manejo de datos y Clasificación.


**Ayudante:** Martina Cádiz (mcadiz2018@inf.udec.cl)

---


La tarea debe ser subida a la plataforma en un archivo con el formato **NombreApellido_tarea1.zip**. Este debe contener el código solicitado, junto con el conjunto de datos utilizado. 

## 1. Web scraping (47 ptos)

Una emprendedora ha comenzado su propia empresa de Notebooks y quieren dar una dura pelea a las grandes empresas como Apple, Asus, HP, etc. Para esto contrataron a una empresa consultora quien les realizo un estudio de mercado, técnico y financiero que les permitió reunir información relevante sobre la industria, el mercado, los costos de los materiales y cómo seria su rentabilidad de aquí a un cierto horizonte de tiempo. Sin embargo, a ellos también les gustaría tener información actualizada, en todo momento, de los precios de ventas de sus competidores, así como también, un análisis actual de los precios a nivel de tienda y marca. Ella no tiene conocimientos de Análisis de Datos y de Machine Learning, por ende, lo/la contrata a usted para que realice este proyecto.

En primer lugar, ella le comenta que no cuenta con una base de datos disponible para realizar algún
análisis y que le gustaría obtener información actualizada del precio al cual están vendiendo los
productos sus competidores. Además, otro de los problemas iniciales que surgieron es que no sabe
cómo estimar el precio de los móviles que fabricará su empresa, y que no le gustaría simplemente
asumir cosas. Por lo tanto, ella le solicita a usted:

1. Que genere un código que permita extraer la información de Notebooks de la página www.solotodo.cl/notebooks, ya que recopila información de varias tiendas y marcas diferentes y no tiene restricciones de extracción de datos mediante técnicas de scrapping. Debe extraer hasta la **página 90**.

2. Que averigüe alguna relación entre las funciones de los Notebooks y su precio de venta. (Luego de recopilar los datos de ventas).

### Los datos que le interesa a la emprendedora son los siguientes:

**Información que se puede extraer desde la página general:**

- Nombre Notebook (id)
- Marca Notebook

*Procesador:*
- Modelo procesador

*RAM:*
- GB
       
*Almacenamiento: (se pedirá extraer el tipo de memoria y sus GB, en caso de que tenga más de una se debe seleccionar la primera)* 
- Tipo de disco duro 
- GB
    
*Tarjeta de video:*
- Marca GPU dedicada
- GB dedicada
    
**Información que deberán extraer dentro de cada producto:**
- Tabla de precios de los computadores en las diferentes tiendas

Como habrán aprendido en clases, en el proceso de recolección de datos no siempre encontrarán toda la información en cada uno de los productos, por lo cual deberán decidir en cómo trabajar con estos tipos de datos faltantes. Para esto tendrán que explicar cada decisión tomada para la representación de estos. Para efectos de revisión, todos los datos obtenidos deberán ser guardados en un archivo ".pkl" (pickle), ya que la página es actualizada constantemente.

**Resumen:** 

En la primera parte se espera que: 
1. Extraigan la información **(15 pts)**,
2. La almacenen en un DataFrame (información y precios) **(2 pts)**,
3. Que limpien los datos **(7 pts)**, 
4. Generen las variables de interes correspondientes (columnas) **(7 pts)**,
5. Que expliquen las decisiones tomadas y guarden los datos trabajados en un archivo “.pkl” **(3 pts)**,
6. Y que respondan preguntas relacionadas a los datos **(13 pts)**.

En la segunda parte se evaluará que:
1. Preprocesen los datos **(3 pts)**,
2. Dividan los conjuntos de datos **(3 pts)**,
3. Entrenen algún algoritmo sobre los datos de entrenamiento **(5 pts)**,
4. Validen sus resultados con el uso de validación cruzada **(5 pts)**,
5. Realicen un testeo **(2 pts)**,
6. Por último que extraigan conclusiones **(5 pts)**.
