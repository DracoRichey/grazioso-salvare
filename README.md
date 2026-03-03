# Grazioso Salvare Animal Rescue Dashboard

An interactive data analytics dashboard built for a rescue animal training organization, enabling staff to filter and identify candidate animals for search-and-rescue operations based on breed, age, and training suitability.

## 📸 Screenshot
*(Add a screenshot of the running dashboard here)*

## 🛠️ Tech Stack

- **Python** — core application logic
- **MongoDB** — NoSQL database for animal shelter records
- **Dash** — interactive web dashboard framework
- **Pandas** — data filtering and classification
- **Plotly** — data visualization and geospatial mapping

## 🔧 Features

- **Modular CRUD module** (`animal_shelter.py`) — reusable Python class with create, read, update, and delete operations against MongoDB
- **Dynamic filtering** — Dash callbacks filter the dataset in real time based on rescue type (Water Rescue, Mountain/Wilderness, Disaster/Individual Tracking)
- **Interactive data table** — sortable, paginated view of shelter animal records
- **Geospatial map** — visualizes animal locations based on filtered results
- **Data classification** — Pandas-based rule logic identifies training-suitable candidates by breed and age range

## 🏗️ Architecture

The project is split into two layers:

1. **Data layer** (`animal_shelter.py`) — a standalone CRUD class that handles all MongoDB interactions. Designed to be reusable across projects with minimal reconfiguration.
2. **Dashboard layer** (`ProjectTwoDashboard.ipynb`) — a Dash application that imports the CRUD module and renders an interactive UI with filtering, visualization, and mapping components.

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- MongoDB running locally or via Atlas
- Required packages:

```bash
pip install dash pandas plotly pymongo jupyter
```

### Running the Dashboard
1. Clone the repository
2. Ensure MongoDB is running and populated with shelter data
3. Open `ProjectTwoDashboard.ipynb` in Jupyter
4. Run all cells — the Dash app will launch in your browser

## 📁 Project Structure

```
├── animal_shelter.py         # Reusable MongoDB CRUD module
├── Project 2.ipynb           # Data exploration and testing
├── ProjectTwoDashboard.ipynb # Main Dash dashboard application
└── README.md
```
