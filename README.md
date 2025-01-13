
# S&P Cosmograph Visualization

This repository contains a Jupyter Notebook that leverages the [py-cosmograph](https://github.com/cosmograph-org/py_cosmograph) library to create a cosmographic visualization of S&P data. The visualization groups companies by their respective sectors, displaying them in distinct, non-overlapping clusters arranged in a circular layout.

## Features

- **Sector-Based Clustering**: Companies are grouped into clusters based on their sector.
- **Non-Overlapping Clusters**: Clusters are arranged with sufficient spacing to avoid visual overlap.
- **Customizable Layout**: The visualization layout can be adjusted for spacing, clustering logic, and style.
- **HTML Export**: The resulting cosmograph is saved as an interactive HTML file.

## Requirements

- Python 3.8+
- Required libraries:
  - `pandas`
  - `cosmograph`

You can install the dependencies using the following command:
```bash
pip install pandas cosmograph
```

## Usage

1. **Prepare Your Dataset**:
   - Ensure your dataset is a CSV file containing at least the following columns:
     - `Sector`: The sector each company belongs to.
     - `Company`: The name of the company.

2. **Update the Notebook**:
   - Replace the placeholder `your_dataset.csv` in the notebook with the path to your dataset file.

3. **Run the Notebook**:
   - Execute the cells in the notebook to process the data and generate the cosmograph visualization.

4. **View the Visualization**:
   - The visualization will be saved as `cosmograph_visualization.html` in the working directory. Open this file in a web browser to interact with the cosmograph.

## Notebook Structure

1. **Imports and Setup**: Imports required libraries and loads the dataset.
2. **Data Preprocessing**: Ensures the dataset is correctly formatted.
3. **Cluster Creation**: Groups companies into clusters based on their sectors.
4. **Graph Construction**: Creates a graph and adds clusters to it.
5. **Visualization Rendering**: Configures the layout and renders the cosmograph as an HTML file.

## Example Visualization Output

The cosmograph arranges sectors in a circular pattern, with companies clustered by their sector. Each cluster is spaced apart to ensure clarity and visual distinction.

## Customization

You can modify the following parameters in the notebook:
- `layout_options`:
  - `type`: The layout style (e.g., circular).
  - `cluster_separation`: The spacing between clusters.
- Dataset: Update or preprocess your data to fit specific needs.

## Repository and Documentation

For more information about the `py-cosmograph` library, visit the [official repository](https://github.com/cosmograph-org/py_cosmograph).

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Feel free to contribute by opening issues or submitting pull requests!
