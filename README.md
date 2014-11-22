<div class="page-header">
<p>
<a href='https://travis-ci.org/garystafford/environment-estimator'><img src='https://travis-ci.org/garystafford/environment-estimator.svg?branch=master'></a>
</p>
<p>
  <a href='https://codeship.com/projects/46419'><img src='https://codeship.com/projects/ffb358c0-4ab8-0132-efcb-7aa9472b8ea5/status'></a>
</p>
<p>
  <a href='https://david-dm.org/garystafford/environment-estimator'><img src='https://david-dm.org/garystafford/environment-estimator.png'></a>
</p>
<p>
  <a href='https://david-dm.org/garystafford/environment-estimator#info=devDependencies'><img src='https://david-dm.org/garystafford/environment-estimator/dev-status.svg?style=flatpng'></a>
</p>
<h2>Environment Application Estimator</h2>
</div>
<p>
  This project is built using MEAN.JS - Full-Stack JavaScript Using MongoDB, Express, AngularJS, and Node.js
  From Creators of MEAN.IO (meanjs.org)
</p>
<p>
  Sample MEAN application for estimating the cost and resources required to add application platforms and
  infrastructure in development and test software environments. Collect and report on time and cost estimates
  from multiple resource groups.
  <ul>
    <li>
      Project source code and architecture originally based on the MEAN.JS project on GitHub
      (github.com/meanjs)
    </li>
    <li>
      Contains (3) modules: core, estimates, and modules
    </li>
    <li>
      Data for Applications, Environments, Estimate Types, and Resources are all read from json configuration file
    </li>
    <li>
      Can be built locally (npm, bower, grunt) or now with fig (fig.sh) and docker (docker.com)
    </li>
    <li>
      Run in browser at http://localhost:3111
    </li>
    </ul>
</p>
<dl>
  <dt><strong>View Estimates</strong></dt>
  <dd>
    List all estimates. Click on an estimate in list to view the estimate details.
    <br>
  </dd>
  <dt><strong>View Estimate Details</strong></dt>
  <dd>
    Click on an estimate in list of estimates to view the estimate details.
    <br>
  </dd>
  <dt><strong>New Estimate</strong></dt>
  <dd>
    Add a new estimate.
    <br>
  </dd>
  <dt><strong>Update an Estimate</strong></dt>
  <dd>
    Update an existing estimate. Access from the list of estimates.
    <br>
  </dd>
  <dt><strong>View Reports</strong> <i>Coming Soon</i></dt>
  <dd>
    View estimate summary reports.
  </dd>
</dl>
<strong>Code details</strong>
<p>
  Optional environment variables (defaults below):<br/>
  <code>echo 'export NODE_PORT=3111' >> ~/.bashrc</code><br/>
  <code>echo 'export NODE_ENV=development' >> ~/.bashrc</code><br/>
  <code>echo 'export ENV_FORM_DATA=../../app/data/formData.json' >> ~/.bashrc</code><br/>
  <code>. ~/.bashrc</code>
</p>
<p> To run locally:<br/>
  <code>npm install</code><br/>
  <code>bower install</code><br/>
  <code>grunt</code><br/>
  <code>node server # alternate method</code>
</p>
<p>
  To run with fig and Docker:<br />
  <code>docker pull dockerfile/nodejs</code><br/>
  <code>docker pull mongo:latest</code><br/>
  <code>fig build</code><br/>
  <code>fig up</code>
</p>
<br>
<img src="https://github.com/garystafford/environment-estimator/blob/master/images/main_page.png?raw=true" alt="Main Page - Desktop">
<br>
<img src="https://github.com/garystafford/environment-estimator/blob/master/images/signup_mobile.png?raw=true" alt="Signup Page - Mobile">
<br>
<img src="https://github.com/garystafford/environment-estimator/blob/master/images/main_page_mobile.png?raw=true" alt="Main Page - Mobile">
<br>
<img src="https://github.com/garystafford/environment-estimator/blob/master/images/estimate_detail_mobile.png?raw=true" alt="Estimate Detail Page - Mobile">
<br>
<img src="https://github.com/garystafford/environment-estimator/blob/master/images/edit_estimate_mobile.png?raw=true" alt="Estimate Edit Page - Mobile">
