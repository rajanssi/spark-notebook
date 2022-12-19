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

To get the access token to Jupyter server, go to your Jupyter server web page. The default token will be set to `12345`. You can change with the Setup Password field during your first log in.

## Other

### [General instructions for using Rahti](https://docs.csc.fi/cloud/rahti/rahti-what-is/)

### [Jupyter Docker stascks user guide](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
