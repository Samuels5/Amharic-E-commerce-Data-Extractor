# Amharic-E-commerce-Data-Extractor

## Project Overview

A pipeline for extracting, labeling, and analyzing Amharic e-commerce data from Telegram channels, with NER model training, interpretability, and vendor analytics.

## Completed Tasks

1. **Environment Setup & Library Installation**

   - Installed all required Python libraries for NLP, ML, and interpretability.

2. **Data Ingestion & Preprocessing**

   - Loaded Telegram data from Excel files.
   - Cleaned and normalized Amharic text.
   - Extracted potential entities (products, prices, locations) using regex.

3. **NER Labeling**

   - Sampled messages for manual labeling.
   - Provided CoNLL labeling template and exported for annotation.
   - Converted labeled CSVs to CoNLL format.

4. **Model Fine-tuning**

   - Loaded labeled data from CoNLL format.
   - Created label mappings and tokenized data for Hugging Face models.
   - Split data into train/validation sets.
   - Trained transformer-based NER models (XLM-Roberta, mBERT).
   - Evaluated and saved both models.
   - Added inference code for new Amharic text.

5. **Model Comparison & Evaluation**

   - Compared XLM-Roberta and mBERT on F1, precision, recall, accuracy, model size, and inference speed.
   - Displayed entity-level metrics and recommendations.

6. **Model Interpretability**

   - Added LIME analysis for NER interpretability.
   - Added attention visualization for token-level interpretability.

7. **Vendor Analytics & Scorecards**
   - Extracted NER entities for all messages.
   - Aggregated by vendor/channel and computed business metrics.
   - Visualized top vendors by product diversity, price range, and location coverage.

## Next Steps

- Export scorecard results for business use.
- Integrate with FinTech decision engines.
- Continue improving NER and analytics with more data and feedback.

---

For details, see the main notebook: `Amharic_Ecommerce_Data_Extractor.ipynb`.
