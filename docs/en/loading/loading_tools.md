---
displayed_sidebar: docs
---

# Load data using tools

StarRocks and its ecosystem partners offer the following tools to help you seamlessly integrate StarRocks with external databases.

## [SMT](../integrations/loading_tools/SMT.md)

SMT (StarRocks Migration Tool) is a data migration tool provided by StarRocks, designed to optimize complex data loading pipelines: source databases (such as MySQL, Oracle, PostgreSQL) ---> Flink ---> destination StarRocks clusters. Its main functions are as follows:

- Simplifies table creation in StarRocks: Generates statements to create tables in StarRocks based on information from external databases and the target StarRocks cluster.
- Simplifies the full or incremental data synchronization process in the data pipeline: Generates SQL statements that can be run in Flink's SQL client to submit Flink jobs for synchronizing data.

The following flowchart illustrates the process of loading data from the source database MySQL through Flink into StarRocks.

![img](../_assets/load_tools.png)

## [DataX](../integrations/loading_tools/DataX-starrocks-writer.md)

DataX is a tool for offline data synchronization, and is open-sourced by Alibaba. DataX can synchronize data between various heterogeneous data sources, including relational databases (MySQL, Oracle, etc.), HDFS, and Hive. DataX provides the StarRocks Writer plugin to synchronize data from data sources supported by DataX to StarRocks.

## [CloudCanal](../integrations/loading_tools/CloudCanal.md)

CloudCanal Community Edition is a free data migration and synchronization platform published by [ClouGence Co., Ltd](https://www.cloudcanalx.com/) that integrates Schema Migration, Full Data Migration, verification, Correction, and real-time Incremental Synchronization.  You can directly add StarRocks as a data source in CloudCanal's visual interface and create tasks to automatically migrate or synchronize data from source databases (e.g., MySQL, Oracle, PostgreSQL) to StarRocks.

## [Kettle connector](https://github.com/StarRocks/starrocks-connector-for-kettle)

Kettle is an ETL (Extract, Transform, Load) tool with a visual graphical interface,  which allows users to build data processing workflows by dragging components and configuring parameters. This intuitive method greatly simplifies the process of data processing and loading, enabling users to handle data more conveniently. Additionally, Kettle provides a rich library of components, allowing users to select suitable components according to their needs and perform various complex data processing tasks.

StarRocks offers the Kettle Connector to integrate with Kettle. By combining Kettle's robust data processing and transformation capabilities with StarRocks's high-performance data storage and analytical abilities, more flexible and efficient data processing workflows can be achieved.
