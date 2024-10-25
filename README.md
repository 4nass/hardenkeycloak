# HardenKeycloak

HardenKeycloak is an AI-powered tool designed to enhance the security of Keycloak IAM (Identity and Access Management) configurations. By analyzing configurations, documentation, and extracting potential vulnerabilities, HardenKeycloak helps ensure best practices are followed, identifies misconfigurations, and suggests pentesting methods specific to Keycloak environments.

### Features

- Configuration Analysis: Analyzes Keycloak configurations to identify potential security risks and improvements.
- Misconfiguration Detection: Leverages machine learning to detect common misconfigurations in Keycloak setups.
- Vulnerability Extraction: Uses NLP to extract and highlight potential vulnerabilities from Keycloak documentation and CVEs.
- Log Analysis (Upcoming): Identifies abnormal patterns in Keycloak logs for enhanced threat detection.
- Payload Generation (Future Development): Suggests test payloads for identified vulnerabilities.

### Installation

#### Requirements

Python 3.8+
PyTorch
Hugging Face Transformers
Additional dependencies listed in requirements.txt

#### Setup

- Clone the repository:

```bash
git clone https://github.com/4nass/HardenKeycloak.git
cd HardenKeycloak
```
- Install the dependencies:

```bash
pip install -r requirements.txt
```
### Usage

#### Basic Configuration Analysis

To run a basic analysis on Keycloak configurations:

```bash
python src/config_analysis/analyze.py --config <path_to_config_file>
```
#### Misconfiguration Detection

Detect potential misconfigurations in a Keycloak setup:

```bash
python src/misconfig_detection/detect.py --config <path_to_config_file>
```
#### Vulnerability Extraction

To analyze documentation or release notes for known vulnerabilities:

```bash
python src/vulnerability_extraction/extract.py --docs <path_to_documentation_file>
```

### Project Structure

```bash
HardenKeycloak/
├── data/                        # Sample configurations and labeled data
├── docs/                        # Documentation for setup and usage
├── src/                         # Core source code for modules
│   ├── config_analysis/         # Configuration analysis module
│   ├── misconfig_detection/     # Misconfiguration detection module
│   ├── vulnerability_extraction/ # Vulnerability extraction module
│   └── utils/                   # Utility scripts and helper functions
├── notebooks/                   # Jupyter notebooks for experiments
├── tests/                       # Unit tests for modules
├── models/                      # Saved/pretrained models
├── scripts/                     # Standalone scripts (e.g., data preprocessing)
├── requirements.txt             # List of dependencies
└── README.md                    # Project overview and instructions
```

### License
This project is licensed under the MIT License. See the LICENSE file for details.
