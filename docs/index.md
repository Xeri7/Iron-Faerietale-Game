---
layout: home
---


<p style="margin-bottom: -20px"> 
    <img src="assets/images/HubWorldMMOLogo01.png" alt="HubWorldMMO" width="400">
    <h4>
        <a href="http://www.sabredartstudios.com/">By SabreDartStudios</a>
    </h4>
</p>

<p>
    <a href="https://github.com/SabreDartStudios/HubWorldMMO/blob/master/LICENSE">
        <img src="https://img.shields.io/github/license/SabreDartStudios/HubWorldMMO.svg?style=flat-square">
    </a>
    <a href="https://discord.gg/qZ76Cmxcgp">
        <img src="https://img.shields.io/badge/Discord-%237289DA.svg?style=flat-square&logo=discord&logoColor=white" alt="Join Discord">
    </a>
    <img src="https://img.shields.io/badge/unrealengine-%23313131.svg?style=flat-square&logo=unrealengine&logoColor=white">
    <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white">
    <img src="https://img.shields.io/badge/.NET-5C2D91?style=flat-square&logo=.net&logoColor=white">
</p>

---

## What is Hub World MMO?

<iframe width="100%" height="410" src="https://www.youtube.com/embed/tW-dclaNAmA" title="Hub World MMO - Introduction" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Setup Instructions

1. Install OWS 2 by following the [Setup Instructions](https://www.openworldserver.com/getting-started/) up to the point of getting your API key.  Once you have your API key, you can continue with setting up the Hub World MMO example project.
2. Fork the [Hub World MMO project](https://github.com/SabreDartStudios/HubWorldMMO) to your own GitHub.  This is a VERY important step if you intend to make modifications.
3. Once you have your own fork of the Hub World MMO project on your GitHub, then you can open Visual Studio 2022 and Clone it.
4. After it downloads all of the files, open Config/DefaultGame.ini and put your API key in the OWSAPICustomerKey and save the file.
5. Open OWSInstanceLauncher/appsettings.json and put your API key in OWSAPIKey.  You also need to set PathToDedicatedServer to point to your Unreal Engine 5 editor and set PathToUProject to point to the OWSHubWorldMMO.uproject file.
6. Open your database management client and connect to the OpenWorldServer database using the instructions from the OWS 2 setup.  Open the Initialize.sql script in the SQL folder based on the DB technology and client type you are using.  Add your API key to the top line of the SQL script, then run it.
7. Download the [Project Content Zip File - 20240727](https://drive.google.com/file/d/186PIAowKN72a2So4zvGb37vpaTLM2q4P/view?usp=sharing) (3.5 GB) and copy the files into your Content folder.
8. Right click on the OWSHubWorldMMO.uproject file and click on "Generate project files..."
9. Open the OWS 2 project in Visual Studio 2022 and press docker-compose.  Give it a minute or two to fully start up.  You must repeat this step whenever you want to develop with the Hub World MMO project.  "docker-compose" MUST stay running in Visual Studio 2022 the entire time.
10. Open OWSHubWorldMMO.sln in a second copy of Visual Studio 2022 and press the green play button.

## Setup Instructions Video

<iframe width="100%" height="410" src="https://www.youtube.com/embed/21q3IvkFLnw" title="Hub World MMO - How to Install" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## _HWAssets Update

If you don't need the Megascans and MSPresets folders which don't change often, you can use the following link to get the latest _HWAssets folder changes (updated 7/27/2024).

[_HWAssets Folder](https://drive.google.com/file/d/1QJinbLTyzgP2BkXqHY6XPWD2ab4xtHO2/view?usp=sharing) 562 MB
