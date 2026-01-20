# Bangalore Walkability Index

A personalized accessibility framework that integrates exponential decay functions with user-customizable weighting systems for real-time urban evaluation.

## Live Demo

**[Try it live](https://bangalore-walkability-index.netlify.app/)**

## Overview

This web application implements a personalized accessibility measurement framework for Bangalore, India. Users can evaluate neighborhoods based on their individual priorities and lifestyle requirements, going beyond one-size-fits-all walkability scores.

## Key Features

- **Personalized Evaluation**: Customize which amenities matter to you
- **Dynamic Weighting**: Set amenities as Standard, Preferred, or Required
- **Service Grouping**: Group similar services that you consider substitutable
- **Exponential Decay**: Control how much you value redundancy vs. diversity
- **Dual Visualization**: Grid-level (fine-grained) and Ward-level (comparative) views
- **Real-time Analysis**: Instant results as you adjust parameters

## Technology Stack

- **Frontend**: HTML, CSS, JavaScript
- **Mapping**: Leaflet.js with OpenStreetMap
- **Data**: OpenStreetMap amenity data (45+ categories)
- **Routing**: Valhalla routing engine for 15-minute walking catchments

## How It Works

### Methodology

1. **Grid-Based Discretization**: Bangalore divided into 250m × 250m cells
2. **Catchment Analysis**: Pre-computed 15-minute walking isochrones for 20,000+ amenities
3. **Exponential Decay**: Diminishing returns from overlapping services
4. **Real-time Calculation**: Lightweight scoring as users adjust preferences

## Data Sources

- **Ward Boundaries**: Urban Data Portal (BBMP)
- **Amenities**: OpenStreetMap (July 2025)
- **Routing**: Valhalla with OSM network data
- **Coordinate System**: WGS84 (EPSG:4326)

## Citation

If you use this tool in your research, please cite:

```bibtex
@article{ghuriki2025walkability,
  title={One Size Fits None: A Personalized Framework for Urban Accessibility Using Exponential Decay},
  author={Ghuriki, Prabhanjana and Chanti, S.},
  year={2025},
  institution={CHRIST (Deemed to be University)}
}
```
