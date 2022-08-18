# Language Translation using Deep Learning

In this project, we build a deep neural network that functions as part of a machine translation pipeline. The pipeline accepts English text as input and returns the French translation. The goal is to achieve the highest translation accuracy possible.

## Approach
To translate a corpus of English text to French, we need to build a recurrent neural network (RNN). Before diving into the implementation, let's first build some intuition of RNNs and why they're useful for NLP tasks.

### Building the Pipeline
Below is a summary of the various preprocessing and modeling steps. The high-level steps include:

1. **Preprocessing**: load and examine data, cleaning, tokenization, padding
1. **Modeling**: build, train, and test the model
1. **Prediction**: generate specific translations of English to French, and compare the output translations to the ground truth translations
1. **Iteration**: iterate on the model, experimenting with different architectures

For a more detailed walkthrough including the source code, check out the Jupyter notebook in the main directory.

### Toolset
We use Keras for the frontend and TensorFlow for the backend in this project. I prefer using Keras on top of TensorFlow because the syntax is simpler, which makes building the model layers more intuitive. However, there is a trade-off with Keras as you lose the ability to do fine-grained customizations. But this won't affect the models we're building in this project.

## Results
The results from the final model can be found in cell 20 of the [notebook](machine_translation.ipynb).

Validation accuracy: 97.5%

Training time: 23 epochs
