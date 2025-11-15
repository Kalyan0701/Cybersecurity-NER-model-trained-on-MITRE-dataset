# Cybersecurity-NER-model-trained-on-MITRE-dataset

Fine-tuned transformer model for detecting cybersecurity entities in text, trained on the MITRE ATT&CK dataset.

## Model Details

- **Model**: microsoft/deberta-v3-small
- **Task**: Token Classification (Named Entity Recognition)
- **Domain**: Cybersecurity
- **Input**: Security reports, threat intelligence, malware analysis
- **Output**: Labeled cybersecurity entities

## Entity Labels

The model recognizes the following cybersecurity entities:

- `B-MALWARE`, `I-MALWARE` - Malicious software (viruses, ransomware, trojans)
- `B-TOOL`, `I-TOOL` - Security tools and utilities
- `B-CVE` - Common Vulnerabilities and Exposures identifiers
- `B-C2` - Command and Control servers
- `B-THREAT_ACTOR` - Threat actor groups and APTs
- `B-TECHNIQUE` - Attack techniques and procedures
- `B-SOFTWARE` - Software applications and systems
- `O` - Other (non-entity text)

## Installation

```bash
git clone https://github.com/yourusername/cybersecurity-ner-mitre.git
cd cybersecurity-ner-mitre
pip install -r requirements.txt
```
### The model is only trained until 1 epoch and the traning epoch could be increased to properly evaluate the model and the metrices.
