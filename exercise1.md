If it's a Java application:  
Linting: Checkstyle, PMD, SpotBugs  
Testing: JUnit, TestNG, Mockito  
Building: Maven, Gradle, Ant  

I have used Bitbucket pipeline to set up the CI. It's quite different than Jenkins. Jenkins has a shared workspace for all the applications that requires regular clean up or the space will run out fast. while Bitbucket pipeline fires up a new container everytime, and delete the build after the pipeline finishes unless otherwise specified. Other options are: GitLab(Integrated with GitLab), Azure pipeline(Part of Azure DevOps, supports multiple languages and platforms), Bamboo(An Atlassian product that integrates well with Jira and Bitbucket).

Cloud envinronment is good for scaling up with high availability and reliability, while self-hosted environment has more control over the infrastucture, and privacy. Depending on the level of customization and flexibility needed, self-hosted solutions offer more control but require more effort to manage; cloud solution is easier to set up but less control of all the components.
Also, budge needs to be taken into account. For small to medium-sized projects, a cloud-based solution might be more cost-effective and easier to manage. For large-scale operations, a self-hosted solution might offer better control and potentially lower costs. Data privacy and security requirements also suggest different setup to ensure that the chosen solution complies with relevant regulations and standards.