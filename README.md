# Reentry Resources Hub

We built the [Buncombe Reentry Resources Hub](http://www.buncombereentryhub.org/) to help those returning
to the community after a period of incarceration or suffering the consequences of a criminal conviction
on their record. Now we are working to scale this resource to every county in North Carolina.
We need help from developers ((Node, React) and writers.

If you are interested in helping, check out the tasks [here](https://github.com/CodeForNC/reentry-resources-hub/projects/3).
This is where we put tasks that don't require deep knowledge of all aspects of the project. If you are an experienced
developer and willing to commit more effort over a longer term, check out the tasks
on [this page](https://github.com/CodeForNC/reentry-resources-hub/projects/2).

## Installation

This repository contains code for both server and client. To develop on your local machine, you will need to install ```node```, ```yarn``` and ```postgresql```. A recent version of ```node`` is required (version >= 7.6). 

If you are using a Mac OSX, install these dependencies using [Homebrew](https://brew.sh/). Once you have homebrew installed, run these following commands in the an empty terminal shell.

'''''
brew install node
brew install yarn
brew install postgresql
````

Next, clone this Reentry Resources Hub repository (or a fork) and install dependencies.
````

If you prefer to use npm, the equivalent procedure is:

````
    git clone https://github.com/Open-NC/reentry-resources-hub.git
    cd reentry-resources-hub
    yarn
````

The descriptions and resource information are stored in a database on AWS. Open an [issue](https://github.com/Open-NC/reentry-resources-hub/issues) and mention [@ejaxon](https://github.com/ejaxon) to obtain credentials or learn how to create a copy of the database. Once you have your username and password, copy the ```server.env.example``` file to a new file with just the ```.env``` extension and replace the placeholder text with your username and password within the file.

You may then run the site locally by running:

````
    yarn start
````

The application is running at http://localhost:3000/. The server is also running, but at http://localhost:3001/.


## Deployment -- NOT VERIFIED

In one terminal, run `node server/index.js`.  In another terminal, run `yarn build` or `npm run build`.

If you want to push the contents of the build folder to GitHub pages, run `yarn deploy`.
