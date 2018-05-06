# Traffic-sign-recognition
Deep neural networks applied to traffic sign recognition on the Belgium dataset  

+ WALEED ABDULLA
Empiezo siguiendo los pasos del artículo de W.A. y de su conferencia.    
https://medium.com/@waleedka/traffic-sign-recognition-with-tensorflow-629dffc391a6    
https://www.youtube.com/watch?v=QHra6Xf6Mew&t=2268s    
Construye varios modelos para llegar hasta una deep net con la siguiente estructura:    
IMAGES - CONV1 - POOL1 - CONV2 - POOL2 - CONV3 - POOL3 - FC1  
Con esto conseguimos una TRAIN ACCURACY=100% y una TEST ACCURACY=94,5%    
Parece un claro caso de "over fitting"   

+ CLASSICAL NEURAL NETS
Vamos a probar de aplicar las redes nuronales más conocidas y clásicas a nuestro caso  
  - LeNet-5  
    Aplicando este modelo obtenemos un 100% de precisión en el TRAIN set y un 93% en el TEST set.   
    Vemos que llegamos al 100% igual que en el artículo de W.A. pero en este caso la precisión en el TEST set es mucho menor.  
    
    

De momento llevo 2 CNN que me han dado resultados parecidos y estas son las conclusiones a las que he llegado:  
+ ¿Puede que el model4 de W.A. esté mal?  
    Por un lado veo que las dimensiones de los INPUTS y OUTPUTS que ha anotado en su código están mal. (O ESO CREO YO)  
    
