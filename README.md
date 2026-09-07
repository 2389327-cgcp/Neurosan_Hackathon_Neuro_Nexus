# Neurosan_Hackathon - Neuro_Nexus

## Multi-Agent Medallion Lakehouse Governance System
A multi-agent network built with Neuro San Studio designed to automate governance, quality engineering, and storage performance tuning for Medallion Lakehouse Architecture (Bronze $\rightarrow$ Silver $\rightarrow$ Gold).

## Project Overview
This project implements an automated, collaborative AI agent ecosystem to audit raw data incoming into a Medallion Lakehouse. The network handles tasks ranging from PII protection and schema validation to generating PySpark cleansing pipelines, dbt data quality tests, and Delta Lake storage optimizations (OPTIMIZE, VACUUM, Z-Order).

## Agent Path
The primary governance network configuration is housed under:
registries/basic/data_engineer 

## Multi-Agent Architecture
# 1.Medallion_Governance_Auditor (Orchestrator)
  •Serves as the primary entry point for queries.
  •Inspects raw data streams for PII compliance, security risks, and high-level schema anomalies.
  •Delegates specific downstream engineering tasks to domain-specialist agents and compiles their outputs into a single         consolidated report.

# 2.Lakehouse_Quality_Specialist (Sub-Agent)
  •Generates memory-optimized PySpark data cleansing scripts for Bronze-to-Silver transitions.
  •Generates dbt schema.yml test configurations and Delta Live Tables (DLT) expectation decorators (@dlt.expect).

# 3.Lakehouse_Optimizer_Agent (Sub-Agent)
  •Analyzes table usage and access patterns to recommend multi-column Z-Ordering strategies.
  •Produces optimized Delta SQL maintenance routines (OPTIMIZE, VACUUM).
