# Generative Pre-Trained Transformer (GPT)

GPT models consist of stacked transformer decoder blocks. The model is trained to predict the next word given the preceding words.

Here, I have implemented a character-level GPT model (predicts the next character given the preceding characters). Initially the characters are encoded using embeddings and then positional encodings are added. This data is passed into a series of decoder blocks. Finally, this is passed into a linear layer and the softmax function is applied to produce a probability distribution for the next character is. This distribution can then be sampled from. The process is repeated to produce text.

I have trained the model on a dataset consisting of texts written by Shakespeare. The model achieves a loss of roughly 1.6 on the training set and 1.7 on the test set.

The model produced the following text:

```
COMANTIS:
Why phipest one dread,-for Edward:
Can all world of laites it by I know she will have wrong whortlams
art wreting whom to guids, ortain I'll quee's him
ISABELLA: a here in has jiers,
Scome, hath her eart, poil'd flowers tongue all,
Your so, quah; can all I hope of Bodward,
What I thee see of TEthonoube, last,
Even the pluck of I say were heavensalis!
By not more accal. Romeo dread, mood have the common,
Hadlian of was powers vassion being.

SICHAS Lews War I have appect, and hath repenate!
But we now rich be call'd dost this was the is disposes
All I could is for his your hear smist good
My busice, I there is strim his I speak of love pitter,
Which fright had give meme have pieversing:
Let my yourself on base, my peaceful wither of
Howld; the hope this should will walk I saw'll
With so poveage.

CORIOLANUS:
Socis the grace; mutimer, what gover, I'lco
Eve a delaze third faces the eighamer remies.
Do Nighmost to doth Mowe all meghore give
The give return of Leggerand by of Yea 
```

Although though not perfect, the model is still quite impressive and could be improved with tuning of the hyperparameters.
