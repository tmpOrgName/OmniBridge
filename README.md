[![codecov](https://codecov.io/gh/OmniSpective/OmniBridge/branch/main/graph/badge.svg)](https://codecov.io/gh/OmniSpective/OmniBridge)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/OmniSpective/OmniBridge/tests.yml)
![PyPI - License](https://img.shields.io/pypi/l/omnibridge)
![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/OmniSpective/OmniBridge)
![PyPI - Downloads](https://img.shields.io/pypi/dd/omnibridge?style=plastic)

# OmniBridge

OmniBridge is a CLI tool that bridges between different AI models. It helps you can access different AI models in a centralized place.

# Install

```
> pip install omnibridge
```

# Usage

Available in CLI with the following arguments:

* -m / --model
* -p / --prompt
* -l / --load-config

single model example:
```
python main.py -m chatgpt -p hello
```

multi model example:
```
python main.py -m chatgpt -p hello -m dalle -p goodbye
```

Note that the order of specification matters, meaning that in the above example, chatgpt will get the prompt `hello` and dalle will get the prompt `goodbye`

The configurations can be set in a .json file and given to the CLI tool with the flag `-l <PATH_TO_CONFIG_FILE>`.

For example:

```
{
    "chatgpt": {
        "api_key": "...",
        "model": "..."
    },
    "hugging_face": {
        "api_key": "...",
        "model_id": "..."
    },
    "dalle": {
        "api_key": "...",
        "num_of_images": ...,
        "resolution": "..."
    }
}
```


# Community 
<a href="https://discord.gg/RjPHfAKd7D"><img src="https://assets-global.website-files.com/6257adef93867e50d84d30e2/636e0a69f118df70ad7828d4_icon_clyde_blurple_RGB.svg" alt="Discord Icon" width="40" height="20"></a>
Join our <a href=https://discord.gg/RjPHfAKd7D>discord server</a>  and share your feedback and ideas with us! 


# Contribute:

Join us in shaping the future of A.I!<br/>
For information on how to contribute, see [here](.github/CONTRIBUTING.md).



