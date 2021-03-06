# This package contains metric functions and DataFrame handling modules

## Installation

install the development version from GitHub:

```bash
pip install git+https://github.com/Analyse/AnalysePredict
```
## Accompanying packages

import numpy as np

import pandas as pd

## Usage

```python
>>> from Analyse.AnalysePredict import A_Predict_module as ap #This module has all seven functions
>>> ap.dictionary_of_metrics([1, 2, 3, 4, 5])
{'mean': 3.0, 'median': 3.0, 'variance': 2.5, 'standard deviation': 1.58, 'min': 1.0, 'max': 5.0}

>>> ap.five_num_summary([1, 2, 3, 4, 5])
{'max': 5.0, 'median': 3.0, 'min': 1.0, 'q1': 1.5, 'q3': 4.5}

or

>>>from Analyse.AnalysePredict import dictionary_of_metrics as dm  #This option imports only one function module
>>>dm.dictionary_of_metrics([1, 2, 3, 4, 5])
{'mean': 3.0, 'median': 3.0, 'variance': 2.5, 'standard deviation': 1.58, 'min': 1.0, 'max': 5.0}
```

The code adheres to [PEP8] guidelines.

[PEP8]: https://www.python.org/dev/peps/pep-0008/ "PEP 8 -- Style Guide for Python Code"

## Functions and examples

### Descriptive statistics and measure of variability

| Function                           | Example                                                                  |
|------------------------------------|--------------------------------------------------------------------------|
| [dictionary of metrics]            | `dictionary_of_metrics([1, 2, 3, 4, 5])`                                 |
| [five_num summ]                    | `five_num_summ([1, 2, 3, 4, 5])`                                         |
| [data parser]                      | `data_parser(["2019-11-29 12:50:54"])`                                   |
| [stop_words_remover]               | `stop_words_remover(twitter_df.copy()).loc[42, "Without Stop Words"]`    |                        | [word_splitter]                    | `word_splitter(twitter_df.copy()).loc[37, "Split Tweets"]`               |
| [number_of_tweets_per_day]         | `number_of_tweets_per_day(twitter_df.copy()).loc['2019-11-22','Tweets']  |
| [extract_municipality_hashtags]    | `extract_municipality_hashtags(df)`                                      |


## Spirit and rules

- Everything should be implemented in raw, organic, locally sourced Python.
- Use libraries only if you have to and only when unrelated to the math/statistics. For example, `from functools import reduce` to make `reduce` available for those using python3. That's okay, because it's about making Python work and not about making the stats easier.
- It's okay to use operators and functions if they correspond to regular calculator buttons. 
Anything beyond that, like `mean`, `median`, we have to write ourselves.

Pull requests are welcome!

## Contributors

- Marcus Moeng :https://github.com/marcusmoeng
- Akhona Stefane :https://github.com/Akhona-Stafane/Analyse
- Lawrence Hlapa :https://github.com/LawrenceHlapa/Analyse
- Mpho Marufu  :https://github.com/Mpho-Marufu
- Pennelope Makhosazane :https://github.com/makhosazane89

