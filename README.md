
# Apache Nifi Rule processor (adapter)


## Overview
- Drools/JBoss Rules is a Business Rules Management System (BRMS) solution. It provides a rich Business Rules Engine (BRE) using RETE algorithm, a web interface based authoring and rules management application (Drools Workbench) and an Intellij/Eclipse IDE plugin for core development.

- Apache NiFi (abbreviation NiagaraFiles) is a software project from the Apache Software Foundation designed to automate the flow of data between software systems. 

- Rule engine based Rule (IF THEN) provides abstraction of hardcoding rules inside the application, hence very powerful.

## Packaging install NAR to Apache Nifi installation 
Step 1. `mvn clean install package -DskipTests`
Step 2. copy nar file from `/nifi-rules-processor/nifi-ruleengien-processor-nar/target/nifi-rules-processor-nar-{VERSION}.nar` to NiFi folder `/nifi-{version}/lib`
Step 3. (Re) start NiFi
Step 4. Add processor search for `RuleEngineProcessor`
Step 5. Connect Json files and magic happens

