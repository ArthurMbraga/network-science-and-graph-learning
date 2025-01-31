# Network Analysis Project

This project involves the analysis of various university networks using assortativity and link prediction techniques.

## Project Structure

```
.gitignore
assortativity_results.csv
data/
    American75.gml
    Amherst41.gml
    Auburn71.gml
    Baylor93.gml
    ...
images/
project.ipynb
```

- `assortativity_results.csv`: Contains the assortativity results for various networks.
- `data/`: Directory containing `.gml` files for different university networks.
- `images/`: Directory for storing images generated during the analysis.
- `project.ipynb`: Jupyter notebook for running the analysis.

## Data

You can download the dataset from [here](https://partage.imt.fr/index.php/s/iyFWSQPJNmc7AC7).

```bash
wget https://partage.imt.fr/index.php/s/iyFWSQPJNmc7AC7/download -O dataset.zip
```

## Assortativity Analysis

The assortativity results are stored in `assortativity_results.csv`. The columns include:
- `network`: The network file name.
- `size`: The size of the network.
- `student_fac`: Assortativity based on student-faculty relationships.
- `major_index`: Assortativity based on major index.
- `degree`: Assortativity based on degree.
- `dorm`: Assortativity based on dormitory.
- `gender`: Assortativity based on gender.

## Link Prediction

The link prediction results are stored in `link_prediction_results.txt`. The results include various metrics such as Common Neighbors, Jaccard, and Adamic-Adar for different thresholds and top values.

## Running the Analysis

To run the analysis, open the `project.ipynb` notebook and execute the cells. Ensure you have the necessary dependencies installed.

## Dependencies

- Python 3.x
- Jupyter Notebook
- NetworkX
- Pandas
- NumPy