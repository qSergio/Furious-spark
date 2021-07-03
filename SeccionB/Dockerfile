# 

FROM jupyter/pyspark-notebook

ENV HOME="/home/jovyan"

RUN pip install pyspark-stubs
# No estoy seguro de si necesita instalar dl
# RUN pip install sparkdl
RUN pip install horovod[spark]

# Jupyter Lab
ENV SPARK_JUPYTER_ENABLE_LABHOME yes

# para cambiar el token de ingreso a spark
ENV JUPYTER_TOKEN "probandospark"

# Ensures spark-submit CLI works
# Falta verificar esta afirmación
ENV PATH $PATH:$SPARK_HOME/bin

# Jupyter Lab
EXPOSE 8888/tcp
# SparkUI port para tener aplicación extra corriendo
EXPOSE 4040/tcp
