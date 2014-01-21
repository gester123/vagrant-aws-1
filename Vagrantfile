Vagrant.configure("2") do |config|
  config.vm.box = "dummy"
  
  config.vm.provider :aws do |aws, override|
    aws.access_key_id = "ACCESS_KEY_ID"
    aws.secret_access_key = "SECRET_ACCESS_KEY"
    aws.keypair_name = "KEYPAIR_NAME"

    aws.ami = "ami-fb436392"  
    aws.instance_type = "m1.small"
    aws.region = "us-east-1"


    override.ssh.username = "ubuntu"
    override.ssh.private_key_path = "~/Documents/Projects/this.pem"
    
  end

end