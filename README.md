# HEART-DISEASE-PREDICTION-HDFS-
Certainly! Here's an enhanced `README.md` with the requested usernames and some added emoji to make it more engaging:

```markdown
# 🚀 HDFS Project

## Overview

This project involves working with the **Hadoop Distributed File System (HDFS)**, a core component of the Apache Hadoop ecosystem. HDFS is designed to store large datasets across multiple machines in a distributed environment, ensuring fault tolerance and scalability.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Data Processing](#data-processing)
- [Results](#results)
- [Contributors](#contributors)
- [License](#license)

## Installation 🛠️

### Prerequisites

Before setting up HDFS, ensure that your environment meets the following prerequisites:

- **Java**: HDFS requires Java 8 or later.
- **SSH**: SSH should be enabled and configured on all nodes in the cluster.
- **Hadoop**: Download and install Hadoop, which includes HDFS.

### Installation Steps

1. **Download Hadoop**:
   ```bash
   wget https://downloads.apache.org/hadoop/common/hadoop-3.3.0/hadoop-3.3.0.tar.gz
   ```

2. **Extract the downloaded archive**:
   ```bash
   tar -xzvf hadoop-3.3.0.tar.gz
   ```

3. **Configure Hadoop Environment Variables**: 
   Add the following to your `.bashrc` or `.zshrc` file:
   ```bash
   export HADOOP_HOME=/path/to/hadoop
   export PATH=$PATH:$HADOOP_HOME/bin
   export HADOOP_CONF_DIR=$HADOOP_HOME/etc/hadoop
   ```

4. **Configure HDFS**:
   Edit the `core-site.xml` and `hdfs-site.xml` files located in the `HADOOP_HOME/etc/hadoop/` directory to set up the namenode and datanodes.

5. **Format the Namenode**:
   ```bash
   hdfs namenode -format
   ```

6. **Start HDFS**:
   ```bash
   start-dfs.sh
   ```

7. **Verify HDFS Setup**:
   Access the HDFS web interface at `http://localhost:9870/` to verify that the setup is correct.

## Usage 🎯

### Basic HDFS Commands

1. **Create a directory in HDFS**:
   ```bash
   hdfs dfs -mkdir /user/pravin1279/input
   ```

2. **Copy files to HDFS**:
   ```bash
   hdfs dfs -put /path/to/local/file.txt /user/pravin1279/input
   ```

3. **List files in a directory**:
   ```bash
   hdfs dfs -ls /user/pravin1279/input
   ```

4. **Read a file from HDFS**:
   ```bash
   hdfs dfs -cat /user/pravin1279/input/file.txt
   ```

5. **Delete a file from HDFS**:
   ```bash
   hdfs dfs -rm /user/pravin1279/input/file.txt
   ```

## Data Processing 🔄

This section details how data is processed within the HDFS environment using MapReduce, Apache Spark, or other tools integrated with Hadoop.

### Example: Running a MapReduce Job

1. **Compile the MapReduce Program**:
   ```bash
   javac -classpath `hadoop classpath` -d wordcount_classes WordCount.java
   jar -cvf wordcount.jar -C wordcount_classes/ .
   ```

2. **Run the MapReduce Job**:
   ```bash
   hadoop jar wordcount.jar org.myorg.WordCount /user/pravin1279/input /user/pravin1279/output
   ```

3. **View the Output**:
   ```bash
   hdfs dfs -cat /user/pravin1279/output/part-r-00000
   ```

## Results 📊

This section should summarize the outcomes of any data analysis or processing done using HDFS.

## Contributors ✨

- **Pravin Kumar Pattnaik** - [pravin1279](https://github.com/pravin1279)
- **Sonit Kumar Swain** - [rzr-18](https://github.com/rzr-18)

## License 📜

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

y.
