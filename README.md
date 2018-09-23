# unistall-a-package


The command is simply npm uninstall <name>

The nodejs documents https://npmjs.org/doc/ have all the commands that you need to know with npm.

A local install will be in the node_modules/ directory of your application. This won't affect the application if a module remains there with no references to it.

If you're removing a global package however, any applications referencing it will crash.

Here are different options:

npm uninstall <name> removes the module from node_modules, but not package.json

npm uninstall <name> --save also removes it from dependencies in package.json

npm uninstall <name> --save-dev also removes it from devDependencies in package.json

npm -g uninstall <name> --save also removes it globally
