---
layout: post
title:      "Sinatra - getting started"
date:       2019-11-04 00:27:40 +0000
permalink:  sinatra_-_getting_started
---


After this project a big take away is how to set up a sinatra application in general. Let's go over the steps. 


1. Save yourself sometime and install the Corneal Gem created by former FlatIron Student Brian Emery after he had become a developer - gem install corneal.
2. Type corneal new "insert project name here no quotes" into the cli and hit enter.
3. Create your git hub repo and set up your project to be able to push.
4. Bundle install.
5. Check to see if everything is working by running shotgun.
6. Create the rake file and add the task for console pry. This will help you later on. 
      task  :console do
             Pry.start
       end
7. Add your models. The prjoect will only require 2 to meet the mvp. Steer away from has many through options unless you are up to the challenge. How difficult were the previous lessons for you to get through?
8. Run rake db:create_migration	NAME=create_users and again for whatever the belongs to object will be.  Make the table name plural so your model name is singular. 
9. Fill out your table data with attributes make sure to give your belongs to object a user_id column in the table - this is the foreign key.
10. Run rake db:migrate
11. Create a db:seeds.rb file so you can use faker or manually create data and add it quickly to test.    
12. Run rake:db:seed with your data so you can test your models, session etc. 
13. Make sure you enable:sessions in the application_controller.rb file as well as set your session_secret, this is done manually ONLY for this test project. Should never be manually created - period.
14. In the config rackup file add -  use Rack::MethodOverride and make sure to use your non ApplicationController. ONLY the application controller should be run. Secondary and tertiary controllers are placed above the application controller and have a command of use. 

You should be ready to rock. There is a lot of work ahead but you should be able to get going without many errors. 
1
	 
  
