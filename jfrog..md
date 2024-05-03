## Jfrog Artifactory first Setup 

[System Requirment](https://jfrog.com/help/r/jfrog-installation-setup-documentation/artifactory-system-requirements-and-platform-support)

## 🚀 Installation Steps

- Provision the VM with the required resources (OS Platform)
- Patch the OS with latest version of core component
- Install the java-1.8.0-openjdk-devel ( and Latest supporting version)
- Download the Jfrom RPM from Jfrog official wbesite [URL](https://releases.jfrog.io/artifactory/artifactory-rpms/jfrog-artifactory-jcr/jfrog-artifactory-jcr-[RELEASE].rpm)
- Install the downloaded rpm package
- Start the Artifactory service
- On Welcome page provide the Artifactory License Key and Xray License Key (This Key is Valid for 30 Days Only if you are working on test setup)
    * Artifactory License Key : cHJvZHVjdHM6CiAgYXJ0**************
    * Xray License Key : cHJvZHVjdHM6CiAgeHJheToKICAgIHByb2****************
- Login with the Default Credentials
    * Username : admin
    * Password : password

Thanks for stopping by! Let's connect and explore the fascinating world of Jfrog Artifactory together. 🚀

## Note :
    * Command to Update the core component on RHEL 6/7/8/9
        # sudo yum update -y
    * Command to Update the core component on Ubuntu 18/20/22
        # sudo apt update -y
        # sudo apt upgrade -y
    * Command to Install the Jfrog Artifactory
        # sudo yum install jfrog-artifactory-jcr-[RELEASE].rpm -y
        # sudo apt install jfrog-artifactory-jcr-[RELEASE].deb -y
    * Command to Start the Artifactory Service
        # sudo systemctl start artifactory
    [Jfrog CLI CheatSheet](https://github.com/ShailAdmin/DevopsDocs/blob/master/JFrogCLI_CheatSheet-v2.pdf)


    