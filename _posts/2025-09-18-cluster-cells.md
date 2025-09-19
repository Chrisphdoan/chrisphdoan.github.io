---
layout: post
title: "Clustering Cells in Single Cell Analysis"
date: 2025-09-18
categories: bioinformatics
---
How do we cluster cells in single-cell RNA-seq?  

Graph-based clustering (Seurat)  
FindNeighbors() has default k = 20, k-nearest neighbor (kNN)  
https://bioconductor.org/books/3.15/OSCA.basic/clustering.html  
1. Similarity is computed. Euclidean distance or cosine similarity  
2. Nearest neighbors are found
3. A graph (network) is built. Cells = nodes, neighbor relationships = edges, stronger similarity = stronger edge weight.  
4. Communities (clusters) are detected. Clustering algorithms in single cell: Louvain or Leiden

