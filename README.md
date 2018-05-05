# Traffic Sign Recognition with TensorFlow with Waleed Abdulla

Vamos a intentar seguir los pasos del artículo de W.A. y programar una deep neural net.

Nos vamos a basar en su ar´ticulo de Medium y el repositoria de GitHub : https://medium.com/@waleedka/traffic-sign-recognition-with-tensorflow-629dffc391a6
También utilizaremos una de sus conferencias donde muestra un segundo articulo aún en desarrollo: https://www.youtube.com/watch?v=QHra6Xf6Mew&t=2268s


ROUND 0 --> Nos descargamos el dataset y lo exploramos viendo como está organizado el tipo de imáganes que hay y su distribución.


ROUND 1 --> Intento aplicar una deep net de una solo capa de 62 nodos con un código basado en el curso de Andrew NG.
NO CONSIGO SACAR NADA EN CLARO, HAY ALGÚN TIPO DE ERROR


ROUND 2 --> Seguimos al pie de la letra el artículo de W.A y aplicamos un primer modelo M1. Este modelo tiene una sola capa de 62 nodos igual al número de categorias del dataset. Utilizamos Adam para optimizar. Obtenemos una precisión variable entre 40 y 70 %.


EL ARTÍCULO 1 DE W.A. LLEGA HASTA AQUÍ. A PARTIR DE ESTE PUNTO HEMOS TENIDO QUE UTILIZAR EL MATERIAL DE SU CONFERENCIA


ROUND 3 --> Repetimos el M! pero esta vez lo programos en clases y analizamos los pesos de la capa. Vemos que hay algunas categorias que tienen mucho acierto y otras que muy poco. HAY CATEGORIAS MUY REPRESENTADAS Y OTRAS MUY POCO REPRESENTADAS.  
En el M2 simplemente mejoramos el M1 utilizando minibatches (para minimizar el tema de la subrepresentación) y Leaky Relu. Obtenemos una precisión del 70-75%.  
En el M3 creamos la primera deep net, con tres capas FC de 200, 100 y 62. Obtenemos una precisión del 93%.


ROUND 4 --> M4 será la primera convolutional neural net. Aplicaremos el siguient esquema con tres capas: [CONV1-POOL]-[CONV2-POOL]-[CONV3-POOL]-FC
En un primer análisis del código de W.A. parece que las dimensiones que el annota son erróneas.
