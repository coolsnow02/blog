10 Deployments a Day
====
##A brief on extreme release protocols.

###@Webonise

A true Weboniser at heart, I started my career with Webonise Lab. A humble and small IT firm that was founded in the year 2009. Webonise Lab was formed with a crew of just 4 people that grew on to 10 (by the time I joined..) - 10 very determined and young minds. All of them freshly out of college who had joined forces forming a strong team with their interleaving skills and interests. Webonise is an outsourced product development company that goes about building applications that people love!

###2009-2010 - An Era of Struggle With Almost Everything...

With the new born startup and a bunch of amateurs in the team, we struggled with everything we did. Planning and executing our first project, developing the project the right way, deploying the proeject, testing it. Everything was an experiment (that is why 'Lab'. The company was made to experiment with technology and new trends). With some basic bookish knowledge on project planning and development that came from the tedious 4-year college graduation was kind of helpful - mind you - "kind of". But deployment and related techniques were totally alien. And getting our first project live was a herculean task. We had no idea of how to go about it.

#### Our Stone-Age Deployment Techniques - 
We started deploying using some really age-old methedologies that involved doing everything manually. 

* First we created an instance on the server(manually - of course).
* Then we installed the dependencies one-by-one.
* Pulled from Git into each instance.

We faced several problems while doing this.
For one, with modifications in our database through migrations, we goofed up data on a live site and rolling back migrations was a problem. Loss of important live data was a different concern altogeher.


With a few more projects and a few more deployments, we realised that this was a very tedious task and we had to find a better way to do it! We are techies.. we had to!

#### 2009-2010 Lessons Learnt
With growing number of projects and need for more deployments, we could not carry on with this rate. Our current deployment rate? 1 deployment in 1 week or two. In all this, we concluded that if we were to grow, we could not keep following this method for each deployment. We realised that we needed versions for our deployments, so that the next time "accidents" happen, we can recover more efficiently.

Our deployment rate is really embarassing! But we needn't worry. As I said, we were and are a bunch of really determined indivuduals. We were confident we'd figure out a better solution.

###2010-2011 The Upliftment

With a new year and quite some experience by then, we were all set to move on and re-define how we dealt with deployments, learning their importance the hard way. The first thing we put to practice was Versioning. We started using versions like 'test' and 'stage' and 'production' depending on the purpose for which we deployed our application.
We also introduced Capistrano - an open source tool for running scripts on multiple servers. With this deployment on multiple instances became easier and it helped us manage our deployments better.
