# sn-togetherai
ServiceNow flow action and subflow that can be used to test together.ai models.

## Together AI - Run AI with an API

1. [https://together.ai](https://www.together.ai/)
2. Sign in with Github
3. Get your API key - [https://api.together.xyz/settings/api-keys](https://api.together.xyz/settings/api-keys)

Together.ai provides $5.00 worth of free credits for each account, and I've found with their optimizations discussed [here](https://www.together.ai/blog/together-inference-engine-v1), this is a decent amount of credits to get started with.

## ServiceNow

1. Import from source control in Studio.
2. Open Together.ai app in Studio and select the system property.
3. Put in your Together AI API key and save it.
4. Open the subflow and click test.
5. Enter a model and prompt. Note: The list of models can be found at [https://api.together.xyz/models](https://api.together.xyz/models) and you will need to enter the full model string including author and model name. (The default in subflow is meta-llama/Meta-Llama-3.1-405B-Instruct-Turbo)
6. Have fun 😁!
   
## Usecase

Since ServiceNow's Now Assist product is unavailable in PDIs, this allows for testing of GenAI responses using together.ai's library of serverless endpoint models. The subflow could even be modified and utilized in a production Flow if together.ai is allowed in your organization.

## Future plans

* Ability to support image generation / storage of the returned image in ServiceNow.
* TBD
