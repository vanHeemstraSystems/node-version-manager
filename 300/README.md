# 300 - Building Our Application

## 100 - Set up nvm

The full instructions for installation are on GitHub , but in general it is as simple as:

```
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

We can instruct nvm to use the latest LTS version (currently 20.12.0) by creating a ```.nvmrc``` file at the root of our project with the contents:

```
lts/*
```
.nvmrc

Now our directory tree will look like:

```
.
└── .nvmrc
```

And then running the command:

```
$ nvm install
```

## 200 - Setup npm

**npm** or "Node Package Manager" is a tool to install Node.js packages. To set up our project run the command:

```
$ npm init
```

And follow the prompts. Hitting the enter key for all prompts is fine for now if you don't want to fill it all out. This will create an initialized **package.json** for us:

```
.
├── .nvmrc
└── package.json
```

## 300 - Setup an node module like Metalsmith

From the root of our project run the command:

```
$ npm install --save metalsmith
```

Which will install Metalsmith and all required dependencies. This will create the node_modules/ directory (with many subdirectories in it) and the package-lock.json file. To save some space I'll skip writing out all the extra node_modules/ subdirectories:

```
.
├── .nvmrc
├── node_modules
│   └── metalsmith
├── package-lock.json
└── package.json
```
