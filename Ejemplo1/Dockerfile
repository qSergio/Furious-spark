# 

FROM jupyter/pyspark-notebook:d4cbf2f80a2a

ENV HOME="/home/jovyan"

RUN pip install pyspark-stubs

#Jupyter Lab
ENV SPARK_JUPYTER_ENABLE_LABHOME yes

# Disable Notebook App Token
ENV JUPYTER_TOKEN "probandospark"

# Ensures spark-submit CLI works
ENV PATH $PATH:$SPARK_HOME/bin

## Exposing necessary ports
# Jupyter Lab
EXPOSE 8888/tcp
# SparkUI ports
EXPOSE 4040/tcp
#EXPOSE 4041/tcp
#EXPOSE 4042/tcp
#EXPOSE 4043/tcp
#EXPOSE 4044/tcp
#EXPOSE 4045/tcp
