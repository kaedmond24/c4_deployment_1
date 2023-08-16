# Deployment using Jenkins and AWS Elastic Beanstalk

1. Log into the Jenkins server using your _username_ and _password_

2. On the Jenkins dashboard, select a _new item_ to setup the pipeline

3. Create a name, then select the _Pipeline_ option

4. Define a pipeline script using the ‘Pipeline script from SCM’ option

5. Enter the Github repository link for the project

6. Select _Add_ to setup your Github credentials

   - [How to setup Github access token](https://docs.github.com/en/enterprise-server@3.8/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

7. Select your Github credentials

8. Set _Branch Specifier_ to _\*/main_ branch

9. Apply and Save

10. Select _Build Now_ option

11. Wait for _SCM Checkout_, _Build_, and _Test_ stages to complete

12. Upon Successful completion, package application files into a zip file in preparation for deployment to AWS Elastic Beanstalk

13. Login into AWS console

14. Create IAM roles for needed services

    - [How to Create an AWS IAM Role for Elastic Beanstalk and EC2](https://scribehow.com/shared/How_to_Create_an_AWS_IAM_Role_for_Elastic_Beanstalk_and_EC2__kTg4B7zRRxCp-aYTJc-WLg)

15. Setup AWS Elastic Beanstalk

    - [Create and Deploy a Python URL Shortener on AWS Elastic Beanstalk](https://scribehow.com/shared/How_to_Create_and_Deploy_a_Python_URL_Shortener_on_AWS_Elastic_Beanstalk__MS9pB8lfRaGFiKAq2FU-cw)

16. Test application access using the domain link provided by AWS Elastic Beanstalk
