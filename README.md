## Dataset Preprocessing
- Step1: Download meta data from https://nijianmo.github.io/amazon/index.html.
- Step2: Put the meta data file in <tt>./data_preprocess/raw_data/</tt>.
- Step3: Set the dataset name (i.e., <tt>$dataset</tt>) in run.sh, run preprocessing by 
    ```
    cd data_preprocess
    sh run.sh
    ```
## Running Experiments
For the integration of low-frequency information and mid-frequency information, we provide four versions corresponding to the ablation study part of the paper.

Example of training, need to update the model layers to one of below in model.py
scomgnn: Item_Graph_Convolution 
Gat: Item_Graph_Convolution
GraphSage: Item_Graph_Convolution

```
python run.py
```


## Then post process and generate prompts
Under prompt folder
