## DBSQL_LANGCHAIN

This repo contains starter examples for working with Langchain and LLM Instruction models (e.g. MPT, from MosaicML) to query Databricks SQL.

### Getting started

* Create a Databricks single node cluster with a GPU (e.g. `Standard_NC8as_T4_v3` on Azure or `g4dn.8xlarge` on AWS). Select runtime version 13.0 ML with GPU support (minimum).

* The `config` folder contains an init script (`config.sh`). Configure the cluster to use this init script.

* Install the following packages into the cluster:

    * accelerate
    * databricks-sql-connector
    * flash-attn
    * langchain
    * ninja
    * transformers==4.29.2
    * triton

You should be good to go.