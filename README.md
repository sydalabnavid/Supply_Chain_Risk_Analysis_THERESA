# Supply_Chain_Risk_Analysis_THERESA

The results, dataset, and notebook are shared on the GitHub
The Rule-Based Regex Extraction is working very well but AI method is not accurateand I need help with it


Comparing Different Methods for Risk Score Analysis
Risk Score Analysis can be performed using different approaches based on the type of data available. The objective is to assess the supply chain risk of various products (SKUs) by analyzing Lead Times and Stock Levels. Below, we explain three different methods used for this analysis.

1-- Tabular Data and Conventional Method for Risk Score Analysis
This method is based on structured tabular data, where all relevant information (such as SKU, Lead times, and Stock levels) is already available in a well-organized table format.

The Risk Score formula used:
Risk Score=Lead times×(1−Stock levels)

Key Features of This Approach:
Directly uses numerical values from structured datasets (e.g., CSV or Excel files).
No need for text processing or entity extraction.
Fast and highly accurate for structured datasets.
Comparison Name:
The results from this approach are called "Tabular Data Analysis Results", and they serve as a benchmark for comparing text-based analysis results.


2-- Text-Based Analysis Using Rule-Based Regex Extraction
In this method, textual descriptions of products are analyzed using regular expressions (regex) to extract structured data.

How It Works:
The system scans text documents to identify patterns related to Lead times, Stock levels, and SKUs.
Extracted values are then used to calculate the Risk Score using the same formula.
Key Features:
Works well for structured text formats that follow a predictable pattern.
Faster than AI-based methods but less flexible when dealing with complex text.
Requires predefined regex rules, which may not work well for varying sentence structures.
Comparison Name:
This approach is called "Text Analysis Using Rule-Based Regex", and it helps evaluate how well text-based extraction compares with tabular data results.


3-- Text-Based Analysis Using BERT-Based Named Entity Recognition (NER)
This method leverages Artificial Intelligence (AI) and Natural Language Processing (NLP) to extract key information from text.

How It Works:
Uses BERT-based NER models to recognize product attributes like Lead times, Stock levels, and SKUs.
AI is supposed to identify and extract relevant numeric values even if the sentence structure varies.
Extracted values are then processed using the Risk Score formula.
Key advantages:
Supposed to be more accurate than regex for handling complex text.
Can extract data from unstructured or inconsistent text formats.

Weakness
Requires pre-trained AI models, making it computationally intensive.


