# GitHub Extension for Visual Studio
###test
The GitHub Extension for Visual Studio provides GitHub integration in Visual Studio 2015.
Most of the extension UI lives in the Team Explorer pane, which is available from the View menu.

Official builds of this extension are available at [the official website](https://visualstudio.github.com).

[![Join the chat at freenode:github-vs](https://img.shields.io/badge/irc-freenode:%20%23github--vs-blue.svg)](http://webchat.freenode.net/?channels=%23github-vs) [![Join the chat at https://gitter.im/github/VisualStudio](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/github/VisualStudio?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Installing beta versions

Older and pre-release/beta/untested versions are available at [the releases page](https://github.com/github/VisualStudio/releases), and also via a custom gallery feed for Visual Studio.

You can configure the gallery by going to `Tools / Options / Extensions and Updates` and adding a new gallery with the url https://visualstudio.github.com/releases/feed.rss. The gallery will now be available from `Tools / Extensions and Updates`.

Beta releases will have `(beta)` in their title in the gallery, following the version number. You can view the release notes in the gallery by hovering over the description, or by clicking the `Release Notes` link on the right side.

## Build requirements

* Visual Studio 2015
* Visual Studio SDK

## Build

Clone the repository and its submodules in a git GUI client or via the command line:

```
git clone https://github.com/github/VisualStudio
cd VisualStudio
git submodule init
git submodule deinit script
git submodule update
```

Open the `GitHubVS.sln` solution with Visual Studio 2015.
To be able to use the GitHub API, you'll need to:

- [Register a new developer application](https://github.com/settings/developers) in your profile.
- Open [src/GitHub.App/Api/ApiClientConfiguration.cs](src/GitHub.App/Api/ApiClientConfiguration.cs) and fill out the clientId/clientSecret fields for your application.

## Contributing

Visit the [Contributor Guidelines](CONTRIBUTING.md) for details on how to contribute as well as the [Open Code of Conduct](http://todogroup.org/opencodeofconduct/#VisualStudio/opensource@github.com) for details on how to participate.

## Copyright

Copyright 2015 - 2016 GitHub, Inc.

Licensed under the [MIT License](LICENSE.md)
