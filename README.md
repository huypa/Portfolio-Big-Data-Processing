🚀 Real-Time Fraud Detection & eCommerce Analytics (Assignment 2B – FIT5202)
This project demonstrates the integration of Apache Kafka, PySpark Structured Streaming, and Machine Learning to detect fraudulent eCommerce transactions and visualise customer behaviour in real time. It was developed as part of *FIT5202: Data Processing for Big Data* at Monash University. [View project details](https://drive.google.com/drive/u/1/folders/1YpGqiuJll28ZlYhHasONw-o4b4QAI_s9)

🎯 Objectives
- Simulate real-time data streaming of browsing behaviour and transactions.

- Ingest and process data streams with Spark Structured Streaming.

- Apply a trained ML fraud detection model (from Assignment 2A) for real-time predictions.

- Generate actionable visualisations for fraud monitoring and inventory planning.

🔑 Key Contributions
1️⃣ Data Streaming with Kafka

- Implemented Kafka producers to simulate real-time streams of browsing and transaction data.

- Sent batches of 500–1000 records every 5 seconds with Unix timestamp alignment.

- Ensured memory efficiency by sequential row reads instead of full dataset loading.

2️⃣ Real-Time Processing with Spark Structured Streaming

- Built a SparkSession with checkpointing and Melbourne timezone support.

- Defined schemas from metadata and joined static datasets (customers, products, categories) with streaming data.

- Engineered features consistent with the ML pipeline from Part A.

- Applied fraud detection model to classify transactions and persist results in Parquet format.

Aggregated insights, e.g.:

- Fraud predictions every 10 seconds.

- Top 20 products in shopping carts (non-fraud) every 30 seconds.

3️⃣ Real-Time Visualisation

- Developed Kafka consumers to read processed data streams.

Built live plots to monitor:

- Fraudulent transactions over time (bar charts).

- Cumulative non-fraud product sales (line chart).

Designed an advanced plot (bubble/choropleth map) to highlight fraud hotspots by location.

🛠️ Tools & Technologies

- Kafka (stream simulation & message brokering)

- PySpark Structured Streaming & MLLib (real-time processing & ML inference)

- Pandas, Matplotlib (data visualisation)

- Parquet (efficient storage & re-streaming)

✅ Outcome

Delivered a prototype real-time fraud detection pipeline achieving accurate fraud predictions and actionable business insights for inventory management. Strengthened expertise in streaming architectures, big data pipelines, and applied machine learning in production-like environments.
