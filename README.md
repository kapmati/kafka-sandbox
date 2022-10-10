# kafka-sandbox

Simple project with different Kafka components. It is build as multi module project only for learning purposes.

This project will be divided into a few phases of development, so it will evolve over time. Below, I describe how this evolution will look like.

## Phase 1 (basic setup)
In the first phase a basic setup of working environment will be provided. Components:  
1. Data-generator - responsible for generating random data, e.g. colors and push them to Kafka with JSON format.
2. Kafka broker
3. Data-collector - responsible for polling data from Kafka in JSON format, storing them in Postgresql and expose them as micrometer metrics.

<plant_uml_will_be_added_later>

## Phase 2 (simple schema registry)
In this phase, JSON format will be changed to Avro format and a Schema Registry component will be added. Avro schemas will be stored in data-generator module.

<plant_uml_will_be_added_later>

## Phase 3 (Kafka Streams)
Simple Kafka Stream will be added. It will be responsible for counting occurrences of each color. Data-collector will be fetching those data.

<plant_uml_will_be_added_later>

## Phase 4 (Kafka Connect)
A new module will be added - Kafka Connect for Postgresql. Data from basic color topic will be fetched by Kafka Connect to the Postgresql database.

<plant_uml_will_be_added_later>

## Phase 5 (GitHub Actions + extended schema registry)
TO BE DONE
