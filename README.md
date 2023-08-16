# PI2-Rol_Data_Analyst
En este repositorio se encuentra la Extracción API.jpynb y EDA.jpynb



![image](https://github.com/Leidypv/PI2-Rol_Data_Analyst/assets/122382146/1879ba47-691f-4e11-a78e-ecc7365b5f5d)

 
Bienvenidos 

Me presento, soy Leidy Parrado y mi cargo es de Data Analista con la empresa Financial Services. Se me ha encomendado el proyecto de analizar el mercado de las criptomonedas.
La empresa se ha mostrado un notable interés en este mercado debido a su crecimiento desde el 2009 y acogida a nivel mundial, El objetivo del proyecto es entender el mercado y detectar posibles oportunidades de inversión para los clientes. 
 
 Para desarrollar el proyecto, he utilizado los datos de la API CoinGecko, seleccionando 10 Criptomonedas a estudiar su comportamiento en el mercado: 
 
1.	Bitcoin (BTC)
2.	Binancecoin (BNB)
3.	Cardano (ADA)
4.	Chives-coin (CHIVES)
5.	Dogecoin (DOGE)
6.	Ethereum (ETH)
7.	Gala (GALA)
8.	Ripple (XRP)
9.	Solana (SOL)
10.	Terra Luna (LUNA)
    
1.Bitcoin: Es la primera criptomoneda que permite realizar transacciones entre personas sin necesidad de intermediario como un bancos o gobiernos.
2.Binancecoin: Se crea con el propósito de pagar transacciones dentro de la plataforma Binance y para obtener descuentos en tarifas.
3.Cardano: ADA es un token nativo, se utiliza para llevar a cabo transacciones y para participar en la red. 
4. Chives Coin: No se dispone de mucha información sobre Chives, lo que podría indicar que es un token relativamente nuevo en el mercado.
5. Dogecoin: Inicialmente nacida como una broma basada en un meme de un perro. Dogecoin ha evolucionado y se ha convertido en una moneda popular para propinas y donaciones en línea.
6. Ethereum: Su Token nativo se utiliza para pagar transacciones en la red.
7. Gala: Es el token nativo de la plataforma Gala Games, permite a los jugadores ser dueños de sus propios juegos y les brinda recompensas por jugar.
8. Ripple: Funciona tanto como plataforma de pago como criptomoneda.
9. Solana: Su token nativo se utiliza en la operación de la red
10. Terra Luna: Su token nativo se utiliza en la red 

A.   Comienzo extrayendo datos históricos del mercado, abarcando el periodo del 01/01/2020 al 01/01/2023 del mercado que incluyen precio, capitalización de mercado y volumen de 24horas, todos expresados en la moneda de cambio USD. 
Mi objetivo con este análisis histórico es obtener una visión general de la distribución y las tendencias de los precios en el mercado de las criptomonedas. Para lograrlo, he optado por utilizar estadísticas relacionadas con el precio de las criptomonedas de los datos y el diagrama de caja, que me permite identificar valores atípicos (outliers) en el mercado.
Observamos que el valor promedio es de $3425.98usd nos puede dar una idea general sobre el rango de precios en el mercado de las criptomonedas. La volatilidad con un valor de $10676.11usd, nos indica la variabilidad de los precios en relación con el promedio. Nos muestra que algunas criptomonedas tienen un precio extremadamente bajo y otras un precio muy alto. Por último, observamos la distribución de los precios en el mercado por ejemplo el 25% de las criptomonedas tienen precio menos o igual a $0.15usd mientras que el 75% se encuentra dentro del rango de $0.15usd y $288.55usd 
La elección del diagrama de caja se fundamenta en su capacidad de trabajar en conjunto con las estadísticas, me proporciona una visión rápida de la distribución de los precios y la presencia de valores atípicos. Esto me ha permitido realizar un análisis detenido de por qué algunos precios difieren. 
Basándome en el análisis estadístico, la gráfica comparativa confirma que la criptomoneda bitcoin alcanza el valor máximo de $67617.01usd, lo cual podría ser un indicio positivo para la inversión en esta criptomoneda dado su alto valor en el mercado.  

B.   El análisis es fundamental para comprender como los inversores y el mercado en general perciben la capitalización de mercado. Por tal razón Inicie la extracción de los datos de market_cap (capitalización de mercado) desde la API. 
Luego, procedí a calcular la matriz de correlación para todas las variables y elegí el mapa de calor para resaltar las correlaciones y comprender como se relacionan las variables entre sí. Cuando el valor de la correlación se acerca a 1 indica correlación positiva fuerte, mientras que un valor cercano a -1indica una correlación negativa fuerte. 
Opte por el mapa de calor porque me ayuda a identificar patrones de correlación entre diferentes variables y para resaltar tanto las relaciones más fuertes como las más débiles entre ellas. 
En el gráfico, apreciamos una fuerte correlación positiva entre la variable market_cap de las criptomonedas con mayor capitalización en el mercado y total_volume que representa un mayor volumen total de las operaciones, este es un indicador importante especialmente al considerar criptomonedas populares como bitcoin, como hemos observado en el análisis previo, nos dio indicio positivo para la inversión. 
Al comparar con los datos del dataframe(tabla), se confirma que efectivamente existe una correlación entre estos dos valores para bitcoin y ethereum, es decir cuando la capitalización de mercado aumenta para estas criptomonedas, es probable que también aumente el valor total de operaciones. Esto sugiere un creciente interés y participación en el mercado para estas criptomonedas.  

Conclusión
Basándonos en los hallazgos, recomendamos a los clientes considerar la inversión en bitcoin como una opción principal debido a su posición en el mercado y su tendencia alcista en cuanto a su valoración.
Así mismo, ethereum se presenta como una segunda opción debido a su importancia en el mundo de las criptomonedas y su capacidad para crecer en el futuro.
Aunque nuestro análisis brinda una base sólida para esta recomendación, es vital tener en cuenta que toda inversión implica riesgos, por lo que es esencial que los inversores realicen su propio análisis antes de tomar una decisión. 

El analisis lo encuentran en el archivo EDA. 

