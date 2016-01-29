#### Install Node.js and npm

[Node.js](https://nodejs.org) comes bundled with [npm](https://www.npmjs.com/). Pre-built installers are available at [nodejs.org](https://nodejs.org/en/download/) or use a [package manager](https://nodejs.org/en/download/package-manager/) to perform the installation. Check the version to insure the install was successful.

```Shell
$ node -v
```

npm is updated frequently. Run the following command with the global flag set to ensure you are running the latest version. Then check the version to insure the update was successful.

```Shell
$ npm install npm@latest -g
$ npm -v
```
*Homebrew users*: Homebrew installs both Node.js and npm when the ```brew install node``` command is issued.  This can later lead to [problems](https://gist.github.com/DanHerbert/9520689) if one attempts to update npm itself using the npm command ```npm update npm -g```.  So consider allowing npm to manage both itself and its packages independent of Homebrew by *explicitly* excluding it from the install.  Once both Node.js and npm are installed, add ```~/.node/bin``` to your ```PATH``` environment variable so that you access NPM commands globally. 

```Shell
$ brew install node --without-npm
$ echo prefix=~/.node >> ~/.npmrc
$ curl -L https://www.npmjs.com/install.sh | sh
```

```Shell
export HOME=/Users/<username>
export NODE_HOME=$HOME/.node
export PATH=$NODE_HOME/bin:$PATH
```

#### Install Gitbook

Gitbook is a Node.js library that provides command line tooling for Gitbook projects.

```Shell
$ npm install gitbook-cli -g
```

#### Fork and clone the caliper-book repo

Fork the [caliper-book](https://github.com/arwhyte/caliper-book) repository and then clone it locally.

```Shell
$ cd myrepos
$ git clone https://github.com/arwhyte/caliper-book.git
```

#### Serve Gitbook locally

Serve your local repo as a book in order to view your changes dynamically as you work.

```Shell
$ gitbook serve
```

For additional Gitbook documentation visit http://help.gitbook.com/.