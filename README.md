# The basic purpose of this project is understanding in depth how does NLP and specially Sentiment analysis works.
The project include 9 steps to complete the task
    # 1- Data Visualization to gain insights of data using:
                - Matplotlib
                - Seaborn
                - How many people gave 1,2..5 stars and what are their reviews(comments) about food(Positive, Negative or Neutral)
    # 2- Perform Sentence tokenization using NLTK
                - Every word will be separated
                - Such as ['I', 'like', 'apple', 'and', 'mango', 'es']
    # 3- We can check for Part-of-speech of this tokenized sentence
                - Part-of-speech will return as [('This', 'DT'), ('is', 'VBZ')] etc
                - It specifies either the word is noun, pronoun, verb etc
    # 4- Optionally we can create chunks of POS to make the above output more clear
                - The output will be like This/DT   is/VBZ etc
    # 5- Performing Sentiment analysis using VADER                                              1st Approach
                - It use Bag of words approach
                - Each word is scored and combined to a total score
    # 6- With VADER we can calculate the Polarity_Score                                          Very important
                - Calculate polarity_score of any sentence
                - The output will be like:
                      - pos: How much positive a sentence is?
                      - neu: How much neutral a sentence is?
                      - neg: How much negative a sentence is?
                      - compound: How much positive(+1) or negative(-1) a sentence is?
    # 7- We can perform same task with roberta model as well                                    Very good approach
                - A pretrained model on Transformers
                - Model used in this project is: "twitter_roberta_base_model" trained on twitter comments
                - same as VADER we can calculate Polarity Score using roberta                   2nd Approach
                - The output will be same as VADER but with really really good results
    # 8- We can compare the result of VADER and roberta and can see 
                - roberta is really really good
    # 9- A very quick and easy way to do sentiment analysis is by:
                - **Pretrained sentiment analysis
                - we can choose tokenization of out choice but builtin also works really good
