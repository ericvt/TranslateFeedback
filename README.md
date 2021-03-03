<span align="center">
<a href="https://opensource.org/licenses/MIT"><img title="license" src="https://img.shields.io/badge/License-MIT-yellow.svg" ></a>
</span>

# Overview

translateFeedback is a python script that parses strings in a column of a spreadsheet, send them to Azure Translator API and store the translation back in another column in the spreadsheet.

## Standalone use

You can pull down the [translateFeedback.py](https://github.com/ericvt/feedback_autotranslate/blob/master/script/translateFeedback.py) module directly and execute it in python environment, or pull the translateFeedback folder directly
It uses Python 3.x and you'll need openpyxl, requests, uuid modules to be installed.

You may also pull TranslateFeedback package from [https://pypi.org/project/TransFeedback/1.2.0/](https://)
and run it into a virtual environment.

## Usage

```bash
python3 translateFeedback.py {spreadsheet} {Column number to translate from} {Column number to translate to} {source language} {target language} {subscription key}
```

or

```bash
python3 translatefedback {spreadsheet} {Column number to translate from} {Column number to translate to} {source language} {target language} {subscription key}
```

* note: the source language and target language code must be compliant with the Translation API language code, see [https://docs.microsoft.com/en-us/azure/cognitive-services/translator/language-support](https://docs.microsoft.com/en-us/azure/cognitive-services/translator/language-support)
