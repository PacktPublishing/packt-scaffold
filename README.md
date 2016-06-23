# GitBook Scaffold for Packt Products

This is an example GitBook-based development workflow. Content is written and edited directly in markdown, and content versioning is handled by Git. The configuration for this project includes several Packt-specific npm modules that make changes to the layout of the core output target (which in this case, is the statically generated website). Many of the changes made via these modules are intended to support integration with Electron, so that course products can be built and shipped as standalone desktop applications.

Getting this working is quite straightforward as it's mostly vanilla. With a decent version of node installed, run `npm install -g gitbook-cli`, navigate to your directory where this scaffold is located, run `gitbook install` and then `gitbook serve`. The idea is that editors do not have to worry about configuration, only what is added or modified in the content directory.

![UI Demo](content/assets/demo.gif)

If you spot anything broken get in touch, as this is primarily a quick-and-dirty MVP.
