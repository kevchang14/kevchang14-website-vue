# kevchang14-website-vue

## Install Vue CLI

### Install Scoop, a Windows command line installer
https://github.com/lukesampson/scoop/wiki/Quick-Start

### Install YARN
Make sure to install nodejs as well

https://classic.yarnpkg.com/en/docs/install/#windows-stable

### Install Vue
https://cli.vuejs.org/guide/installation.html

The command below installs both Vue as well as the CLI service that enables hot-reloads and serves your static content locally

```
yarn global add @vue/cli @vue/cli-service-global
```

### Update Vue to not use the Taobao Registry (optional)
The Taobao registry seems to negatively impact performance when creating a project and installing dependencies. Disable it by checking the vue configuration
```
vue config
```
Set in the file returned in the Resolved file path 
```
useTaobaoRegistry: false
```

## Running a project

### Using the Vue UI
Start the UI by running 
```
vue ui
```
You can use the UI to create a new project or import an existing project. The UI even includes a handy dependency manager to install new JS packages (make sure to run npm install if you're importing an existing project). Start your development server under "Tasks" then "Serve"

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

### CI/CD Tutorial
https://dev.to/rossta/deploying-a-vuejs-website-to-amazon-s3-with-circleci--5hh7
