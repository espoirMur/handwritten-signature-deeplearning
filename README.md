# handwritten-signature-deep learning
Contains random ideas for a deep learning project about signature handwritten recognition

I had the ideas to start this project as a learning project for deep learning!

Will apply the method of deep learning to recognize signatures on a document.

But for now I still looking how to start:

the first step is to collect useful resources and check what is already done by others peoples.
here is what I have collected.

- [The first one ](https://www.google.rw/amp/s/gizmeon.com/2017/10/21/fraud-analysis-deep-learning-n-offline-signature-verification/amp/)
- [the second](https://github.com/luizgh/sigver_wiwd/blob/master/interactive_example.ipynb) a jupyter notebook with some work done.
- [the third one](http://aeop.asecamps.com/wp-content/uploads/2017/07/5.pdf)

Let me digest them and plan how this project will bde done.
[Another good paper](https://arxiv.org/pdf/1705.05787.pdf) 

Some keywords to explore :
-  **Writer-Dependent classifiers** :  _In this scenario, a training set is
constructed for each user of the system, consisting of genuine signatures as positive examples and
genuine signatures from other users (random forgeries) as negative samples. A binary classifier
is then trained on this dataset, resulting in one model for each user_
This approach has shown to work well for the task, but since it requires one model to be trained for each user, complexity
increases as more users are enrolled.

- **Writer-Independent classification:** _In this
case, a single model is trained for all users, by training a classifier in a dissimilarity space . The inputs for classification are dissimilarity vectors, that represent the difference between
the features of a query signature, and the features of a template signature (a genuine signature of
the user)._
In spite of the reduced complexity, Writer-Independent systems often perform worse,
and the best results in standard benchmarks are obtained with Writer-Dependent systems.

After reading [This ](https://arxiv.org/pdf/1705.05787.pdf) research paper I decide to use a writer dependent classifier for handwritten recognition.
for the first try I will train the data with the sinature from 10 person, and increase the dataset in the future.
the output of this work can be presented to organization such as banks , or others instutuition.

but some questions arise :
- how to collect data?
- how to build the dataset?

The resarch takes this approach : **_a Writer-Independent feature learning
phase followed by Writer-Dependent classification_**
