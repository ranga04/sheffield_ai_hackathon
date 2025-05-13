# sheffield_ai_hackathon

# SheffAware Colab Notebook

SheffAware aggregates Sheffield open data on public services, green spaces and infrastructure. It computes ward-level metrics and displays an interactive Folium map with controls to toggle individual features or view a composite equity score.

## Open the Notebook
1. Go to [Google Colab](https://colab.research.google.com/)  
2. Upload `SheffAware.ipynb` from this folder or open it via GitHub

## Data Sources
Download all raw data from the Sheffield City Council Open Data Portal:  
https://sheffield-city-council-open-data-sheffieldcc.hub.arcgis.com/

Key datasets to place in a `data/` folder:
- Ward boundaries (GeoJSON)  
- Libraries  
- School crossings  
- CCTV cameras  
- Recycling centres  
- Tree preservation orders  
- Parks and countryside  
- Local nature reserves  
- Wildlife sites  
- Flood zones  
- SuDS links  
- Drain nodes and links  
- Grit bins  

## Running the Analysis
1. Install dependencies in Colab:
   ```bash
   !pip install geopandas folium pandas scikit-learn


2. Ensure your `data/` folder is available (upload or mount Google Drive)
3. Update any file paths in the notebook to point to `data/`
4. Run all cells in order
5. Use the map cell’s feature controls to switch between metrics or show the equity score

## Exporting the Map

To save the interactive map as an HTML file:

```python
m.save('SheffAware_map.html')
```

## License

MIT License


