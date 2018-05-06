# Traffic-sign-recognition
Deep neural networks applied to traffic sign recognition on the Belgium dataset  

+ BARNCH WALEED ABDULLA  
Empiezo siguiendo los pasos del artículo de W.A. y de su conferencia.    
https://medium.com/@waleedka/traffic-sign-recognition-with-tensorflow-629dffc391a6    
https://www.youtube.com/watch?v=QHra6Xf6Mew&t=2268s    
Construye varios modelos para llegar hasta una deep net con la siguiente estructura:    
IMAGES - CONV1 - POOL1 - CONV2 - POOL2 - CONV3 - POOL3 - FC1  
Con esto conseguimos una TRAIN ACCURACY=100% y una TEST ACCURACY=94,5%    
Parece un claro caso de "over fitting"   

+ BRANCH CLASSICAL NEURAL NETS  
Vamos a probar a aplicar las redes nuronales más conocidas y clásicas a nuestro caso  
  - LeNet-5  
    Aplicando este modelo obtenemos un 100% de precisión en el TRAIN set y un 93% en el TEST set.   
    Vemos que llegamos al 100% igual que en el artículo de W.A. pero en este caso la precisión en el TEST set es mucho menor.  
    
    

De momento llevo 2 CNN que me han dado resultados parecidos y estas son las conclusiones a las que he llegado:  



+ ¿Puede que el model4 de W.A. esté mal?  
    Por un lado veo que las dimensiones de los INPUTS y OUTPUTS que ha anotado en su código están mal. (O ESO CREO YO)  
    La segunda parte del artículo no está publicada y la he conseguido de una conferencia en youtube.  
    El hecho de que no esté publicada me da mala espina, ¿Si ya tiene el código escrito porque no publica el artículo?  
    Todo esto me induce a pensar que el código pueda estar mal, y que haya un error. 
    Como él mismo dice en deep learning es muy difícil saber si hay un error porque el modelo te da resultados pero no tienes forma fácil de saber si eso es correcto.  
    
+ VARIANCE o OVERFITTING --> REGULARIZACIÓN  
  Si tengo que seguir con esta línea lo primero que hay que hacer es intentar corregir el problema del overfitting.    
  Para ello hay muchas técnicas: dropout, early stopping, data augmentation  
  
  
+ OTHER APPROACHES  
  Existen muchos papers incluso una competición con el Belgium dataset. Podría probar a aplicar alguno de sus modelos.  
    - The German Traffic Sign Recognition Benchmark: A multi-class classification competition  
      https://www.researchgate.net/publication/224260296_The_German_Traffic_Sign_Recognition_Benchmark_A_multi-class_classification_competition
     - A committee of neural networks for traffic sign classification  
      https://www.researchgate.net/publication/241191907_A_committee_of_neural_networks_for_traffic_sign_classification
     - Multi-column deep neural network for traffic sign classification  
      https://www.sciencedirect.com/science/article/pii/S0893608012000524
     - Traffic sign recognition with convolutional neural network based on max pooling positions  
      https://cgi.csc.liv.ac.uk/~frans/PostScriptFiles/icnc-fskd_2016_MaxPooling.pdf
  
+ GERMAN DATASET  
  Hay un segundo dataset que aún no he tocado, el german dataset.  
  Tengo un artículo parecido al de W.A : https://navoshta.com/traffic-signs-classification/ y también un repositorio en github.
  Puede ser una buena solución para el data augmentation que necesito para corregir la variance del belgium dataset
