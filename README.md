Slow Travel Berlin
------------------

This repo contains configuration for the Slow Travel
Berlin website.

Overview
========

The site is a Wordpress installation deployed using Docker.
In order to test locally or do a deployment, you'll need to
install [Docker](https://www.docker.com/products/docker).

If you aren't deploying the site but just administering it,
no need to install Docker, it's all through the web. Skip
down to [configuration](#configuration) for further
instructions.

Deployment<a name="deployment"></a>
===================================

The deployment of the site is designed to be simple,
self-contained, and repeatable. Docker, through the
`docker-compose` tool, allows us to specify a full
environment, and the relationship between the various
services used (such as the database, caching
proxy, and website itself).

It's important to stress that the strength of this
setup is the confidence you have in being able to
deploy the site again, anywhere, on any hosting
provider. As a result, it's important to resist the
temptation to change fundamental aspects of the
infrastructure outside of Docker. If you do,
if someone comes along expecting the deploy to
be as easy as a `docker-compose up` they are
going to be confused as to why your fancy add-on
does not work.

When in doubt, at least heavily document what was
done. Or learn Docker. It's easy, I promise. :)

For a full run through of how to deploy the
site, see the [DEPLOYMENT](docs/DEPLOYMENT.md)
page in the docs.

Configuration<a name="configuration"></a>
=========================================

Configuration steps are still being squared
away, and are dependent on what themes
and plug-ins are found to be necessary.
Full instructions can be found at the
[Configuration](docs/CONFIGURATION.md)
page.
