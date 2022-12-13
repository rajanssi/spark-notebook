# Apache Spark + Jupyter Notebook

Apache Spark and Jupyter Notebooks on Openshift. Runs newest version of `jupyter/all-spark-notebook` on Rahti. 

## Running through the Command line:

*  Download oc client for openshift
* `oc login`
* `oc new-project`
* `oc process -f pyspark-template.yml | oc apply -f -`

## Using the tempate with Rahti2

After succesfull deployment, you can open Jupyter Notebook frontend web page at 

`http://www.pyspark-route-<your-project-name>.2.rahtiapp.fi`.


## Other

### [General instructions for using Rahti](https://docs.csc.fi/cloud/rahti/rahti-what-is/)

### [Jupyter Docker stascks user guide](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
