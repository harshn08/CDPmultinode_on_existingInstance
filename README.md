# CDPMultinodeDocker

CDP Multinode script using Docker on Mac/Windows 10
Multi Node CDP DC cluster using Ansible script on Docker 

Updated on March 10 , 2020


Assumptions

		This document assumes that you have access to an AWS account.
		Partners or their IT Dept can create their own VPC, Subnet, key-pair and security group in the same availability zone that will be used to create multi node instances in the script below.
		Request cloudera license from partner portal . 
		Access to valid cloudera.com credentials to download binaries
		Access to the relevant script from partner portal here.
		Access to the following versions of docker are used for Mac OS and Windows 10 Pro. 

AWS Dependencies

		AWS keypair (e.g. “.pem”) files to use with the scripts
		Decide on AWS region/AZ (us-east-1 used in this example)
		Image Used: ami-02eac2c0129f6376b #CentOS-7 x86_64 (Ensure an equivalent CentOS image is available in your AZ)
		Create a VPC(or use default), subnet and Security Group (SG) where these nodes are in the same AZ. Record the SG to be used in the config files. Make sure the SG is open to all hosts inside the security group. 
