# Web3Eval

Web3Eval is a tool for repeatedly running a set of pre-defined Web2 and Web3 tasks in a setting with tightly-controlled initial conditions. With each run, Web3Eval will start from a blank slate. The agents being evaluated will need to solve tasks. All runs are conducted in freshly-initialized docker containers or natively.

## Requirements

### Build

Web3Eval can be built from source code using `pip install -e .`.

After installation, you must configure your API keys. Web3Eval will look for the OpenAI keys from the `ENV.json` file in the current working directory. An example `ENV.json` file is provided below:

```
{
    "OPENAI_API_KEY": "sk-",
    "OPENAI_API_BASE": "https://",
    "AZURE_OPENAI_AD_TOKEN": ""
}
```

### Docker

Web3Eval requires Docker (Desktop or Engine). To install Docker Desktop see [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/).

### Init WebArena Tasks

Navigate to the `webarena` directory and run the following command:

```
python Script/init_tasks.py
```




## Web Arena

### Overview
http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:4399 

### Environment Variables
```
export SHOPPING="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:7770"
export SHOPPING_ADMIN="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:7780/admin"
export REDDIT="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:9999"
export GITLAB="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:8023"
export MAP="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:3000"
export WIKIPEDIA="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:8888/wikipedia_en_all_maxi_2022-05/A/User:The_other_Kiwix_guy/Landing"
export HOMEPAGE="http://ec2-15-168-175-171.ap-northeast-3.compute.amazonaws.com:4399"
```
