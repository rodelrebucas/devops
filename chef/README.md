#### Installing chef on Windows 7 using chocolately
    
    choco install chefdk (must have an elevated rights)

### Start the chef client service

    chef-service-manager -a start

#### Generate your cookbook 

    chef generate cookbook first_cookbook

#### Setup config files

    touch config.rb
    touch web.json

#### Run the cookbook

    chef-solo -c config.rb -j web.json