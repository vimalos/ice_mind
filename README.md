# ice_mind
Autonomous Data Lakehouse Maintenance Agent using LLMs and RAG

Lakehouse Sentinel is an AI-powered agent designed to monitor, diagnose, and maintain Spark + Iceberg data pipelines. It combines Agentic AI, LLMs, and Retrieval-Augmented Generation (RAG) to provide intelligent recommendations, generate maintenance commands, and assist data engineers in managing complex lakehouse environments.

🚀 Features
	•	Metadata Ingestion
	•	Automatically fetches Hive Metastore (HMS) metadata
	•	Loads Iceberg table metadata and snapshots
	•	Stores metadata as JSON locally for analysis
	•	Automated Analysis & Diagnostics
	•	Detects complex partitions
	•	Identifies stale snapshots and orphan files
	•	Detects schema drift across tables
	•	Finds small files and recommends compaction
	•	RAG-powered AI Agent
	•	Builds vector store from HMS metadata, Iceberg metadata, and internal documentation
	•	Answers natural language questions about your lakehouse
	•	Generates Spark SQL / Iceberg commands and actionable insights
	•	Optional API Interface
	•	FastAPI server for querying the agent via REST API

  🛠 Tech Stack
  Layer                Technology
  Agent / LLM          Python, LangChain, OpenAI API / local LLaMA
  RAG / Vector Store   FAISS, LlamaIndex
  Data Lake            Spark 3.5.6, Iceberg 1.6.1, Hive Metastore
  Storage              Local FS / S3 / MinIO
  API / Serving        FastAPI
  Utilities            PySpark, Pandas, JSON
