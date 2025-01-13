# Data
This folder contains data created by the Congruence Engine project as part of the project's investigation into the different uses of Optical Character Recognition (OCR). 

The folder [worralls_1910_images](https://github.com/congruence-engine/experimenting-with-optical-character-recognition/tree/main/data/worralls_1910_images) contains example images from the 1910 Worrall's *Yorkshire Textile Directory* (pocket edition), which is representative of the kinds of documents that the project worked with. 

The file [Worralls_Companies_v10_Standardized.xlsx](https://github.com/congruence-engine/experimenting-with-optical-character-recognition/blob/main/data/Worralls_Companies_v10_Standardized.xlsx) is an example of a dataset created as a result of extracting OCR data from a series of documents. This dataset was created with a series of editions of the Worrall's *Yorkshire Textile Directory* (pocket edition) from the following years:
* 1889
* 1895
* 1900
* 1905
* 1910
* 1914
* 1920
* 1933
* 1936
* 1940

This dataset was created by using the following workflow:
1. Manual photography of the original images, using a smartphone camera - [see example for 1910](https://github.com/congruence-engine/experimenting-with-optical-character-recognition/tree/main/data/worralls_1910_images)
2. OCR carried out using Surya, resulting in a series of .txt files - [available here]()
3. Conversion of .txt files into csv format, using OpenAI's GPT API - [see code here](https://github.com/congruence-engine/experimenting-with-optical-character-recognition/blob/main/code/Surya/gpt_post_processing.ipynb). Note that this code uses a custom [prompt](https://github.com/congruence-engine/experimenting-with-optical-character-recognition/blob/main/code/Surya/gpt_prompt.txt) and [system prompt](https://github.com/congruence-engine/experimenting-with-optical-character-recognition/blob/main/code/Surya/system_text.txt). 
4. Manual correction of errors introduced as part of the above processes, including:
    * Entries missed out by Surya due to the small print of the input text
    * Hallucinations and omissions introduced by the OpenAI GPT post-processing
