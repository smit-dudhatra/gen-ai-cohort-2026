there are 2 levels of AI Engineering:-

1) Fundamentals OF AI:-
   how LLM is trained and work
2) application Of AI:-
  how one can integrate the LLM in real world use cases and fine tune with the exact client requirements

what is GPT ?
GPT stands for Generative Pre-trained Transformer
it is ultimately a LLM.

A transformer which is pre-trained and generates the output

user Input -> [GPT] -> Output (Next Predcition Token)

claude , gemini all are GPTs

Generative:-

things are not in DB, we will generate things on the go.

Pre-trained:-

trained on pre-existing training data

Transformer:-

The Whole Engine

Every LLM has its own vocabulary to translate the user input

Step 1:-
Tokenize the input (means convert the user input in it's own language)

[https://gptforwork.com/tools/tokenizer](url)

check this website

input your text and see how the input gets tokenized

it's not necessary that the each and every token has it's token id
sometimes most used words get fully tokenized 

this is useful to shrink the vocabulary

step 2:-
vector embeddings

plot the related token in 3D Plane (X,Y,Z)

[https://projector.tensorflow.org/](url)

step 3:-

Positional Encoding

vector embeddings + position data (what is the vecotr distance between two tokens)

Piyush loves [x]
[x] loves Piyush

same vector embeddings but position data is different


self attention mechanism / single head attention mechanism:-

in this , tokens talks to each other and determine which ones are mose relevant to each other 
they try to find context-aware meanings

River [Bank] and HDFC [Bank]

softmax == LLM temprature

What probability level do you want for the output?
(ketli probability walu output joiye che ?)

Inferencing is the act or process of reaching a logical conclusion based on evidence, observations, and background knowledge.

Cross Enthropy Loss -> difference between two plausible (rational/logical) outcome

example

suppose
2 + 2 = 99 - it's too far --> model back propogation
2 + 2 = 15 - bit far ->> model back propogation
2 + 2 = 5 - just 1 away ->> model back propogation
2 + 2 = 4 -> Exact match

there is no back propogation in inferencing
while model is giving answer to you , it is inferencing you are not doing model back propogation

inferencing is for pre-trained model

during model training weights are updated via model back propogation
