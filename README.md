# DeepChrome

This repo contains deep learning models for building interpretable representations of epigenetic markers
that can predicting gene expression.

[QData lab](https://qdata.github.io/qdata-page/categories/AIbiomed//) at
the University of Virginia.

## Projects
![Overview Image](https://qdata.github.io/qdata-page/pic/interpretDeep.png)

The below methods all aim to predict gene expression; however, the methods differ in their implementation and biological interpretations.
For the most part, the programs build from top to bottom.

|                                    | **Input Data**                                                                                    | **Output**                   | **Method**                         | **Biological Insight**                                |
|------------------------------------|---------------------------------------------------------------------------------------------------|------------------------------|------------------------------------|-------------------------------------------------------|
| [DeepChrome](DeepChrome)           | histone modifications                                                                             | gene expression              | Convolutional Neural Network       | Nearby Combinations of histone modifications          |
| [AttentiveChrome](AttentiveChrome) | histone modifications                                                                             | gene expression              | Long Short-Term Memory Unit        | Longer distance dependencies of histone modifications |
| [DeepDiffChrome](DeepDiffChrome)   | histone modifications                                                                             | differential gene expression | Long Short-Term Memory Unit        | Representations across Cell Types                     |
| [ChromeGCN](ChromeGCN)             | histone,  transcription factors, chromatin accessibility (DNAse I), chromatin organization (Hi-C) | gene expression              | Graph Convolutional Neural Network | Distal promoter elements                              |
