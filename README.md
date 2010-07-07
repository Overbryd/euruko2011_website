# This is the EuRuKo 2011 Website

It has very interesting publication/collaboration possibilities.
Authors are collaborators to this repository, they can just push to publish changes.

The server is constantly pulling from this repository. A Jekyll process, takes care to generate a static version of the site.
All static files are served by a Nginx webserver.

## Rake tasks

There is a rake task that will get you up & writing:

    rake post title="Your title in here"

It will create a new file with an apropriate filename and YAML front matter.

## Collaboration

Forking and sending pull requests to improve the website is highly appreciated.

## Publishing

Just do it (if you are collaborator to this repository):

    git push

## Serving the website locally

You can do this by cloning this repository and running Jekyll:

    git clone git://github.com/Overbryd/euruko2011_website.git

    cd euruko2011_website

    jekyll --server
    
    open http://localhost:4000/
