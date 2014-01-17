10 Deployments a Day
====
##A brief on extreme release protocols.

###@Webonise

A true Weboniser at heart, I started my career with Webonise Lab. A humble and small IT firm that was founded in the year 2009. Webonise Lab was formed with a crew of just 4 people that grew on to 10 (by the time I joined..) - 10 very determined and young minds. All of them freshly out of college who had joined forces forming a strong team with their interleaving skills and interests. Webonise is an outsourced product development company that goes about building applications that people love!

##2009-2010 - An Era of Struggle With Almost Everything...

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

Our deployment rate was really embarassing! But we needn't worry. As I said, we were and are a bunch of really determined indivuduals. We were confident we'd figure out a better solution.

##2010-2011 The Upliftment

With a new year and quite some experience by then, we were all set to move on and re-define how we dealt with deployments, learning their importance the hard way. 

The first thing we put to practice was Versioning. We started using versions like 'test' and 'stage' and 'production' depending on the purpose for which we deployed our application.

We also introduced Capistrano - an open source tool for running scripts on multiple servers. With this, deployment on multiple instances became easier and it helped us manage our deployments better.

We also felt the need to monitor the errors and exceptions in our applications. There was no way to figure out something went wrong in the application or something has broken until we came across it ourselves. So we implmented plugins that notified us or errors and exceptions. Made us react faster to these situations and have them fixed before more damage was done.

###Our First Mess Up

Well we were amateurs, with some experience, and the potential to mess up deployments completely. And so, we did. We were making some major front end changes to an already live site and had to deploy for testing it internally. While doing a 'cap deploy' we accidentally deployed it on production which was the environment for the live site. And ka-boom! What a mess! We went ballistic over fixing it and undoing it on production, and dont even get me started on the client feedback! A nightmare as it was, mistakes like these are unaffordable for any startup. And this had to be dealt with seriously.

###2010-2011 Lessons Learnt

* With our epic mess up, and some more experince toying around with deployments, we realised one thing, and that was - 

  Rollback application code - easier with versioning but rolling back database - still aint an easy task.

* What we also understood, is that deployments should not be assigned to everyone and anyone involved with development. An experienced, responsible selected lot should deal with deployments to avoid such accidents. And so, we felt the need to control who had access to deployments and related tasks.


###2011-2012 One Step Ahead

With a new year came new ideas, more experience and maturity in the way we did things. With past mistakes and learnings, we decided to introduce dedicated SysAdmins who would handle deployments and related tasks.
SysAdmins are sophisticated and trained individuals who are well expertised in deployments, infrastructure management and handling servers efficiently. 
We also started writing bash scripts for installations of services, tools and plugins. This reduced the laborious efforts of installing all dependencies and tools and plugins manually one-by-one.

To make life easier, we moved from capistrano to webistrano. Capistrano being the remote server automation tool that helped us with our deployments, webistrano gave us a web UI for managing capistrano deployments. Neat right?

While we went all "cool" using more sophisticated tools and plugins to aid our deployments, we were still facing problems and deployments weren't all that smooth. Now the question was, what are we still doing wrong? Well not wrong entirely, but realisation dawned upon us that SysAdmins were not able to understand the developer's side of the story and other technicalities of running the application and had to be spoon fed with a lot of details like - dependencies, security, scalability, availability, database and so on and so forth. This was creating a road block for achieving efficient deployments.

###2011-2012 Lessons Learnt

* We figured that we needed to bridge this gap between developers and SysAdmins. We needed to introduce someone that had a fair knowledge of both to make 

Our deployment rates reached 2-3 deployments a week. Which, I believe, is an achievement in itself considering the previous rate.
But this is not enough! With the number of projects growing, the company growing, and the need for more frequent deployments, this rate was definitely not enough!


