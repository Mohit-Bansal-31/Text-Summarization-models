# Text Summarization Model Evaluation

## Overview
In this study, we evaluated four pretrained text summarization models from Hugging Face:
- `bart-large-cnn`
- `t5-tokenizer`
- `distilbart-cnn`
- `bart-large-cnn-samsum`

These models were tested on five text domains:
- **Health**
- **Politics**
- **Sports**
- **Technology**
- **Finance**

Each domain consisted of five texts, and we applied the **TOPSIS** method to rank the models based on five evaluation metrics:
- **Meteor Score**
- **Bleu Score**
- **Rouge-1 Score**
- **Gunning-Fog Index**
- **Flesch-Kincaid Readability Score**

The results for each domain are presented below.

## Evaluation Results by Domain

### Health Domain
The models were tested on five different health-related texts. The evaluation criteria focused on summarization quality and readability, ensuring that the most effective model for health-related content was identified.

**Results for the Health domain are as follows:**

| Text | Model                  | Meteor Score | Bleu Score | Rouge-1 Score | Gunning-Fog Index | Flesch-Kincaid | Topsis Score | Rank |
|------|------------------------|--------------|------------|---------------|-------------------|----------------|--------------|------|
| T1   | bart-large-cnn         | 0.219602     | 3.657375   | 0.393939      | 12.68             | 10.2           | 0.68073      | 2    |
|      | **t5-tokenizer**       | **0.181226** | **4.007935** | **0.367647**  | **7.25**          | **8.4**        | **0.782152** | **1** |
|      | distilbart-cnn         | 0.154201     | 0.773349   | 0.360566      | 9.8               | 9.3            | 0.487152     | 4    |
|      | bart-large-cnn-samsum  | 0.19759      | 1.788384   | 0.412214      | 12.68             | 11.1           | 0.357557     | 3    |
| T2   | bart-large-cnn         | 0.217897     | 5.652792   | 0.468085      | 14.32             | 10.8           | 0.584889     | 2    |
|      | t5-tokenizer           | 0.163337     | 2.968577   | 0.340136      | 9.17              | 12.2           | 0.380412     | 4    |
|      | distilbart-cnn         | 0.202219     | 6.387366   | 0.455515      | 16.08             | 13.5           | 0.551979     | 3    |
|      | **bart-large-cnn-samsum** | **0.241499** | **6.628251** | **0.42029**   | **11.41**         | **10.4**       | **0.772343** | **1** |
| T3   | bart-large-cnn         | 0.194193     | 3.350138   | 0.337838      | 12.68             | 11.1           | 0.424205     | 3    |
|      | **t5-tokenizer**       | **0.197888** | **6.824422** | **0.408451**  | **13.16**         | **13.0**       | **0.856718** | **1** |
|      | distilbart-cnn         | 0.177173     | 3.506127   | 0.305415      | 11.34             | 11.1           | 0.498213     | 2    |
|      | bart-large-cnn-samsum  | 0.159817     | 1.02372    | 0.230216      | 15.91             | 13.9           | 0.189972     | 4    |
| T4   | bart-large-cnn         | 0.18837      | 5.347337   | 0.315068      | 9.32              | 7.3            | 0.707321     | 2    |
|      | t5-tokenizer           | 0.192421     | 5.064896   | 0.346667      | 10.74             | 7.7            | 0.674528     | 3    |
|      | **distilbart-cnn**     | **0.205873** | **7.067582** | **0.331231**  | **13.07**         | **8.9**        | **0.782394** | **1** |
|      | bart-large-cnn-samsum  | 0.162436     | 1.028423   | 0.25          | 10.7              | 8.3            | 0.186088     | 4    |
| T5   | bart-large-cnn         | 0.148393     | 1.559808   | 0.277778      | 19.42             | 13.9           | 0.274549     | 4    |
|      | t5-tokenizer           | 0.164046     | 0.752475   | 0.242991      | 9.18              | 5.6            | 0.329668     | 3    |
|      | distilbart-cnn         | 0.181049     | 0.950305   | 0.35514       | 15.31             | 11.1           | 0.716693     | 2    |
|      | **bart-large-cnn-samsum** | **0.186122** | **9.388488** | **0.350877**  | **8.0**           | **8.4**        | **0.820569** | **1** |


### Politics Domain
For political texts, the models were evaluated based on their ability to capture key points while maintaining coherence and readability. Political discourse often contains complex structures, making this evaluation crucial.

**Results for the Politics domain are as follows:**

