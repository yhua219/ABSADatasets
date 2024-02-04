# Data Preparation Tool

## Steps to annotate custom datasets for PyABSA
- 1. Pre-word segmentation
- 2. Annotate the segmented data
- 3. convert the apc dataset to atepc dataset
- 4. merge your custom dataset into integrated_datasets and PR

You can find the tool scripts at https://github.com/yangheng95/ABSADatasets/tree/v2.0/DPT

## 1. Pre-word segmentation
Before annotating non-blank segmented text (e.g., English), you need to segment the data. Run `pre_word_segment_for_non_english_data.py` and
select the output file `*.seg` to annotate.


## 2. ASTE_DPT:  A Stand-alone browser based multi-purpose manual data annotation tool for ABSA

 This repository contains [<b>ASTE_DPT</b>](https://github.com/yhua219/ABSADatasets/blob/v2.0/DPT/2_ASTE_DPT.html), an extended version of the ABSA Dataset Prepare Tool (DPT) [(source)](https://github.com/yangheng95/ABSADatasets/tree/v2.0/DPT) for Aspect-based Sentiment Analysis (ABSA) training dataset annotation. 
 
 ASTE_DPT is a no-code, no-installation small HTML file that can be used locally without a server to protect data security/privacy. 

## <font color='yellowgreen'>How to use:</font>

 You can download the [<b>2_ASTE_DPT.html</b>](https://github.com/yhua219/ABSADatasets/tree/v2.0/DPT) file and open it in a browswer to use locally.
 
 You can also use this [<b>ASTE_DPT online version</b>](https://yhua219.github.io/ASTE_DPT/). 

The main features and steps are illustrated in the [Usage Instructions](https://github.com/yhua219/ABSADatasets?tab=readme-ov-file#usage-instructions) below.

 For sample input data files, please try any of the files in [DPT/sample_data](https://github.com/yhua219/ABSADatasets/tree/v2.0/DPT/sample_data) subdirectory:

 * The .seg and .csv files are raw text files for annotation

 * The "ABSADataWorkFile.json" is an example export file containing saved annotation progress to be restored. 

 --------------------

## <font color='yellowgreen'>Input and output files:</font>
 
 ASTE_DPT input: &emsp; &ensp; A CSV file with text entries.

 ASTE_DPT outputs: &ensp; A zip file containing 4 dataset files: 
  1) Training data files for Aspect-Sentiment-Triplet Extraction (ASTE) (new feature).

  2) Training data files for Aspect-sentiment Classification (ASC), Aspect-term Extraction (AE) (from the original DPT), and Opinion-term extraction (OE) (new feature).

  3) Training data files for sentence-level Sentiment-analysis (from the original DPT).  

  4) Underlying data file that preserves progress and can be uploaded to restore previous progress and continue the annotation. 
 

 All the output files follow the same format as in the [Datasets](https://github.com/yangheng95/ABSADatasets/tree/v2.0/datasets) subdirectory. These dataset files can be used by models in [PyABSA](https://github.com/yangheng95/PyABSA).

<br>

<i>Please visit [ABSA Dataset](https://github.com/yangheng95/ABSADatasets) for more information about the datasets and the original files (files other than 2_ASTE_DPT) in this repository.</i>

<br>

---------------------------------------------
## <font color='yellowgreen'>Usage Instructions</font>

![ASTE_DPT instructions](https://github.com/yhua219/ABSADatasets/blob/v2.0/ASTE_DPT%20instructions.png?raw=true)



