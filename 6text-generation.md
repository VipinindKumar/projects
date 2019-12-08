---
layout: post
title: Text Generation
description: Text generation from a Recurrent Neural Network trained on English translated version of "The Ramayana of Valmiki, translated by Hari Prasad Shastri" 
image: https://github.com/VipinindKumar/Neural-Style-Transfer/raw/master/images/galmton-taj/generated_image.jpg
nav-menu: true
---



### Text generation from a Recurrent Neural Network trained on English translated version of "The Ramayana of Valmiki, translated by Hari Prasad Shastri"


<hr/>


**Epoch 5/20**

2532/2532 [==============================] - 331s 131ms/step - loss: 1.1127

####################

Temperature: 0.2

####################

on of the 
sages, the titans and the powerful 
Ravana and the son of Dasaratha, who was able to disport the son of 
Dasaratha and the son of Dasaratha and the 
monkeys and the son of Dasaratha and 
the foremost of the Rakshasas and 
the son of Ravana's heart and the 
sun and the son of the Wind-god 

 of Dasaratha and 
the son of Vayu, the son of Dasaratha, 
who was subject to the sun and 
the son of Dasaratha and Shri Ramachandra and 
the son of the Gods, the King of the Monkeys, 
who was able to change the sun and 
the sun in the presence of the 
forest and the head of the powerful 
Ravana and

 and the son of Dasaratha and the 
sun and the son of Dasaratha and 
the son of Vasava, the King of the Monkeys, having set out from the sun and 
arrows and the son of the Wind-god 
and the titans with the army of the 
sun and the son of Dasaratha, the 
son of Dasaratha and having slain the 
monkeys


<hr/>




**Epoch 20/20**

2532/2532 [==============================] - 332s 131ms/step - loss: 0.9149

####################

Temperature: 1.0

####################

able to deep like a lion, made calamity bore the terror of his anger. Having accepted these words 
of Raghava, many deceiting flowering 
battle. On none hanging his instruction and great intellect with thy grief! It was formerly. Now 
Bharata and cross their lives four departure. The prowess of roya

icate tones, Manu whose boon 
must take heart, this is help to the titans in seas for shouting, lay possessed of 
himself with con-litulat ever 
bestowed on him; therefore, provoked youth and in 
words with joined palms, said :- 
cc This matter none were mine own abode. None were mastered with their

s, 
ascended a celestial partike, cut forth, whether he bears the scent 
of this toward and again, the aged titan among 
the sacrificial fires of my opposi- 
ity, would not listen, between the 
Goddess Poulastya and their leaders, in a 
brahmin of which I will destroy the kine 
and the third was fil


<hr/>


### Model, library and parameters used:

```python
textgen = textgenrnn(name='Ramayan RNN')

train_function = textgen.train_from_largetext_file

train_function(file_path='ram.txt',
              new_model=True,
              num_epochs=train_cfg['num_epochs'],
              gen_epochs=train_cfg['gen_epochs'],
              batch_size=1024,
              train_size=train_cfg['train_size'],
              validation=train_cfg['validation'],
              rnn_layers=model_cfg['rnn_layers'],
              rnn_size=model_cfg['rnn_size'],
              rnn_bidirectional=model_cfg['rnn_bidirectional'],
              max_length=model_cfg['max_length'],
              dim_embeddings=100)

```



```python
model_cfg = {'rnn_size': 128,
            'rnn_layers': 3,
            'rnn_bidirectional': True,
            'max_length': 30}

train_cfg = {'num_epochs': 20,
            'gen_epochs': 5,
            'train_size': 0.9,
            'validation': True}

```
