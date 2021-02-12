
# Apache Nifi Rule processor (adapter)


## Overview
- Drools/JBoss Rules is a Business Rules Management System (BRMS) solution. It provides a rich Business Rules Engine (BRE) using RETE algorithm, a web interface based authoring and rules management application (Drools Workbench) and an Intellij/Eclipse IDE plugin for core development.

- Apache NiFi (abbreviation NiagaraFiles) is a software project from the Apache Software Foundation designed to automate the flow of data between software systems. 

- Rule engine based Rule (IF THEN) provides abstraction of hardcoding rules inside the application, hence very powerful.

## How to install:
1. `mvn clean install package -DskipTests`
2. copy nar file from `/nifi-ruleengien-processor/nifi-ruleengien-processor-nar/target/nifi-ruleengien-processor-nar-{VERSION}.nar` to your NiFi folder `/nifi-{version}/lib`
3. (Re) start your NiFi
4. Add processor search for `RuleEngineProcessor`
5. Connect Json files and magic happens

