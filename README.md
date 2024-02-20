In my project I used azure to create a web application for a blog.
The first step was to create the web app and to choose a domain. (davidsalpharesume.azurewebsites.net)
I deployed a docker container and used the azure cloud shell to configure the container.
I already created a resource group to run app with so I configured the container with it's settings.
webapp config container set --name davidsalpharesume --resource-group redteamRG --docker-custom-image-name cyberxsecurity/project1-apachewebserver --enable-app-service-storage -t
I then customized the blog with 2 articles on cybersecurity and a link to my LinkedIn page.
The next task to complete would be to create a key vault to better secure my web app.
I then looked into a self-signed certificate vs using a trusted ssl certificate so if I choice a domain off of godaddy, then I would be ready to do so.
As I chose to go with azure they automatically proivde a trsuted certificate for their domains.
To provide a content delivery network(CDN) I created an Azure Front Door which is a modern cloud based CDN so that vistors to my web app can experience high performance and a secure environment for my users.
While there are many rules to choose from on the WAF provided with the front door, I created my own custom rule.
Creating the Key vault, verifying the trusted sll certificate, and creeating the front door were all steps needed to provided a safe, smooth functioning, and scalable web app to fit our global audience.
