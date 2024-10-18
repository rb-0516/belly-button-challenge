# Belly Button Biodiversity Dashboard

## Project Overview

This interactive dashboard explores the Belly Button Biodiversity dataset, which catalogs the microbes colonizing human navels. The dataset reveals that a small handful of microbial species (operational taxonomic units, or OTUs) were present in more than 70% of people, while the rest were relatively rare.

View the live dashboard: [Belly Button Biodiversity Dashboard](https://rb-0516.github.io/belly-button-challenge/)

## Features

1. **Data Source**: The dashboard reads data from `samples.json` using D3.js.

2. **Dropdown Menu**: Users can select different test subjects using a dropdown menu.

3. **Demographic Info Panel**: Displays metadata about the selected individual.

4. **Bar Chart**: Shows the top 10 OTUs found in the selected individual.
   - Uses `sample_values` for bar heights
   - Uses `otu_ids` for labels
   - Uses `otu_labels` for hover text

5. **Bubble Chart**: Visualizes the relative frequency of all OTUs in the selected individual.
   - X-axis: `otu_ids`
   - Y-axis: `sample_values`
   - Marker size: `sample_values`
   - Marker colors: `otu_ids`
   - Text values: `otu_labels`

6. **Interactive Elements**: All visualizations update when a new sample is selected from the dropdown menu.

## Technologies Used

- HTML/CSS
- JavaScript
- D3.js
- Plotly.js

## Setup and Deployment

1. The project is deployed on GitHub Pages.
2. To run locally, clone this repository and open `index.html` in a web browser.

## File Structure

- `index.html`: The main HTML file
- `static/js/app.js`: Contains the JavaScript code for the dashboard
- `samples.json`: Contains the dataset (not included in the repository, fetched from a URL)

## Development Process

This project was developed as part of a data visualization challenge. It involved the following steps:

1. Data loading and parsing using D3.js
2. Creating interactive charts with Plotly.js
3. Implementing dynamic updates based on user selection
4. Deploying the finished product to GitHub Pages

## Future Improvements

- Add additional visualizations to explore the data further
- Implement responsive design for better mobile experience
- Include more detailed statistical analysis of the data

## Credits

Data provided by the [Belly Button Biodiversity project](http://robdunnlab.com/projects/belly-button-biodiversity/).

