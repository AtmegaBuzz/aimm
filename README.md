<div align="center">
  
# `🤖 Aimm (AI Model Manager)`
## **A CLI App to manage your machine learning models**

</div>

![Basic Use](resources/docs/terminal.gif)



```
Usage: aimm [command] [options]

Current Dir:
  init                                        Initialize aimodels.json.
  add <model_name>:[version]                  Add a model to aimodels.json.
  remove <model_name>:[version]               Remove a model from aimodels.json.

System Wide:
  list                                        List all models.
  info <model_name>:[version]                 Get info about a model.
  install <model_name>:[version]              Install a model.
  uninstall <model_name>:[version]            Uninstall a model.
  credentials <user>@<domain>                 Set credentials.

Search:
  search <query>                              Search for a model.
  search <query> --include-adult              Search for a model and include adult results.
  search <query> --only-adult                 Search for a model and only include adult results.

Options:
  --install-completion          Install completion for the current shell.
  --show-completion             Show completion for the current shell, to copy it or customize
                                the installation.
  --help                        Show this message and exit.

Run 'aimm help [command]' for more information on a command.
```


## 📖 Table of Contents

- [📖 Table of Contents](#-table-of-contents)
- [📝 Description](#-description)
- [📦 Installation](#-installation)
- [📃 Usage](#-usage)
- [💻 Quickstart](#-quickstart)
- [📒 Examples](#-examples)
- [📚 Documentation](#-documentation)
- [📜 License](#-license)

## 📝 Description

AI Model Manager CLI, it's like pip or npm - but for AI models!

For users, this allows easily managing your collection of AI models. It stores your models in a location that all of your AI enabled apps can access, so you don't need to worry about the huge files taking up so much space, or creating symlinks. Finally, no more having to hunt for a model and making sure you rename it and put it in the correct folder correctly. 

For developers, it means less code that you have to handle initializing your app and collecting all of the AI model resources needed. AI Model Manager also will provide security through checksum checks and pickle scanning.

## 📦 Installation

```bash
pip install <package_name>
```

## 📝 Usage

```bash
aimm <command> <args>
```

## 💻 Quickstart

First search for a model you want to use. For example the BSRGAN model, a super resolution model that can upscale images.

```bash
aimm search BSRGAN
```

Then we install the model

```bash
aimm install BSRGAN
```

You can also add it to a local aimodels.json file to keep track of all the models you use in your project.


First we have to initialize the aimodels.json file


```bash
aimm init
```

Then we can add the model to the file

```bash
aimm add BSRGAN
```


## 📒 Examples

```bash
examples with pictures go here
```

## 📚 Documentation

[Documentation](https://docs.aimodels.org)

## 📜 License

[Apache License 2.0](./LICENSE.md)