## Setup your computer for Blacklight development in advance

During the workshop you will be learning to customize Blacklight while following along on your local computer. We ask that you set up your development environment in advance of the workshop. Developers may do this in a variety of different ways. Please do this however you feel most comfortable. You will need to be able to do the following:

- Run this Ruby on Rails application
- Edit files in a Rails application and see the changes
- Run an instance of Solr. We will recommend using `solr_wrapper` (pre-configured with this application) for this workshop. If you plan to use something different,  you are welcome to, as long as you can use the same solr configurations see `solr/conf` and can index our fixture data.

If you are new to Ruby on Rails development we recommend the following guide to get started: https://gorails.com/setup/ . This will help you set up the Ruby and Rails requirements for the workshop.

## Development system requirements:
- Install Ruby (2.7.1 recommended) https://gorails.com/setup#ruby
- Java version 8 or higher (for solr). See the Solr documentation for how to check this
https://lucene.apache.org/solr/guide/8_4/solr-system-requirements.html#java-requirements 

### To test your setup.. 
Clone https://github.com/projectblacklight/intro-to-blacklight-2020

1. Run `$ bin/setup`
2. In a separate terminal window, run `$ bundle exec solr_wrapper` to launch solr
3. Run `$ bin/rails blacklight:index:seed`
4. Run `$ bin/rails server`

Open http://localhost:3000 in a browser 

You should see a Blacklight application that looks similar to https://demo.projectblacklight.org.
