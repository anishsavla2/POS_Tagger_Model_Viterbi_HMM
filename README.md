English Parts-of-Speech (POS) Tagger with HMM

Problem:

I've built a POS tagger for English using a Hidden Markov Model (HMM). POS are represented by tagging each word, such as The/DT Santa/NNP Cruz/NNP.

Dataset:

WSJ part of the Penn Treebank dataset:
Train: Sections 00-18 (51,681 sentences).
Dev: Sections 19-21 (7,863 sentences).
Test: Sections 22-24 (9,046 sentences).
The tagset consists of 36 tags (45, including punctuation).

Components:

Hidden Markov Model:

I implemented a bigram HMM with add-α smoothing.
Included 〈START〉 and 〈STOP〉 tokens.
Constructed transition and emission tables.

Viterbi Decoding:

Decoding using Viterbi to find the best tag sequence.
Utilized add-α smoothing, with α = 1.
Implemented a baseline tagger that assigns the most frequent tag seen in the training set.

Debugging:

For initial debugging, I trained and tested on a single example to ensure proper labeling.


