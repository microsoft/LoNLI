# LoNLI v1.0

We release CheckList-based behavioral testsuite *LoNLI* dataset associated with [Trusting RoBERTa over BERT: Insights from CheckListing the Natural Language Inference Task
](https://arxiv.org/abs/2107.07229). We create a semi-synthetic large test-bench (363 templates, 363k examples) and an associated framework that offers following utilities: 
1) individually test and analyze reasoning capabilities along 17 reasoning dimensions (including pragmatic reasoning), 
2) design experiments to study cross-capability information content (leave one out or bring one in); and 
3) the synthetic nature enable us to control for artifacts and biases.
![Alt text](Otherdatasets.png?raw=true "LoNLI against the spectrum of (a subset of) NLI datasets")

## Files

1. `data_v2.zip` - Unzip it to find 363 files. Each files is named with the corresponding capability (borrowed from [TaxiNLI](https://github.com/microsoft/TaxiNLI)).
   - For example `boolean_1.tsv` contains the examples form `boolean_1` template (found in `templates.ipynb`). 
   - Each file contains three columns "premise", "hypothesis" and "label"
2. `templates.ipynb` - The python notebook is a single-stop shop for creating data for all templates. It uses the `lexicon.py`
   - To run the notebook and install necessary requirements, please follow the guidelines in the [CheckList](https://github.com/marcotcr/checklist) repository.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
