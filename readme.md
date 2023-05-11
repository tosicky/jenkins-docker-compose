## How to setup jenkins agent guide
Please reference [here](https://www.cloudbees.com/blog/how-to-install-and-run-jenkins-with-docker-compose) for how setup docker agent for jenkins docker-compose

### Setup and Add the Jenkins Agent to the Jenkins Master
1. Go to your Jenkins dashboard;
1. Go to Manage Jenkins option in main menu;
1. Go to Manage Nodes and clouds item;
1. Go to New Node option in side menu;
1. Fill the Node/agent name and select the type; (e.g. Name: jenkins_agent, Type: Permanent Agent)
1. Now fill the fields:

  * Remote root directory; (e.g.: /home/jenkins )

  * label; (set the label to -> jenkins_agent )

  * usage; ( only build jobs with label expression…​)

  * Launch method; ( Launch agents by SSH )

  * Host; ( jenkins-agent )

  * Credentials; ( jenkins )

  * Host Key verification Strategy; ( Manually trusted key verification …​ )

  * Click on the Advanced field, set `Port to 22`, set JavaPath to `/opt/java/openjdk/bin/java`

1. Press the Save button and the agent1 will be registered, but offline for the time being. Click on it to see the launch process is successful.
![image](https://github.com/tosicky/consume-rest-api-java/assets/14918937/68307d60-3475-4979-98a6-d4ff1f607de9)
