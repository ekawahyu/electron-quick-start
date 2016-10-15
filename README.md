# electron-quick-start

**Clone and run for a quick way to see an Electron in action.**

This is a minimal Electron application based on the [Quick Start Guide](http://electron.atom.io/docs/latest/tutorial/quick-start) within the Electron documentation.

**Use this app along with the [Electron API Demos](http://electron.atom.io/#get-started) app for API code examples to help you get started.**

A basic Electron application needs just these files:

- `package.json` - Points to the app's main file and lists its details and dependencies.
- `main.js` - Starts the app and creates a browser window to render HTML. This is the app's **main process**.
- `index.html` - A web page to render. This is the app's **renderer process**.

You can learn more about each of these components within the [Quick Start Guide](http://electron.atom.io/docs/latest/tutorial/quick-start).

## To Use

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/ekawahyu/electron-quick-start-serialport
# Go into the repository
cd electron-quick-start-serialport
# Install nvm using curl
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.32.0/install.sh | bash
# or install nvm using wget
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.32.0/install.sh | bash
# Install node.js 5.12.0
nvm install 5.12.0
# Install electron globally
npm install -g electron
# Install node-gyp globally
npm install -g node-gyp
# Install dependencies and run the app
npm install && npm start
```

## Electron-rebuild

For some reason if you get version mismatch, you can try to rebuild the native node module as follow. Please remove all "dependencies" and "devDependencies" from package.json before executing these commands:

```bash
npm install --save serialport
npm install --save-dev electron-rebuild
./node_modules/.bin/electron-rebuild -$(electron -v)
```

Learn more about Electron and its API in the [documentation](http://electron.atom.io/docs/latest).

## Other Example Apps

For more example apps, see the
[list of boilerplates](http://electron.atom.io/community/#boilerplates)
created by the awesome electron community.

#### License [CC0 1.0 (Public Domain)](LICENSE.md)
