# Data Lake Layering Project

This project demonstrates the implementation of a multi-layered data lake architecture using Python. The goal is to process datasets through multiple layers, enhancing the quality and utility of the data at each stage.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Layers in the Data Lake](#layers-in-the-data-lake)
- [Setup Instructions](#setup-instructions)
- [Data Operations](#data-operations)
- [Enriched Layer](#enriched-layer)
- [Example Dataset](#example-dataset)
- [Execution](#execution)
- [Contributing](#contributing)
- [License](#license)

---

## Project Overview

The project organizes datasets into multiple layers within a data lake, applying transformations and enhancements at each stage:
1. **Raw Layer**: Initial layer for storing raw, unprocessed data.
2. **Refined Layer**: Contains data after basic processing.
3. **Curated Layer**: Contains cleaned and transformed data for specific use cases.
4. **Enriched Layer** (New): Adds further enhancements such as calculated fields, additional transformations, or metadata enrichment.

---

## Layers in the Data Lake

1. **Raw Layer**:
   - Stores data exactly as ingested from the source.
   - No transformations are applied.

2. **Refined Layer**:
   - Applies basic data processing, such as marking rows as processed.

3. **Curated Layer**:
   - Applies cleaning and transformation steps to prepare the data for analysis or downstream applications.

4. **Enriched Layer** (New):
   - Adds advanced data operations, such as calculated fields or additional enrichments.
   - Example: Adding a "Bonus" column derived from the "Salary" column.

---

## Setup Instructions

### Prerequisites
- Python 3.7 or higher
- Required libraries:
  - `pandas`
  - `os`
  - `shutil`

Install dependencies:
```bash
pip install pandas
