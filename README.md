# Analysis of thoughts during food decision making

How do we process and evaluate different aspects of a choice when we make decisions? How does self-control influence these processes? Previous studies suggest that we may 
sample from the previously encoded memories (Shalden & Shohamy, 2016) to build the evidence for our choices. Our previous work also suggest that self-control affects the temporal
pattern of processing choice attributes and constructing their values (HajiHosseini & Hutcherson, 2021). In this study, we asked what thoughts people remember when they make
food choices and whether these thoughts are affected by self-control. 

### Methods
We showed our participants pictures of food items and asked them to rate how much they wanted to eat that food. We also asked them to give at least one and at most four reasons for every choice they made. We also asked them to rate their preference for these foods before and after they completed their blocks of choices. We instructed some of these participants to choose naturally and some to focus on healthy eating when they made choices.

### Code
AnalyzeReasons_1.ipynb reads the original data and perfroms cleaning and pre-processing. Then it runs Topic Modeling using LDA from sklearn, clusters the thoughts into 3 topics and measure the overall semantic similarity of each topic cluster to the words "taste" and "health". We found that when participants chose naturally, their thought clusters were more similar to 'taste' and less similar to 'health' whereas when they focused on health, the similarity of their thought clusters to 'taste'/'health' decreased/increased respectively.

AnalyzeReasons_2.ipynb runs several regression models to analyze the influence of self control on people's thoughts, and the relationships between their thoughts, choices, and preferences.


For questions about data, please contact me hajihosseini@gmail.com

### References

Shadlen, M. N., & Shohamy, D. (2016). Decision making and sequential sampling from memory. Neuron, 90(5), 927–939. https://doi.org/10.1016/j.neuron.2016.04.036

Hajihosseini, A., & Hutcherson, C. A. (2021). Alpha oscillations and event-related potentials reflect distinct dynamics of attribute construction and evidence accumulation in dietary decision making. ELife, 10. https://doi.org/10.7554/ELIFE.60874
