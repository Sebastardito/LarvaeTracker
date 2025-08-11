# 🐛 LarvaeTracker - Interactive Larvae Growth Analysis Platform

**LarvaeTracker** is a powerful web application for researchers studying larvae development. It transforms raw growth data into interactive visualizations and statistical insights, accelerating your analysis workflow.

## ✨ Key Features
| Feature | Description |
|---------|-------------|
| **📈 Interactive Visualizations** | Plot growth curves with customizable standard deviations |
| **🧪 Multi-level Statistics** | Calculate metrics by population, cycle, group, or combinations |
| **🔗 Correlation Analysis** | Compute Pearson/Spearman correlations between groups |
| **📊 Trend Detection** | Identify and classify growth trends |
| **⚖️ Comparative Analysis** | Compare max/min values across groups |
| **🧪 Statistical Testing** | Perform ANOVA and Tukey HSD post-hoc tests |
| **🔍 Cluster Analysis** | Identify similar patterns with hierarchical clustering |
| **📄 Automated Reporting** | Generate comprehensive PDF reports with visualizations |
| **🎨 Responsive Dashboard** | Modern UI with dark/light theme support |

---

## 🚀 Getting Started

### ⚙️ Installation
1. Clone the repository:
```bash
git clone https://github.com/Sebastardito/LarvaeTracker.git
cd LarvaeTracker
```

2. Create a virtual environment:
```bash
python -m venv venv
# Activate:
source venv/bin/activate    # Linux/Mac
.\venv\Scripts\activate     # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### 🖥️ Usage
```bash
python tracker.py path/to/your/data.csv
```
The application will automatically open in your browser at `http://127.0.0.1:5000`

**Workflow Guide**:
1. Select target populations, cycles, and groups
2. Choose growth metric (e.g., `Indv_Weight`)
3. Customize visualization settings
4. Explore statistical analyses through dashboard tabs
5. Generate PDF reports with one click

---

## 📂 Data Requirements
Your CSV should include these columns:
| Column | Required | Description | Example |
|--------|----------|-------------|---------|
| `Population` | ✓ | Population identifier | `PopA` |
| `Cycle` | ✓ | Growth cycle identifier | `Cycle1` |
| `Group` | ✓ | Experimental group | `Control` |
| `Age_Days` | ✓ | Age in days | `10` |
| `Data_Date` | △ | Measurement date | `2024-03-01` |
| Measurement Columns | ✓ | Growth metrics | `Indv_Weight` |

**Example CSV Structure** (default ';' separator):
```csv
Population;Cycle;Group;Age_Days;Data_Date;Indv_Weight;Other_Metric
PopA;Cycle1;Control;10;2024-03-01;0.25;15.2
PopB;Cycle2;Experimental;15;2024-03-06;0.42;18.7
```

---

## 🧠 Scientific Methods
- Descriptive statistics (mean, std dev, percentiles)
- Linear regression for trend analysis
- Pearson/Spearman correlations
- ANOVA with Tukey HSD post-hoc
- Hierarchical clustering
- Daily growth rate calculations
- Comparative analysis (% differences)
- Hypothesis testing

---

## 🧩 Project Structure
```
LarvaeTracker/
├── tracker.py            # Flask application core
├── templates/            # Dashboard UI components
│   └── index.html        
├── static/               # Assets directory (CSS/JS)
├── requirements.txt      # Dependency specifications
└── data/                 # Sample datasets (optional)
```

---

## 📜 License
Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 👨‍🔬 Author
**Sebastardito!** - SAEU 2025  
[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/Sebastardito/LarvaeTracker)
```
