# README

### SWAG / CommonsenseQA Multiple choice model with BERT

* usage:

  `python swag_bert_baseline.py `

  `python csQA_bert_baseline.py`

  

* optional parameter arguments:

  `--data_dir`   input data directory (should contain the `train.scv` and `val.csv` )

  `--output_dir`   directory for saving the BERT configurations the model weights, and the evaluation results

  `--bert_model`   can be a string in the following: `bert-base-uncased`, `bert-large-uncased`, `bert-base-cased`, and `bert-base-cased` 

  `--max_seq_length`  the maximum total input sequence length after tokenization. Sequences longer than it will be truncated

  `--do_train`   Boolean for whether to run the training steps

  `--do_eval`   Boolean for whether to run the evaluation on val set

  `--train_batch_size` Default is 16

  `--eval_batch_size` Default is 16

  `--learning_rate` 

  `--num_train_epochs ` number of training epochs. Default is 3

  `--seed` random seed

### Evaluation results

#### SWAG

##### 	Hyperparameters

	* batch size: 8
	* BERT model: base, uncased
	* maximum sequence length: 100
	* training epochs: 3

##### Results

Dev set accuracy: 0.755

(Test set has no ground truth label)



#### CommonsenseQA

##### 	Hyperparameters

- batch size: 16
- BERT model: base, uncased
- maximum sequence length: 128
- training epochs: 4

##### Results

Dev set accuracy: 0.5348 (BERTBase implementation by University College London: 0.530)

(Test set has no ground truth label)