### Spark Summit Europe Retrospective
---
https://spark-summit.org/eu-2017/schedule/
https://databricks.com/sparksummit/sessions
---
#### Keynote day 1 : Apache Spark 2.2
* Spark approach : high level api & unified engine
* Extended to streaming & deep learning
* Structured Spark Streaming 
  * from batch plan to incremental plan
  * 4x faster than Flink (Spark SQL optim)
* Targeting continuous processing without microbatch for Spark 2.3
---
* Deep learning 
  * image support in MLLib for 2.3
  * https://github.com/yahoo/TensorFlowOnSpark
  * Deep Learning pipelines on ML pipelines model
---
#### Structured streaming
* high level API on top of Spark SQL
* Spark SQL optimiser / Tungsten
* Event time aggregation
  * windowing
  * UDF
  * watermarking
---
#### Spark perf troubleshooting
* marketing benchmarks are antipattern
* TPCDS benchmark
* tools WebUI RestAPI Eventlog
* https://github.com/LucaCanali/sparkMeasure
---
#### Spark memory model
* internally binary format
* improvements on sort and hashmap
---
#### Spark SQL optimisation
* partitions number auto
* broadcast join
---
#### Lessons learned from the field
* Good choices :
  * tables
  * Dataframe or Dataset API
  * columnar / parquet
  * splittable
---
#### Auto test Spark workflow
* Azkaban
---
Multitenant Spark notebooks workloads
---
#### Dr Elephant
* Dev productivity vs Cluster efficiency
* Audit jobs on cluster
* Recommandations
* https://github.com/linkedin/dr-elephant
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
Monitor Spark in the cloud
---
#### RDD DataFrames Dataset
* RDD
  * Control / Flexibility 
  * Low level / No schema
  * Describe how to do 
* DataFrame / Dataset
  * High level structured APIs with schema
  * Easy /readable
  * Descrive what to do : can be optimized
---
Testing Spark
---

