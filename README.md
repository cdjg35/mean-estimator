[![TravisCI](https://travis-ci.org/garystafford/mean-estimator.svg?branch=master)](https://travis-ci.org/garystafford/mean-estimator)&nbsp;&nbsp;
[![David Dependencies](https://david-dm.org/garystafford/mean-estimator.png)](https://david-dm.org/garystafford/mean-estimator)&nbsp;&nbsp;
[![David Dev Dependencies](https://david-dm.org/garystafford/mean-estimator/dev-status.png)](https://david-dm.org/garystafford/mean-estimator#info=devDependencies)&nbsp;&nbsp;
[![Gitter](https://badges.gitter.im/Join Chat.svg)](https://gitter.im/garystafford/mean-estimator?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)&nbsp;&nbsp;

[![Codeship](https://codeship.com/projects/ffb358c0-4ab8-0132-efcb-7aa9472b8ea5/status)](https://codeship.com/projects/46419)

## MEAN Estimator

This project is built using MEAN.JS - Full-Stack JavaScript Using MongoDB, Express, AngularJS, and Node.js. 
From Creators of MEAN.IO (<http://www.meanjs.org>). Sample MEAN application for estimating the cost and resources
required to add, update, and remove system components in development and test software environments.
For example, adding a new web server to a test environment, or updating a load-balancer in production.

* Project source code and architecture originally based on the MEAN.JS project on GitHub (<http://www.github.com/meanjs>)
* Docker and fig configuration originally based on post on GiantSwarm Blog (<http://blog.giantswarm.io/getting-started-with-docker-and-meanjs>)
* Contains (3) modules: core, estimates, and modules
* Data for Components, Environments, Estimate Types, and Resources are all read from json configuration file:`app/data/formData.json`
* Can be built locally (npm, bower, grunt) or now with fig (<http://www.fig.sh>) and docker (<http://www.docker.com>)
* Run in browser at `http://localhost:3111`

**View Estimates**  
List all estimates. Click on an estimate in the list to view the estimate details.  
RESTful endpoint (GET): `http://localhost:3111/estimates`

**View Estimate Details**  
Click on an estimate in the list of estimates to view the estimate details.  
RESTful enpoint (GET): `http://localhost:3111/estimates/<estimate_id>`

**New Estimate**  
Add a new estimate.  
RESTful endpoint (POST): `http://localhost:3111/estimates`

**Update an Estimate**  
Update an existing estimate. Access from the list of estimates.  
RESTful endpoint (PUT): `http://localhost:3111/estimates/<estimate_id>`

**Delete an Estimate**  
Update an existing estimate. Access from the list of estimates.  
RESTful endpoint (DELETE): `http://localhost:3111/estimates/54716703da107e3500c083a5`

**View Reports** _Coming Soon_  
View estimate summary reports coming soon. Service working.  
RESTful endpoint:  
`http://localhost:3111/reporting/resources`
`http://localhost:3111/reporting/infrastructure`

###Code Details

Optional environment variables (defaults if not set, below)
```
echo 'export NODE_PORT=3111' >> ~/.bashrc
echo 'export NODE_ENV=development' >> ~/.bashrc
echo 'export ENV_FORM_DATA=../../app/data/formData.json' >> ~/.bashrc
. ~/.bashrc
```

Run locally
```
npm install
bower install
grunt
node server # alternate method
```

Build and run with fig and Docker
```
docker pull dockerfile/nodejs
docker pull mongo
fig build && fig up
```
Alternate way to build and run with fig and Docker  
Builds two containers (`db_1` and `web_1`) using `fig.yml` file  
NOTE: script removes all exited containers and untagged images
```
. fig_start.sh
```

###Preview
![Main Page - Desktop](https://github.com/garystafford/mean-estimator/blob/master/images/main_page.png?raw=true)

![Signup Page - Mobile](https://github.com/garystafford/mean-estimator/blob/master/images/signup_mobile.png?raw=true)

![Main Page - Mobile](https://github.com/garystafford/mean-estimator/blob/master/images/main_page_mobile.png?raw=true)

![Estimate Detail Page - Mobile](https://github.com/garystafford/mean-estimator/blob/master/images/estimate_detail_mobile.png?raw=true)

![Estimate Edit Page - Mobile](https://github.com/garystafford/mean-estimator/blob/master/images/edit_estimate_mobile.png?raw=true)
