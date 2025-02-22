<!--

    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.

-->

# Apache Pulsar Adapters

This repository is used for hosting all the adapters maintained and supported by Apache Pulsar PMC.

[Apache Flink adapter](https://github.com/apache/flink/tree/master/flink-connectors/flink-connector-pulsar) is supported and maintained by Apache Flink Community.

## Building

In order to build this code you can simply use Maven

mvn install

In order to build this repository the linked Pulsar release must be released to Maven Central
other wise you have to build it locally.

For instance if this code depends on Pulsar 2.11.0 you have to build Pulsar 2.11.0 locally

```
git clone https://github.com/apache/pulsar
git checkout v2.11.0
mvn clean install -DskipTests
```

This is because this repository depends on test integration artifacts of the relative version on the main 
Apache Pulsar codebase
