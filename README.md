# argocd-demo

Se crean los archivos argocd-nginx-staging, argocd-nginx-prod, argocd-helm-python y argocd-helm-python-prod que son el manifest que permiten la creación de la aplicación por medio de kubectl apply. Estos archivos constan de una ruta que les permite acceder los archivos obligatorios para Helm.

## Uso

Se crean archivos de configuración para la creación de 3 aplicaciones que tendrán datos de configuración diferente ya que cada una utiliza su value de forma distinta. Dónde a cada una se le establecen unos valores diferentes.

Para el archivo de configuración argocd-nginx-test.yaml su archivo será values.yaml

Mientras que para argocd-nginx-staging.yaml es values-staging.yaml

Y para argocd-nginx-prod.yaml es values-prod.yaml

La carpeta template contiene todos los manifest a ejecutar para cada una de las aplicaciones, y tendrán variables que son las que hacen que se pueda acceder a cada uno de los valores establecidos en los diferentes servicios.

Esto se encuentra dentro del repositorio juanb3r/argocd-demo/helm/nginx-test
