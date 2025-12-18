# Service Repository: VOLIA.one Ukrainian language project

**"VOLIA.one — Learn the Language of Freedom"**

This repository is the centralized service layer for the **VOLIA.one** project. It stores shared data, system documentation, and configuration logic used by the VOLIA.one website and FlutterFlow application.

## 📂 Directory Structure
- `/data`: JSON-based master data (curriculum, prompts, configs).
- `/docs`: Technical specifications for the WordPress bridge and app integrations.
- `/scripts`: Utilities for data transformation or maintenance.

## 🔄 Data Pipeline
1. **Source**: WordPress Admin (ACF Pro).
2. **Bridge**: WPCodeBox 2 (PHP) pushes data via GitHub REST API.
3. **Consumer**: FlutterFlow App via GitHub Raw API calls.

## 🛠 Schema: /data/vocabulary.json
The curriculum data follows this structure:
- `ukrainian`: Cyrillic text.
- `english`: Translation.
- `category`: Primary grouping.
- `sub_category`: Specific lesson/set.
- `is_phrase`: Boolean (True if entry is a sentence).

## 📜 Documentation
See [ETHICS.md](./ETHICS.md) for the project philosophy, privacy architecture, and pricing model.