| Text | Model                  | Meteor Score | Bleu Score | Rouge-1 Score | Gunning-Fog Index | Flesch-Kincaid | Topsis Score | Rank |
|------|------------------------|--------------|------------|---------------|-------------------|----------------|--------------|------|
| T1   | bart-large-cnn         | 0.264528     | 7.723828   | 0.384         | 11.47             | 8              | 0.511318     | 2    |
|      | t5-tokenizer           | 0.274338     | 7.426853   | 0.369231      | 16                | 13.6           | 0.476561     | 3    |
|      | distilbart-cnn         | 0.304545     | 4.979768   | 0.432         | 12.49             | 9.3            | 0.365259     | 4    |
|      | **bart-large-cnn-samsum**  | **0.28118**      | **9.247552**   | **0.416**         | **10.36**             | **8**              | **0.65209**      | **1**    |
| T2   | bart-large-cnn         | 0.495135     | 26.60834   | 0.637931      | 15.24             | 12.2           | 0.873284     | 2    |
|      | t5-tokenizer           | 0.135263     | 0.531238   | 0.204082      | 11.56             | 7.8            | 0.165111     | 4    |
|      | **distilbart-cnn**         | **0.516605**     | **27.6176**    | **0.556452**      | **14.97**             | **11.4**           | **0.876013**     | **1**    |
|      | bart-large-cnn-samsum  | 0.393199     | 19.50808   | 0.550459      | 17.39             | 13.5           | 0.668141     | 3    |
| T3   | bart-large-cnn         | 0.278454     | 10.33371   | 0.45614       | 9.25              | 6.7            | 0.290805     | 3    |
|      | t5-tokenizer           | 0.26804      | 12.37826   | 0.40678       | 8                 | 4.8            | 0.484647     | 2    |
|      | distilbart-cnn         | 0.298879     | 7.475518   | 0.438095      | 8.1               | 5.5            | 0.789396     | 4    |
|      | **bart-large-cnn-samsum**  | **0.346449**     | **18.03983**   | **0.48062**       | **8**                 | **7.1**            | **0.789937**     | **1**    |
| T4   | bart-large-cnn         | 0.227575     | 4.496155   | 0.368         | 21.17             | 17.4           | 0.630547     | 1    |
|      | t5-tokenizer           | 0.162744     | 1.234318   | 0.269231      | 8.11              | 7.6            | 0.372882     | 3    |
|      | distilbart-cnn         | 0.187491     | 3.343718   | 0.21083       | 19.67             | 15.6           | 0.429087     | 2    |
|      | bart-large-cnn-samsum  | 0.208101     | 1.355375   | 0.392857      | 17.03             | 14.4           | 0.340136     | 4    |
| T5   | **bart-large-cnn**         | **0.246378**     | **5.07381**    | **0.472441**      | **9.04**              | **7.1**            | **0.745717**     | **1**    |
|      | t5-tokenizer           | 0.195414     | 1.986426   | 0.36985       | 10.4              | 7.2            | 0.187606     | 4    |
|      | distilbart-cnn         | 0.201078     | 3.298672   | 0.394161      | 12.71             | 11.2           | 0.428417     | 3    |
|      | bart-large-cnn-samsum  | 0.208092     | 3.789361   | 0.459259      | 9.47              | 6.7            | 0.519339     | 2    |

### Sports Domain
Summarization of sports texts required capturing dynamic events and essential highlights concisely. The models were assessed based on their ability to retain the most relevant details while keeping the summaries concise and readable.

**Results for the Sports domain are as follows:**

