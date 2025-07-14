# Reddit Russia-Ukraine Discourse Analysis

> 📌 **Note:** This repository is a **mirrored academic project** developed as part of a group assignment for CS 5664 (Knowledge Discovery from Text) at Virginia Tech.  
> All commit history and contributions reflect collaborative work from the original repository: [VT GitLab – cs5664-ukraine-term-project](https://code.vt.edu/brandonh03/cs5664-ukraine-term-project).

## Project Overview
This project analyzes Reddit discourse about the Russia-Ukraine war using network science and NLP techniques. It is divided into two main parts: network creation and analysis.

### Prerequisites
- Ensure all packages in `requirements.txt` are installed.
- Place all files in the same directory.

## Workflow
1. **Network Creation**
   - Run `make_network.ipynb` to process the dataset `reddit_opinion_ru_ua.csv` and generate the edgelist `network_similarity_vec.csv`.
2. **Network Analysis**
   - Run `network_analysis.ipynb` to perform graph analysis on the generated edgelist.
3. **Text Analysis**
   - Run `text_analysis.ipynb` for sentiment analysis and topic modeling.
   - In `text_analysis.ipynb`, the LDA topic number search is commented out for speed. Ideal `k` values are hard-coded. To run the search, uncomment the cell under "evaluate to find best number of topics" and remove the second argument. After viewing plots, add the second argument back to pinpoint the ideal `k`.
4. **Visualization**
   - `reddit.gephi` provides supplementary network visualizations using Gephi.

## Usage Notes
- Generate your own edge list `network_similarity_vec.csv` by running `make_network.ipynb`.
- Run each notebook sequentially from the top to the bottom cell for correct results.

## Files
- `make_network.ipynb`: Network creation from Reddit dataset.
- `network_analysis.ipynb`: Graph/network analysis.
- `text_analysis.ipynb`: Sentiment and topic modeling analysis.
- `reddit.gephi`: Gephi network visualization file.
- `requirements.txt`: List of required Python packages.
- `Reddit_Russia_Ukraine_Discourse_Analysis_Report.pdf`: Project report.

---
For questions or further details, see the original repository or contact the project contributors.