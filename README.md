# three-two-one

List of Commands To Make Your Own Gem
  //first you're going to clone my repo down to a folder, then just go through the commands from that directory!
  //based on RubyGems.org documentation: http://guides.rubygems.org/make-your-own-gem/
  git clone https://github.com/billhimmelsbach/three-two-one
  cd three-two-one
  gem build threetwoone.gemspec
  gem install ./threetwoone-0.0.1.gem
  irb
  require 'threetwoone'
  Threetwoone1.threetwoone
  quit
  // If you want to actually upload your awesome gem, the next step requires you to have an account on RubyGems.org which is super easy to do.
  // Once you have set it up, you'll have to run the following command with your own username:
  // curl -u YOUR_USERNAME https://rubygems.org/api/v1/api_key.yaml > ~/.gem/credentials; chmod 0600 ~/.gem/credentials
  // You won't be able to push to RubyGems though using the name "Threetwoone" because I already took that name for my project!
  // But you can tweak the names of the files to anything you want!
  gem push Threetwoone-0.0.1.gem
