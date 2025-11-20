# long_context_relic

To run evaluation from the paper, use
`python scripts/eval_model_responses.py`

The evaluation script requires the `pandas` and `rapidfuzz` packages.

The 292 long context RELiC examples are in the `data/long_context_relic_acl.csv` file. The relevant column names are:

- `book_title`: Title of the primary source book
- `prefix`: Literary analysis preceding the primary source quotation
- `suffix`: Literary analysis following the primary source quotation
- `answer_quote_text`: Ground truth primary source quotation
- `answer_quote_idx`: idx of ground truth in the list of primary source sentences
- `num_sents`: Number of sentences in ground truth
- `close_reading_example`: TRUE if example is in the close reading fold
- `human_eval_set`: TRUE if example was attempted by a human