
# 🗺️ Locating the Forgotten Data Type: Intro to Geospatial Analysis with Python

Welcome! This repository supports a talk given at the Python Meetup 2025, titled:

> **"Locating the Forgotten Data Type: Intro to Geospatial Analysis with Python"**  
> By Haris Ballis

This repo includes a practical notebook and code samples showcasing how to work with geospatial data in Python — from constructing simple geometries to performing real-world spatial queries and visualizations.

---

## 🧠 What You’ll Learn

- What geospatial data types are and why they matter
- How to construct and store geometries using Shapely
- How spatial context reduces database complexity
- How to query and visualize real-world data (e.g., cafes along a road)
- Introduction to spatial indexing (H3), projections, and formats

---

## 📦 Dependencies

Install the requirements using `pip` or `uv`:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

---

## 📁 Key Notebook: `cafes_along_road.ipynb`

This notebook:
- Downloads an OpenStreetMap road network using `osmnx`
- Selects a target road (`Δημητρίου Γούναρη`) and creates a buffered area around it
- Queries **Google Places API** for cafes and bakeries along the road
- Uses `GeoPandas` for spatial filtering, intersection, and joining
- Calculates inter-cafe distances and density
- Aggregates points into **H3 hexagonal cells** for spatial summaries
- Visualizes the results with `plotly`

---

## 🔐 API Access

This example uses the **Google Places API**. Set your API key as an environment variable:

```bash
export GOOGLE_API_KEY=your_key_here
```

---

## 🧭 License

MIT License. Feel free to adapt or build on this work — just give credit where it's due.

---

## 🙋‍♂️ About the Author

Haris Ballis – geospatial analyst, Python enthusiast, and optimization geek.  
🔗 [github.com/harisbal](https://github.com/harisbal)
