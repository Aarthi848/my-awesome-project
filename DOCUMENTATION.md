# 📚 Aswini Project Documentation

## 📋 Table of Contents
1. [Project Overview](#project-overview)
2. [Repository Structure](#repository-structure)
3. [Setup & Installation](#setup--installation)
4. [Module Documentation](#module-documentation)
5. [Testing](#testing)
6. [CI/CD Pipeline](#cicd-pipeline)
7. [Usage Examples](#usage-examples)

---

## 🎯 Project Overview
**Repository:** `gaarthi848/aswini`  
**Visibility:** Public  
**Default Branch:** `main`

> *Add a brief description of what this project does, its purpose, and target audience.*

---

## 📁 Repository Structure
```
aswini/
├── README.md                          # Project documentation
├── .gitlab-ci.yml                     # CI/CD pipeline configuration
├── New_workflow/
│   ├── main.py                        # Main application entry point
│   ├── requirements.txt               # Python dependencies
│   ├── setup.py                       # Package installation script
│   ├── test_main.py                   # Tests for main module
│   ├── .gitlab-ci.yml                 # Workflow-specific CI config
│   └── README.md                      # Workflow documentation
└── new_level/
    ├── .gitlab-ci.yml                 # Level-specific CI config
    ├── requirements.txt               # Dependencies for new_level
    ├── app/
    │   ├── __init__.py                # Package initializer
    │   └── math_utils.py              # Mathematical utility functions
    └── tests/
        ├── __init__.py                # Test package initializer
        └── test_math_utils.py         # Tests for math utilities
```

---

## 🛠️ Setup & Installation

### Prerequisites
- Python 3.x
- pip

### Installation Steps
```bash
# Clone the repository
git clone https://gitlab.com/gaarthi848/aswini.git
cd aswini

# Install dependencies
pip install -r New_workflow/requirements.txt
# OR
pip install -r new_level/requirements.txt

# Install package (if applicable)
python setup.py install
```

---

## 📖 Module Documentation

### 1. New Workflow Module (`New_workflow/`)

#### `main.py`
> **Purpose:** Main application entry point  
> **Description:** *Add details about what this script does, its inputs/outputs, and key functions.*

**Key Functions:**
```python
# Add function signatures and descriptions here
def main():
    """Main execution function"""
    pass
```

#### `setup.py`
> **Purpose:** Package configuration and installation script  
> **Description:** Defines package metadata, dependencies, and entry points.

---

### 2. New Level Module (`new_level/`)

#### `app/math_utils.py`
> **Purpose:** Mathematical utility functions  
> **Description:** *Add details about available math operations.*

**Available Functions:**
```python
# Example structure - replace with actual functions
def add(a, b):
    """Returns sum of two numbers"""
    pass

def multiply(a, b):
    """Returns product of two numbers"""
    pass
```

---

## 🧪 Testing

### Run Tests
```bash
# New workflow tests
python -m pytest New_workflow/test_main.py -v

# Math utils tests
python -m pytest new_level/tests/test_math_utils.py -v

# All tests
python -m pytest -v
```

### Test Coverage
```bash
pytest --cov=app --cov-report=html
```

---

## 🔄 CI/CD Pipeline

### GitLab CI Configuration
The project uses multiple `.gitlab-ci.yml` files for different workflows:

1. **Root Level:** Main pipeline configuration
2. **New Workflow:** Workflow-specific CI/CD
3. **New Level:** Module-specific CI/CD

**Pipeline Stages:**
- `test` - Run unit tests
- `build` - Build artifacts
- `deploy` - Deploy to environment

---

## 📝 Usage Examples

### Example 1: Using Math Utilities
```python
from new_level.app.math_utils import add, multiply

result = add(5, 3)
print(f"5 + 3 = {result}")
```

### Example 2: Running Main Workflow
```bash
python New_workflow/main.py
```

---

## 🤝 Contributing
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Merge Request

---

## 📄 License
*Add license information here*