# Talk to your data with RTutor

RTutor is an AI-based Shiny App that can quickly generate and test R code. Powered by API calls to OpenAI, natural languages are translated into R scripts, which are then executed within the Shiny platform. An R Markdown source file and HTML report can be generated. 

## Installation
``` r
library(remotes)
install_github("gexijin/RTutor")
```

## Obtain an API key from OpenAI
1.  Create a personal account at [OpenAI](https://openai.com/api/).
2.  After logging in, click on **Personal** from top left.
3.  Click **Manage Account** and then **Billing**, where you can add **Payment methods** and set **Usage limits**. $3-$5 per month is more than enough for most people.
4. Click on **API keys** to create a new key, which can be copied.

## Use the API key with RTutor
There are several ways to do this. 
- After the app is started, you can click on **Settings** and paste the API key.
- You can also save this key as a text file called **api_key.txt** in the working directory. 
- Finally, you can create an environment variable called **OPEN_API_KEY**. Instructions for [Windows](https://docs.oracle.com/en/database/oracle/machine-learning/oml4r/1.5.1/oread/creating-and-modifying-environment-variables-on-windows.html), 
[Mac](https://phoenixnap.com/kb/set-environment-variable-mac), and 
[Linux](https://linuxize.com/post/how-to-set-and-list-environment-variables-in-linux/). 

## To start RTutor
```{r example}
library(RTutor)
run_app()
```
