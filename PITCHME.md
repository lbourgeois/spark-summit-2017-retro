### Spark Summit Europe
https://spark-summit.org/eu-2017/schedule/
https://databricks.com/sparksummit/sessions
---
#### Apache Spark 2.2 & further
* Spark approach : high level api & unified engine
* Extended to streaming & deep learning
* Structured Spark Streaming 
* Targeting continuous processing without microbatch for Spark 2.3
---
* Deep learning 
  * image support in MLLib for 2.3
  * https://github.com/yahoo/TensorFlowOnSpark
  * Deep Learning pipelines on ML pipelines model
---
#### Structured streaming
* high level API on top of Spark SQL engine
* Spark SQL optimizer
* Event time aggregation
  * windowing
  * UDF
  * watermarking
* 4x faster than Flink
---
#### Storage systems
* HDFS/HBase/Kudu/Solr
* Key questions
  * SQL/API
  * RT needed
  * Ingestion rate
  * Append/Update
* Streaming typed => Kudu
* Batched / Agg => HDFS
* Streming entity profiled => HBase
* Streaming with keyword search => Solr
---
#### RDD DataFrames/Dataset
* RDD
  * Control / Flexibility 
  * Low level / No schema
  * Describe how to do 
* DataFrame / Dataset
  * High level structured APIs with schema
  * Easy /readable
  * Descrive what to do : can be optimized
---
#### Spark memory model
* Key points
  * RDD stored in binary format
  * Optimisation on sort and hashmap algorithms
---
#### Spark perf troubleshooting
* marketing benchmarks are antipattern
* TPC-DS benchmark
* out of the box tooling : WebUI RestAPI Eventlog
* https://github.com/LucaCanali/sparkMeasure : collect & analyse Spark metrics using Spark Listeners
---
#### Dr Elephant
* Dev productivity vs Cluster efficiency
* Audit jobs on cluster
* Recommandations
* https://github.com/linkedin/dr-elephant
---
#### Spark Testing
* https://github.com/holdenk/spark-testing-base
---
#### Spark SQL optimisation (?)
* partitions number auto
* broadcast join
---
#### Lessons learned from the field (?)
* Good choices :
  * tables
  * Dataframe or Dataset API
  * columnar / parquet
  * splittable
---
#### Auto test Spark workflow (?)
* Azkaban
---
