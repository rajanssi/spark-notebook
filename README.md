# Apache Spark + Jupyter Notebook

Apache Spark and Jupyter Notebooks on Openshift. Runs newest version of `jupyter/all-spark-notebook` on Rahti. 

## Running through the Command line:

*  Download oc client for openshift
* `oc login`
* `oc new-project`
* `oc process -f pyspark-template.yml | oc apply -f -`

## Using the tempate with Rahti2

After succesfull deployment, you can open Jupyter server frontend web page at 

`http://www.pyspark-route-<your-project-name>.2.rahtiapp.fi`.

To get the access token to Jupyter server, you can first use the command `oc get pods` to find the right pod name and then type `oc logs -f <pod-name>`. You'll find the access token at the bottom, below the "Or copy and paste one of these URLs:" log message. Copy only the contents after the "token=" part and paste it to you Jupter server login field, or set up easy to remember password for yourself. After that, you are ready to use Jupyter Lab interface with Spark engine. 

## Other

### [General instructions for using Rahti](https://docs.csc.fi/cloud/rahti/rahti-what-is/)

### [Jupyter Docker stascks user guide](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
