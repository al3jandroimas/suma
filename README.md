# BRUNO: A Deep Recurrent Model for Exchangeable Data
# Dataset
Los códigos fueron creados en google colab, por tanto se guardo en la siguiente carpeta: content/ y descargados de la siguiente pagina:

# MNIST
[yann.lecun.com/exdb/mnist/](http://www.yann.lecun.com/exdb/mnist/)

# Fashion MNIST
[github.com/zalandoresearch/fashion-mnist](http://wwww.github.com/zalandoresearch/fashion-mnist)

# Omniglot
[github.com/brendenlake/omniglot/tree/master/python](http://github.com/brendenlake/omniglot/tree/master/python)

Descargamos archivos .pkl de [github.com/renmengye/few-shot-ssl-public#omniglot](http://wwww.github.com/renmengye/few-shot-ssl-public#omniglot). Estos los usamos para hacer train-test-validation split.

Corremos el archivo utils.py para procesar imágenes Omniglot

# CIFAR-10
Esta base de datos sera descargado directamente de la página

# Prueba y Entrenamiento
Para las pruebas y entrenamiento primero corrimos los archivos siguientes: utils.py, utils_conditional.py, data_iter_conditiona.py, nn_extra_student.py,nn_extra_nvp_conditional.py, nn_extra_nvp.py,nn_extra_gauss.py,data_iter.py.

Ahora descargamos las siguientes bases de datos:

[drive.google.com/drive/folders/1x4EZFEE_bT9lvBu25ZnsMtV4LNKhYaG5?usp=sharing](http://www.drive.google.com/drive/folders/1x4EZFEE_bT9lvBu25ZnsMtV4LNKhYaG5?usp=sharing). para obtener los archivos 02691156.zip y 03001627.zip y fue descargado en la ruta content/ de google colab

Despúes corrimos defaults_config.py y el siguiente fue m1_shapenet.py para despues correr train.py y test_samples.py

Para entrenar lo anterior hicimos lo siguiente:

!CUDA_VISIBLE_DEVICES=0,1 python3 /content/suma/train.py y /content/suma/m1_shapenet.py

# Generación de muestras
!CUDA_VISIBLE_DEVICES=0 python3 /content/suma/test_samples.py

# Generación de muestras de la priori
!CUDA_VISIBLE_DEVICES=0 python3 /content/suma/test_samples_prior
