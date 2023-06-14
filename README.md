# kubeflow_pipeline
Kubeflow Pipeline from Scratch

In this example we are going to create a Kubeflow pipeline that we can upload to our Kubeflow pipelines installation

Contents:
- kf-pipeline-juan: Jupyter Notebook with all the steps to create and compile a Kubeflow pipeline
- IRIS_Classifier_pipeline: YAML file with the compiled pipeline. This is the result of running the notebook and can be uploaded to Kubeflow.
- iris.csv

## Kubeflow Installation Instructions
In order to install Kubeflow pipelines in local you can use Docker and Minikube.

1. Install Docker
2. Install Minikube (instructions here: https://minikube.sigs.k8s.io/docs/start/)
3. Check that all pods are running (kubectl get pod -A)
4. Deploy Kubeflow to this cluster (instructions here: https://www.kubeflow.org/docs/components/pipelines/v1/installation/localcluster-deployment/)
5. Check that all pods are running
6. Forward ports (kubectl port-forward -n kubeflow svc/ml-pipeline-ui 8080:80)
7. Open Kubeflow ui (http:localhost:8080)
