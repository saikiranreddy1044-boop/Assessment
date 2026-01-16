# HEALTHCARE ELIGIBILITY INGESTION PIPELINE

## PROJECT SUMMARY
This pipeline ingests healthcare eligibility files from multiple external partners using a configuration-driven approach.
Incoming data is normalized into a single standardized schema to support downstream analytics and processing.

---

## CORE CAPABILITIES
- Fully configuration-driven ingestion
- Multi-format and multi-delimiter support
- Schema standardization
- Validation and error handling
- CSV and Excel output support

---

## INGESTED PARTNERS
- **Acme Health** — Pipe-delimited text files
- **Better Care** — Comma-delimited CSV files

---

## STANDARDIZED DATA MODEL
- **external_id** : Unique member identifier
- **first_name**  : Proper case formatting
- **last_name**   : Proper case formatting
- **dob**         : ISO-8601 date (YYYY-MM-DD)
- **email**       : Lowercase
- **phone**       : Standardized phone number
- **partner_code**: Partner identifier

---

## EXECUTION INSTRUCTIONS (COLAB)
1. Launch the notebook in Google Colab
2. Upload partner input files
3. Execute all notebook cells

### Artifacts Produced
- `final_eligibility_output.csv`
- `final_eligibility_output.xlsx`

---

## PARTNER ONBOARDING PROCESS
1. Add partner details to the configuration object
2. Define delimiter, schema mapping, and partner code
3. Core processing logic remains unchanged

---

## DATA QUALITY CONTROLS
- Required field enforcement
- Invalid data handling
- Rejection of malformed records
- Processing metrics per partner

---

## TECHNOLOGY STACK
Python, Pandas, Google Colab
