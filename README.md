# CSE-551 Graph Theory: Community Detection in Protein Graphs vs. Hypergraphs for Gene Function Prediction: A Comparative Study Using hyperNETX & GOAtools

## Overview

Community detection in biological networks, such as protein-protein interaction (PPI) networks, is a critical step in understanding gene functions and cellular processes. This project investigates the effectiveness of traditional graph models versus advanced hypergraph models in detecting protein communities. These communities provide insights into the functional groupings of proteins and help identify enriched Gene Ontology (GO) terms, improving our ability to predict gene functions and understand complex biological systems. The study also compares these techniques to a similar analysis applied to the **YouTube social network**, where community detection aims to uncover user behavior and interaction patterns.

## Project Goals

- Investigate the application of graph and hypergraph models for community detection in protein interaction networks.
- Compare the performance of traditional graph-based and hypergraph-based approaches in uncovering meaningful protein communities.
- Identify GO term enrichment within the identified protein communities to enhance functional prediction accuracy.
- **Community Detection in YouTube Network**: Compare protein interaction communities with social network communities for insight into structural differences and similarities.

## Methodology

### Data Representation

1. **Protein Graphs**: In traditional graphs, proteins are represented as nodes, and interactions between them as edges. Each edge corresponds to a direct interaction between two proteins. This representation captures pairwise interactions but may fail to account for more complex, higher-order relationships between proteins.

2. **Protein Hypergraphs**: Hypergraphs generalize the idea of interactions by allowing hyperedges, which can link multiple proteins at once. These higher-order relationships can better capture the multifaceted nature of protein interactions, such as protein complexes and multi-protein assemblies, leading to a more comprehensive understanding of protein functions.

3. **YouTube Graphs**: In the YouTube social network, users are modeled as nodes, and interactions between users (e.g., comments, likes, shares) as edges. This captures pairwise social relationships and interactions in a simplified way.

4. **YouTube Hypergraphs**: Hypergraphs in the YouTube context capture interactions involving multiple users (e.g., collaborative content creation or group discussions), providing a richer representation of community structures.

### Tools and Libraries

- **NetworkX**: For handling and analyzing traditional graph-based structures.
- **HyperNETX**: For the analysis of hypergraphs, particularly useful in representing higher-order interactions.
- **GOA Enrichment Analysis**: For assessing the functional enrichment of GO terms within the identified protein communities.

### Community Detection Techniques

- **Louvain Modularity**: A widely used method for detecting communities by optimizing the modularity of the network. This technique is applied to both graph and hypergraph structures to find cohesive subgroups.
- **Spectral Clustering**: A clustering technique that utilizes the eigenvalues of the graph's Laplacian matrix to identify clusters of proteins in both graphs and hypergraphs.

### Data Processing

1. Convert the protein interaction data into both graph and hypergraph formats.
2. Convert the YouTube social network data into both graph and hypergraph formats.
3. Apply community detection algorithms to both protein and YouTube networks to identify functional communities.
4. Perform GO term enrichment analysis on the identified protein communities to evaluate their functional relevance.

## Research Questions

- **How do hypergraphs compare to traditional graphs in capturing protein community structures?**
- **Can hypergraph-based community detection reveal more biologically meaningful protein communities that are enriched with specific Gene Ontology (GO) terms?**
- **Do hypergraphs provide a more accurate representation of social dynamics and community structures within the YouTube network compared to traditional graph models?**
  
## Expected Outcomes

- **Protein Networks**: This research is expected to demonstrate that hypergraphs, by capturing higher-order interactions, offer a more accurate representation of protein communities. Identifying enriched GO terms within these communities will enhance the accuracy of gene function predictions and lead to a deeper understanding of molecular mechanisms.
  
- **YouTube Network**: The findings will provide insights into the potential of hypergraph-based community detection in social networks, comparing its performance to traditional graph methods for applications such as content recommendation, user segmentation, and influencer identification.

## Conclusion

Through a comparative study of graph-based and hypergraph-based community detection methods, this research aims to improve gene function prediction by uncovering more biologically relevant communities in protein interaction networks. The integration of GO term enrichment analysis will further strengthen the predictive power of these community detection methods. Additionally, the study will assess the applicability of these methods to social networks, providing broader insights into network structure detection.

---

## **Do's and Done**

### **To Do:**
- Convert protein interaction data into both graph and hypergraph formats.
- Implement and compare community detection algorithms (Louvain, Spectral Clustering) on both graph and hypergraph formats.
- Perform GO term enrichment analysis on the identified protein communities.
- Replicate the community detection process for the YouTube social network and compare results with protein networks.

### **Done:**
- Set up the research framework and defined the goals for comparing graph and hypergraph community detection methods.
- Gathered and preprocessed protein interaction data and YouTube network data.
- Investigated the integration of hypergraphs and their potential advantages over traditional graph models.
- Implemented initial steps in using **NetworkX** and **hyperNETX** for community detection.
- Started working with GOA enrichment analysis to identify functional insights within protein communities.

---

### **References**
- **NetworkX**: https://networkx.org/documentation/stable/reference/index.html
- **HyperNETX**: https://github.com/pnnl/HyperNetX
- **GOA Enrichment Analysis**: https://github.com/tanghaibao/goatools