| Text | Model                  | Meteor Score | Bleu Score | Rouge-1 Score | Gunning-Fog Index | Flesch-Kincaid | Topsis Score | Rank |
|------|------------------------|--------------|------------|---------------|-------------------|----------------|--------------|------|
| T1   | bart-large-cnn         | 0.309986     | 10.50628   | 0.475248      | 11.4              | 11.9           | 0.414225     | 3    |
|      | t5-tokenizer           | 0.236642     | 5.611869   | 0.268908      | 5.9               | 8.3            | 0.281866     | 4    |
|      | distilbart-cnn         | 0.35334      | 14.06789   | 0.504854      | 11.51             | 12.3           | 0.571397     | 2    |
|      | **bart-large-cnn-samsum**  | **0.42705**      | **18.24812**   | **0.588235**      | **10.33**             | **11.1**           | **0.760236**     | **1**    |
| T2   | bart-large-cnn         | 0.422585     | 21.25477   | 0.573643      | 9.68              | 8.2            | 0.787477     | 2    |
|      | t5-tokenizer           | 0.166161     | 3.2898     | 0.316832      | 10.68             | 7.1            | 0.149055     | 4    |
|      | distilbart-cnn         | 0.341426     | 18.59747   | 0.59375       | 6.89              | 4.4            | 0.698445     | 3    |
|      | **bart-large-cnn-samsum**  | **0.403466**     | **19.76247**   | **0.616667**      | **6.13**              | **4.7**            | **0.79782**      | **1**    |
| T3   | bart-large-cnn         | 0.050891     | 0.333802   | 0.09434       | 11.31             | 7.6            | 0.321341     | 4    |
|      | t5-tokenizer           | 0.061989     | 1.114454   | 0.051282      | 7.37              | 3.1            | 0.539278     | 2    |
|      | **distilbart-cnn**         | **0.340006**     | **6.058932**   | **0.132231**      | **14.09**             | **9.3**            | **0.584631**     | **1**    |
|      | bart-large-cnn-samsum  | 0.353664     | 0.610592   | 0.101695      | 11.81             | 9.5            | 0.514743     | 3    |
| T4   | **bart-large-cnn**         | **0.295131**     | **6.774294**   | **0.473282**      | **14.17**             | **10.1**           | **0.818364**     | **1**    |
|      | t5-tokenizer           | 0.135989     | 1.597928   | 0.205128      | 9.28              | 7.3            | 0.18341      | 3    |
|      | distilbart-cnn         | 0.258718     | 5.154616   | 0.375         | 14.26             | 11.1           | 0.627959     | 2    |
|      | bart-large-cnn-samsum  | 0.13182      | 1.980429   | 0.266667      | 12.76             | 10.1           | 0.155333     | 4    |
| T5   | bart-large-cnn         | 0.136897     | 7.924632   | 0.261682      | 13.32             | 10.8           | 0.617854     | 2    |
|      | t5-tokenizer           | 0.047043     | 0.294456   | 0.113636      | 11.32             | 7.4            | 0.052304     | 4    |
|      | **distilbart-cnn**         | **0.201038**     | **11.47843**   | **0.348264**      | **10.76**             | **6.0**            | **0.89856**      | **1**    |
|      | bart-large-cnn-samsum  | 0.138522     | 7.166926   | 0.32          | 12.88             | 7.6            | 0.615087     | 3    |


### Technology Domain
Technology-related texts often contain technical terms and detailed explanations. The evaluation in this domain focused on summarization accuracy and clarity, ensuring the summaries were both informative and accessible.

**Results for the Technology domain are as follows:**

| Text | Model                  | Meteor Score | Bleu Score | Rouge-1 Score | Gunning-Fog Index | Flesch-Kincaid | Topsis Score | Rank |
|------|------------------------|--------------|------------|---------------|-------------------|----------------|--------------|------|
| T1   | bart-large-cnn         | 0.199273     | 3.556854   | 0.318841      | 9.56              | 6.8            | 0.14916      | 4    |
|      | t5-tokenizer           | 0.186449     | 4.986463   | 0.272727      | 9.38              | 7.5            | 0.201449     | 3    |
|      | distilbart-cnn         | 0.323883     | 9.737795   | 0.450946      | 10.34             | 8.2            | 0.770367     | 2    |
|      | **bart-large-cnn-samsum**  | **0.372504**     | **9.54145**    | **0.515152**      | **8.41**              | **5.1**            | **0.819899**     | **1**    |
| T2   | **bart-large-cnn**         | **0.2607**       | **11.05018**   | **0.412121**      | **9.41**              | **8.3**            | **0.741195**     | **1**    |
|      | t5-tokenizer           | 0.245106     | 8.937777   | 0.402778      | 8.61              | 7.8            | 0.374791     | 3    |
|      | distilbart-cnn         | 0.238178     | 7.662261   | 0.374038      | 9.81              | 8.2            | 0.370067     | 4    |
|      | bart-large-cnn-samsum  | 0.276307     | 9.42125    | 0.42236       | 8.93              | 9              | 0.623859     | 2    |
| T3   | bart-large-cnn         | 0.276517     | 4.722928   | 0.382609      | 8.04              | 6.4            | 0.377811     | 3    |
|      | t5-tokenizer           | 0.25816      | 8.603267   | 0.339623      | 6.96              | 5.3            | 0.184273     | 4    |
|      | **distilbart-cnn**         | **0.319088**     | **8.377093**   | **0.548148**      | **9.53**              | **8.6**            | **0.815727**     | **1**    |
|      | bart-large-cnn-samsum  | 0.339106     | 8.723413   | 0.5           | 8.16              | 6.9            | 0.786701     | 2    |
| T4   | bart-large-cnn         | 0.213962     | 6.269622   | 0.382609      | 12.76             | 11.2           | 0.33236      | 3    |
|      | t5-tokenizer           | 0.197389     | 4.812779   | 0.344371      | 12.71             | 10.1           | 0.193254     | 4    |
|      | **distilbart-cnn**         | **0.258962**     | **10.62101**   | **0.405263**      | **15.64**             | **13**            | **0.806214**     | **1**    |
|      | bart-large-cnn-samsum  | 0.23072      | 6.194225   | 0.388489      | 12.7              | 10.1           | 0.359992     | 2    |
| T5   | **bart-large-cnn**         | **0.306693**     | **11.89793**   | **0.440945**      | **17.42**             | **15.2**           | **0.804081**     | **1**    |
|      | t5-tokenizer           | 0.167642     | 2.737621   | 0.276423      | 12.06             | 8.1            | 0.205876     | 4    |
|      | distilbart-cnn         | 0.258711     | 10.58902   | 0.370968      | 17.81             | 15.9           | 0.678493     | 2    |
|      | bart-large-cnn-samsum  | 0.259262     | 9.071449   | 0.390244      | 17.03             | 14.7           | 0.645121     | 3    |


