# makemore-tr

The `makemore-tr` project's aim is to mimic the style and structure of authentic Turkish names with a deep learning model.
The structure of the model is based on following paper [A Neural Probabilistic Language Model, 'Bengio et al. 2003'](https://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf).

Also Andrej Karpathy's youtube video ['Building makemore Part 2: MLP'](https://www.youtube.com/watch?v=TCH_1BHY58I&list=PLAqhIrjkxbuWI23v9cThsA9GvCAUhRvKZ&index=3&ab_channel=AndrejKarpathy)  influences and teaches me a lot on this project. 

Lastly, thanks to Kamil Toraman for the [raw data](https://gist.github.com/kvtoraman/f300ae077828c6940d96cd3b19181b3f).

The project involves three main notebooks:

1. **Data Cleaning Notebook (`data-cleaning.ipynb`)**: This notebook is responsible for cleaning the dataset of Turkish names. It removes duplicates, unwanted characters, and prepares a list of cleaned names.

2. **Model Training Notebook (`makemore-tr.ipynb`)**: This notebook builds a character-level language model using PyTorch. It sets up the vocabulary, creates datasets, and trains a neural network model to generate plausible Turkish names.

3. **Model Training Notebook with Manual Backpropagation (`manual_backprop_tr.ipynb`)**: In this notebook I done back propagation manually (without using loss.backward()) to gain hard level understanding of backpropagation and gradients. 

### Dependencies

Ensure you have the following libraries installed on your environment for proper execution of the notebooks:

- `torch`: For building and training the neural network model.
- `matplotlib`: For plotting and visualizing data during training.

### Example Outputs

To generate new Turkish names after training the model, simply execute the sampling cell in the `manual_backprop_tr` notebook. The model will output a list of new names based on the learned patterns. Sample output may include names like:

```

cant.
süze.
ergin.
topvar.
erk.
can.
say.
ker.
yıldıralp.
evi.
kara.
dorulhan.
gökmeter.
ağatarakan.
aslan.
serkoç.
nur.
tapdsel.
salkuşa.
yurdu.

```

These names are generated by the model and aim to mimic the style and structure of authentic Turkish names.