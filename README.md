<h1 align="center">
<a href="https://www.dlubal.com/en" title="Tutorial 1"><img src="./img/logo.png" width="180" height="180" alt="Dlubal Software" /></a>

Dlubal Software GmbH

[![image](https://img.shields.io/twitter/follow/dlubal_en?style=social)](https://twitter.com/dlubal_en "Twitter Follow")
[![image](https://img.shields.io/badge/GitHub-Dlubal_Software-darkblue?logo=github&amp;)](https://github.com/Dlubal-Software "Github Follow")
[![image](https://img.shields.io/badge/http://-dlubal.com-darkblue)](https://www.dlubal.com/en-US "RFEM Latest")
[![image](https://img.shields.io/badge/docs-API-darkblue?logo=read-the-docs&amp;logoColor=white)](https://dlubal-software.github.io/RFEM_Python_Client/ "RFEM Latest")

[![image](https://img.shields.io/badge/RFEM-v6.0-blue)](https://www.dlubal.com/en/products/rfem-fea-software/what-is-rfem "RFEM")
[![image](https://img.shields.io/badge/RSTAB-v9.0-blue)](https://www.dlubal.com/en/products/rstab-beam-structures/what-is-rstab "RFEM")
[![image](https://img.shields.io/badge/Python-3-blue?logo=python&amp;logoColor=yellow)](https://www.python.org/)
![image](https://img.shields.io/badge/coverage-87%25-green)

</h1>


<h2 align="center">

Welcome to RFEM Python API

<a href="https://www.dlubal.com/en/products/rfem-fea-software/what-is-rfem" title="Tutorial 1"><img src="./img/2Dtruss.gif" width=550 alt="Tutorial" /></a>
</h2>

Python client (high-level functions) for [RFEM 6](https://www.dlubal.com/en/products/rfem-fea-software/what-is-rfem) using [Web Services](https://en.wikipedia.org/wiki/Web_service) (WS), [SOAP](https://cs.wikipedia.org/wiki/SOAP) and [WSDL](https://en.wikipedia.org/wiki/Web_Services_Description_Language). Available Python SOAP pkgs can be found on [wiki.python.org](https://wiki.python.org/moin/WebServices#SOAP).


## Description
This Python project is focused on opening RFEM 6 to all of our customers, enabling them to interact with RFEM 6 on a much higher level. If you are looking for a tool to help you solve parametric models or optimization tasks, you have come to the right place. This community serves as a support portal and base for all of your future projects. The goal is to create an easily expandable Python library, which communicates instructions to RFEM 6 through WebServices (WS). WS enables access to RFEM 6 either via a local instance or a remote internet connection.

## Architecture
<a align="center">


</a>

### Data Structure
* [![main](https://img.shields.io/badge/main.py-blue)](main.py): setting of individual objects by one line entry
* [![window](https://img.shields.io/badge/window.py-blue)](/RFEM/window.py): definition of GUI layer; called first
* [![initModel](https://img.shields.io/badge/initModel.py-blue)](/RFEM/initModel.py): runs after window and initializes suds.Client by connecting to `http://localhost:8081/wsdl` and active model in RFEM. It also evelops esential global functions.
* [![enums](https://img.shields.io/badge/enums.py-blue)](/RFEM/enums.py): definition of enumerations
* [![dataTypes](https://img.shields.io/badge/dataTypes.py-blue)](/RFEM/dataTypes.py): definition of special data types
* [![RFEM](https://img.shields.io/badge/RFEM-blue)](/RFEM): folder following structure of RFEM 6 navigator containing individual types of objects


## Getting started

### Dependencies
Dependency check is implemented inside [initModel.py](/RFEM/initModel.py) with option to install during execution.
* <img align="left" alt="Visual Studio Code" width="26px" src="./img/PyPI.png" style="padding-right:2px;" />PyPi pkgs: [SUDS](https://github.com/cackharot/suds-py3), [requests](https://docs.python-requests.org/en/master/), [six](https://pypi.org/project/six/), [mock](https://pypi.org/project/mock/), and [xmltodict](https://pypi.org/project/xmltodict/).

* <img align="left" alt="Visual Studio Code" width="26px" src="./img/RFEM.png" style="padding-right:2px;" />RFEM 6 application. Client is always compatible with the latest version.

### Step by step
1) 🌀 [Clone](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository#:~:text=Cloning%20an%20Existing%20Repository) this repository (if you have GitHub account) or download actual [release](https://github.com/Dlubal-Software/RFEM_Python_Client/releases)
2) <img align="left" alt="Visual Studio Code" width="18px" src="./img/RFEM.png" style="padding-right:2px;" />Open RFEM 6 application

3) ☑️ Check if there are no opened dialogues in RFEM and server port range under *Options-Web Services* corresponds to the one set in initModel
4) 🏃 Run your script. Inspirations can be found in [Examples](/Examples/) or [UnitTests](/UnitTests/).

### Examples
Scripts intended to be used as templates or examples. Also can be used for testing of backward compatibility.

### Unit Tests
Collection of scripts to support further development.

## Documentation
For complete description of classes and functions visit our [![image](https://img.shields.io/badge/GitHub-page-darkblue?logo=github&amp;)](https://dlubal-software.github.io/RFEM_Python_Client/).

## Wiki
If you run into problems see our [Wiki](https://github.com/Dlubal-Software/RFEM_Python_Client/wiki). We are slowly but surely expanding the solutions to the problems found in the Issues section.

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Contribute
Contributions are always welcome! Please ensure your pull request adheres to the following guidelines:

* Alphabetize your entry.
* Search previous suggestions before making a new one, as yours may be a duplicate.
* Suggested READMEs should be beautiful or stand out in some way.
* Make an individual pull request for each suggestion.
* New categories, or improvements to the existing categorization are welcome.
* Keep descriptions short and simple, but descriptive.
* Start the description with a capital and end with a full stop/period.
* Check your spelling and grammar.
* Make sure your text editor is set to remove trailing whitespace.
* Use the #readme anchor for GitHub READMEs to link them directly

NOTE: Development is in early stages so please respect that. There will be broken objects or adjustments affecting backward compatibility. Use Issues section to point out any problems. Thank you for your understanding.


### 🤝 Connect with us:

[![website](./img/globe-light.svg)](https://www.dlubal.com/en)
&nbsp;&nbsp;
[![website](./img/youtube-light.svg)](https://www.youtube.com/c/DlubalEN)
&nbsp;&nbsp;
[![website](./img/twitter-light.svg)](https://twitter.com/dlubal_en)
&nbsp;&nbsp;
[![website](./img/linkedin-light.svg)](https://de.linkedin.com/company/dlubal-software)
&nbsp;&nbsp;
[![website](./img/instagram-light.svg)](https://www.instagram.com/dlubal_software/)
&nbsp;&nbsp;
[![website](./img/github-light.svg)](https://github.com/Dlubal-Software)

### Languages and Tools 🛠️

[<img align="left" alt="Visual Studio Code" width="26px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" style="padding-right:15px;" />](https://code.visualstudio.com/)
[<img align="left" alt="Visual Studio Code" width="26px" src="./img/Python.png" style="padding-right:15px;" />](https://www.python.org/)
[<img align="left" alt="Visual Studio Code" width="26px" src="./img/RFEM.png" style="padding-right:15px;" />](https://www.dlubal.com/en/products/rfem-fea-software/what-is-rfem)
[<img align="left" alt="Visual Studio Code" width="26px" src="./img/RSTAB.png" style="padding-right:15px;" />](https://www.dlubal.com/en/products/rstab-beam-structures/what-is-rstab)
[<img align="left" alt="JavaScript" width="26px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" style="padding-right:15px;" />](https://www.javascript.com/)
[<img align="left" alt="Node.js" width="26px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" style="padding-right:15px;" />](https://nodejs.org/en/)
[<img align="left" alt="Node.js" width="26px" src="./img/csharp.png" style="padding-right:15px;" />](https://docs.microsoft.com/en-us/dotnet/csharp/)
[<img align="left" alt="GitHub" width="26px" src="https://user-images.githubusercontent.com/3369400/139448065-39a229ba-4b06-434b-bc67-616e2ed80c8f.png" style="padding-right:15px;" />](https://github.com/Dlubal-Software)
<img align="left" alt="Terminal" width="26px" src="./img/terminal-light.svg" style="padding-right:15px;" />