# install_aws_genomics_cli_ubuntu


aws s3api get-object --bucket healthai-public-assets-us-east-1 --key amazon-genomics-cli/nightly-build/amazon-genomics-cli.zip amazon-genomics-cli.zip

unzip amazon-genomics-cli-<version>.zip
cd amazon-genomics-cli/ 
./install.sh
  
  If this gives bwlo error
  
ERROR: npm is known not to run on Node.js v10.19.0
You'll need to upgrade to a newer Node.js version in order to use this
version of npm. You can find the latest version at https://nodejs.org/
  
  Then install latest Node.js
  
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash

  nvm ls-remote

  nvm install <version>
  
  nvm use <version>

  node -v
  
  Then run ./install.sh

  