### Finance Domain
Financial texts require precise information retention while maintaining clarity. The models were tested on their ability to summarize financial content while ensuring readability and comprehensibility.

**Results for the Finance domain are as follows:**

| Text | Model                  | Meteor Score | Bleu Score | Rouge-1 Score | Gunning-Fog Index | Flesch-Kincaid | Topsis Score | Rank |
|------|------------------------|--------------|------------|---------------|-------------------|----------------|--------------|------|
| T1   | **bart-large-cnn**         | **0.293193**     | **7.055251**   | **0.485294**      | **6.34**              | **3.5**            | **0.678353**     | **1**    |
|      | t5-tokenizer           | 0.174592     | 2.674008   | 0.40678       | 2.92              | 0.2            | 0.368849     | 3    |
|      | distilbart-cnn         | 0.271717     | 6.749952   | 0.517986      | 6.37              | 3.6            | 0.676931     | 2    |
|      | bart-large-cnn-samsum  | 0.154811     | 0.855283   | 0.336449      | 2.12              | -0.6           | 0.318764     | 4    |
| T2   | bart-large-cnn         | 0.23023      | 4.410798   | 0.363636      | 12.7              | 11.3           | 0.095448     | 4    |
|      | t5-tokenizer           | 0.253857     | 10.6098    | 0.465517      | 12.68             | 10.2           | 0.577074     | 3    |
|      | distilbart-cnn         | 0.315713     | 9.909893   | 0.430233      | 10.9              | 11.5           | 0.639987     | 2    |
|      | **bart-large-cnn-samsum**  | **0.32839**      | **13.21044**   | **0.533333**      | **12.38**             | **9.5**            | **0.85842**      | **1**    |
| T3   | bart-large-cnn         | 0.293195     | 10.17423   | 0.439024      | 10.43             | 9.0            | 0.624318     | 2    |
|      | t5-tokenizer           | 0.243504     | 3.827232   | 0.265035      | 15.43             | 13.8           | 0.189397     | 3    |
|      | **distilbart-cnn**         | **0.382304**     | **11.36201**   | **0.530225**      | **11.3**              | **8.0**            | **0.833238**     | **1**    |
|      | bart-large-cnn-samsum  | 0.262045     | 5.20148    | 0.392253      | 15.46             | 10.1           | 0.165373     | 4    |
| T4   | bart-large-cnn         | 0.168797     | 8.326541   | 0.384         | 13.69             | 10.3           | 0.537334     | 3    |
|      | t5-tokenizer           | 0.233936     | 3.516025   | 0.405797      | 11.47             | 11.5           | 0.395717     | 4    |
|      | distilbart-cnn         | 0.17281      | 8.765274   | 0.34638       | 14.26             | 11.0           | 0.567832     | 2    |
|      | **bart-large-cnn-samsum**  | **0.253493**     | **6.67748**    | **0.442623**      | **14.1**              | **8.8**            | **0.644549**     | **1**    |
| T5   | bart-large-cnn         | 0.225558     | 7.580675   | 0.346457      | 16.48             | 13.1           | 0.502433     | 3    |
|      | t5-tokenizer           | 0.268104     | 0.602068   | 0.184684      | 8.03              | 7.5            | 0.234006     | 4    |
|      | distilbart-cnn         | 0.294145     | 12.62863   | 0.428571      | 17.51             | 15.4           | 0.634264     | 2    |
|      | **bart-large-cnn-samsum**  | **0.294157**     | **18.25583**   | **0.48227**       | **11.73**             | **9.9**            | **0.84506**      | **1**    |


## Final Results
Based on the TOPSIS evaluation, the best-performing models for each domain were identified, providing insights into their respective strengths in different text domains.

**Final Results are as follows:**

| Text Domain | Best Model(s)                          |
|-------------|----------------------------------------|
| Health      | t5-tokenizer, bart-large-cnn-samsum    |
| Politics    | bart-large-cnn, bart-large-cnn-samsum  |
| Sports      | distilbart-cnn, bart-large-cnn-samsum  |
| Technology  | bart-large-cnn, distilbart-cnn         |
| Finance     | bart-large-cnn-samsum                  |

This evaluation provides insights into the performance of different summarization models across various domains, helping in selecting the most suitable model for a given task.

