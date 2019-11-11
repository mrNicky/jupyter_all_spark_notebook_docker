# jupyter_all_spark_notebook_docker
Run Jupyter Notebook Python, Scala, R, Spark, Pyspark

### Pull docker image 
```docker pull jupyter/all-spark-notebook```

### Run container with volume

Créate a directory which is used to save your notebooks. 

```mkdir work```

In the following command, replace /path_to_your_volume_folder 

```docker run --rm -p 8888:8888 -v /path_to_your_volume_folder:/home/jovyan/work jupyter/all-spark-notebook```

### Copy from shell the output of previous command docker run 

http://127.0.0.1:8888/?token=4ef80ae6f0f6d901e....590d0420f11a4127c9

### Careful

When you run the jupyter notebook, save your notebooks inside work folder not outside if not you will lose all your works 
