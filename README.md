[![Build Status](https://dev.azure.com/cloud5mins/AzUnzipEverything/_apis/build/status/FBoucher.AzUnzipEverything?branchName=original)](https://dev.azure.com/cloud5mins/AzUnzipEverything/_build/latest?definitionId=23&branchName=master)

[![Deploy to Azure](https://img.shields.io/badge/Deploy%20To-Azure-blue?logo=microsoft-azure)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2sirmyron%2FAzUnzipEverything%2Foriginal%2Fdeployment%2FdeployAzure.json?WT.mc_id=azure-function-unzip)

# AzUnzipEverything

A simple Azure Function to Unzip files from a blob storage to another one

This current version only supports ".zip"

## How to deploy

To deploy all the resources in your Azure subscription, just click on the **Deploy to Azure** button

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsirmyron%2FAzUnzipEverything%2Foriginal%2Fdeployment%2FdeployAzure.json?WT.mc_id=azure-function-unzip" target="_blank"><img src="https://azuredeploy.net/deploybutton.png"/></a>

Fill-up the form and voila! It will be automatically deployed in your Azure subscription. If you don't own an Azure subscription already, you can create your **free** account today. It comes with 200$ credit, so you can experience almost everything without spending a dime. 
[Create your free Azure account today](https://azure.microsoft.com/en-us/free?WT.mc_id=tohack-github-frbouche)

Learn more on [how to deploy you Azure Function automatically or using the Azure Resource Manager (ARM) template](https://docs.microsoft.com/en-us/azure/azure-functions/functions-infrastructure-as-code?WT.mc_id=cloud5mins-github-frbouche)

![CreationForm][CreationForm]

## How to use it.

You can upload files to an Azure Blob storage using many different tool and code, but for this quick introduction let's use the Azure Portal.

Once [deployed](https://github.com/FBoucher/AzUnzipEverything#how-to-deploy), open the Azure portal [portal.azure.com](https://portal.azure.com?WT.mc_id=cloud5mins-youtube-frbouche)

1. navigate the resource Group you just deployed (ex: demoAzUnzipEverything).

    ![resourceGroup][resourceGroup]

1. Select the **Storage Account** that starts by "dropzone".
1. Click on **Blobs**, in the middle of the screen.
1. Click on the **input-files**. 
1. Click on the Upload button, and you can now upload a zip file.

    ![uploadFile][uploadFile]

1. After a few second the files you be Unzipped into the blob storage **output-files**.


## Continuous Integration (CI)

As you can see by the status badge [![Build Status](https://dev.azure.com/cloud5mins/AzUnzipEverything/_apis/build/status/FBoucher.AzUnzipEverything?branchName=master)](https://dev.azure.com/cloud5mins/AzUnzipEverything/_build/latest?definitionId=23&branchName=master) at the top of the page this project is automatically build at every push. 

Have a look, the [Azure DevOps](https://dev.azure.com/cloud5mins/AzUnzipEverything/) project is **public**! 


### Create a Continuous Integration, Continuous Deployment (CI-CD) for your Azure Function

In this video, I show you how to write an Azure Resource Manager (#ARM) template to deploy automatically your serverless Azure Function to Azure. It can be then used with a "Deploy to Azure" button from GitHub or any website, or in an Azure Pipeline to complete a Continuous Integration, Continuous Deployment (CI-CD) solution.

[![FunctionCICD][FunctionCICD]](https://www.youtube.com/watch?v=GRztpy337kU)


There is also a **written version** if you prefer reading: http://www.frankysnotes.com/2019/07/four-ways-to-deploy-your-azure-function.html



## TODOs

A GitKraken [Glo board](https://app.gitkraken.com/glo/board/XRYx_9FgZwAVbri7) is also available.

- [ ] Add Support for .rar
- [X] Add ARM template
- [X] Add a Deploy to Azure button

## More details

I have a [blob post](https://www.frankysnotes.com/2019/02/how-to-unzip-automatically-your-files.html) about this Azure Function. 

I also have a video where I build and test the function.

[![Auto-UnzipFunction_YT][Auto-UnzipFunction_YT]](https://www.youtube.com/watch?v=GRztpy337kU)
  

I also have an extended version where I introduce more the Visual Studio Extension to work with Azure Function. And explain more details about the Azure Function V2.

[![AzureFunctionWithVSCode_YT][AzureFunctionWithVSCode_YT]](https://www.youtube.com/watch?v=t9PvXWEzU-o)


## Contributing

Want to contribute? Check out our [Code of Conduct](CODE_OF_CONDUCT.md) and [Contributing](CONTRIBUTING.md) docs. This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.  Contributions of any kind welcome!

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):


[CreationForm]: /medias/CreationForm.png "Creation Form"
[resourceGroup]: /medias/resourceGroup.png "Select the ResourceGroup"
[uploadFile]: /medias/uploadFile.png "Upload Zip file"
[FunctionCICD]: /medias/AzureFunctionCICD_YT.png "YouTube thumbnail"
[Auto-UnzipFunction_YT]: /medias/Auto-UnzipFunction_YT.png "YouTube thumbnail"
[AzureFunctionWithVSCode_YT]: /medias/AzureFunctionWithVSCode_YT.png "YouTube thumbnail"


<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="http://cloud5mins.com"><img src="https://avatars3.githubusercontent.com/u/2404846?v=4" width="100px;" alt="Frank Boucher"/><br /><sub><b>Frank Boucher</b></sub></a><br /><a href="https://github.com/FBoucher/AzUnzipEverything/commits?author=fboucher" title="Code">💻</a> <a href="#video-fboucher" title="Videos">📹</a> <a href="https://github.com/FBoucher/AzUnzipEverything/commits?author=fboucher" title="Documentation">📖</a></td>
  </tr>
</table>

<!-- ALL-CONTRIBUTORS-LIST:END -->
