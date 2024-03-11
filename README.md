# Semantic Kernel Demo

This repo contains a .NET Interactive notebook showing some features of [Semantic Kernel](https://learn.microsoft.com/en-us/semantic-kernel/overview/).
To work with the notebook, you need to install the [Polyglot Notebooks](https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.dotnet-interactive-vscode) extension in VS Code.

The notebook `1-AI-kernel.ipynb` shows using the kernel: 
- with plugins, declaring .NET native and semantic functions
- for generating images using an Azure OpenAI DALL-E model
- leveraging Planner to create & execute a plan, incl. using different plugins

## Configuration
To configure your environment, open the notebook `0-AI-settings.ipynb` and follow the steps. This will create a `config/settings.json` file in your project with all required settings & secrets. 

If you want to test the EmailPlugin in the Planner section, you need to create a `config/email_endpoint.txt` file containing the endpoint URL of a Logic App workflow. 
The workflow should look like this:

<img src="https://github.com/cplemm/SemanticKernelDemo/blob/f9576e196b33a53b8c686885ddca1cea0e9ebee4/EmailWorkflow.png" width="50%" >
