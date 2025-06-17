# 🐝 Bee Haven - Azure Data Engineering Case Study

## Overview

**Bee Haven** is a cloud-based data engineering project built around real-world challenges in environmental monitoring and sustainability. Originating from a collective of beekeepers, the project addresses bee population decline through robust data collection, integration, and analysis. Revived through a partnership with the University of Honighausen, this project leverages Microsoft Azure to build a scalable data lakehouse.

This repository documents the end-to-end implementation of a data pipeline that integrates historical and new data on hive behavior, processes it via Azure Data Factory and Synapse Analytics, and delivers insights through a Medallion Lakehouse architecture (Bronze → Silver → Gold).

> 📘 This case study supports hands-on learning for the **Microsoft DP-900 Azure Data Fundamentals** exam.

---

## 🧱 Architecture

The pipeline follows a classic Medallion Lakehouse structure:

- **Bronze**: Raw CSV uploads from hive sensors and external APIs
- **Silver**: Cleaned, structured Parquet files for efficient analytics
- **Gold**: Aggregated tables for reporting and insight generation

### Tools & Services Used:
- **Azure Data Lake Storage Gen2**
- **Azure Data Factory (ADF)**: Orchestration & pipeline automation
- **Azure Synapse Notebooks**: Data cleaning and transformation (Python-based)
- **BrightSky Weather API**: External weather enrichment
- **Parquet Format**: Efficient storage for analytical workloads
- **Role-Based Access Control (RBAC)**: Secure and granular access control

---

## ✨ Key Features

- ✅ ETL Pipeline (Extract → Transform → Load) via ADF
- ✅ Medallion architecture with Bronze, Silver, and Gold zones
- ✅ Automated file ingestion, transformation, and archival
- ✅ JSON API data integration and semi-structured processing
- ✅ Dynamic file handling with parameters, `Get Metadata`, and `ForEach` logic
- ✅ Daily scheduled pipeline + chaining of downstream processes
- ✅ Weather data enrichment using BrightSky (no API key required)

---

## 🔍 Learning Objectives

This project is ideal for:
- Practicing **cloud-native ETL design**
- Understanding Azure storage and pipeline components
- Learning **parameterisation and automation** in ADF
- Gaining hands-on experience with **Synapse Notebooks** and **JSON parsing**
- Understanding **RBAC & IAM** for secure data environments

> 🎯 Focused on preparing learners for key DP-900 exam topics like data storage, processing, analytics, and security in Azure.

---

## 📁 Project Structure

