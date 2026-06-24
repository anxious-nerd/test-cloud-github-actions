# Intelligent Antivirus: HPC and MLOps Pipeline - SECCIÓN PRUEBAS N_JOBS

Este repositorio es un clon y modificación del repo https://github.com/fabrizziomcl/hp3c-cibersecml

Se clonó la rama test-(métricas) y se relizaron las modificaciones pertinentes:

Se modificó el workflow de github actions para que el trigger sea la modificación del archivo src/config/config.py
En este caso se realizó un commit por cada n_jobs evaluado (1-14)

La acción realizada después del reentrenamiento será el push del reports/, json de las métricas (ya no model ni preprocessor)

Se elimninó el test que verifica que n_jobs=-1 para correr el modelo (ya que se tenía que probar con los diferentes n_jobs)

Se eliminó la data de raw para que el experimento sea el mismo cada vez

En src/config/config.py se determinan los parámetros de la corrida, abajo se cambia el n_jobs








