# Mythical Mysfits: DevSecOps with Docker and AWS Fargate

## Overview
![mysfits-welcome](/images/mysfits-welcome.png)

**Mythical Mysfits** is a (fictional) pet adoption non-profit dedicated to helping abandoned, and often misunderstood, mythical creatures find a new forever family! Mythical Mysfits believes that all creatures deserve a second chance, even if they spent their first chance hiding under bridges and unapologetically robbing helpless travelers.

Our business has been thriving with only a single Mysfits adoption center, located inside Devils Tower National Monument. Speak, friend, and enter should you ever come to visit.

We've just had a surge of new mysfits arrive at our door with nowhere else to go!  They're all pretty distraught after not only being driven from their homes... but an immensely grumpy ogre has also denied them all entry at a swamp they've used for refuge in the past.  

That's why we've hired you to be our first Full Stack Engineer. We need a more scalable way to show off our inventory of mysfits and let families adopt them. We'd like you to build the first Mythical Mysfits adoption website to help introduce these lovable, magical, often mischievous creatures to the world!

We're growing, but we're struggling to keep up with our new mysfits mainly due to our legacy inventory platform.  We heard about the benefits of containers, especially in the context of microservices and devsecops. We've already taken some steps in that direction, but can you help us take this to the next level? 

We've already moved to a microservice based model, but are still not able to develop quickly. We want to be able to deploy to our microservices as quickly as possible while maintaining a certain level of confidence that our code will work well. This is where you come in.

If you are not familiar with DevOps, there are multiple facets to the the word. One focuses on organizational values, such as small, well rounded agile teams focusing on owning a particular service, whereas one focuses on automating the software delivery process as much as possible to shorten the time between code check in and customers testing and providing feedback. This allows us to shorten the feedback loop and iterate based on customer requirements at a much quicker rate. 

In this workshop, you will take our Mythical stack and apply concepts of CI/CD to their environment. To do this, you will create a pipeline to automate all deployments using AWS CodeCommit or GitHub, AWS CodeBuild, AWS CodePipeline, and AWS Fargate. Today, the Mythical stack runs on AWS Fargate following a microservice architecture, meaning that there are very strict API contracts that are in place. As part of the move to a more continuous delivery model, they would like to make sure these contracts are always maintained.

The tools that we use in this workshop are part of the AWS Dev Tools stack, but are by no means an end all be all. What you should focus on is the idea of CI/CD and how you can apply it to your environments.

### What you'll do:

These labs are designed to be completed in sequence, and the full set of instructions are documented below.  Read and follow along to complete the labs.  If you're at a live AWS event, the workshop attendants will give you a high level run down of the labs and help answer any questions.  Don't worry if you get stuck, we provide hints along the way.  

* **[Lab 0](Lab-0):** Deploy Existing Mythical Stack
* **[Lab 1](Lab-1):** Integrating Security Right from the Get Go
* **[Lab 2](Lab-2):** Offloading Builds to AWS CodeBuild
* **[Lab 3](Lab-3):** Automating End to End Deployments for AWS Fargate
* **[Lab 4](Lab-4):** Moar Security! Implementing Container Image scanning

### Conventions:
Throughout this workshop, we will provide commands for you to run in the terminal.  These commands will look like this:

<pre>
$ ssh -i <b><i>PRIVATE_KEY.PEM</i></b> ec2-user@<b><i>EC2_PUBLIC_DNS_NAME</i></b>
</pre>

The command starts after the $.  Text that is ***UPPER_ITALIC_BOLD*** indicates a value that is unique to your environment.  For example, the ***PRIVATE\_KEY.PEM*** refers to the private key of an SSH key pair that you've created, and the ***EC2\_PUBLIC\_DNS\_NAME*** is a value that is specific to an EC2 instance launched in your account.  You can find these unique values either in the CloudFormation outputs or by going to the specific service dashboard in the [AWS management console](https://console.aws.amazon.com).

If you are asked to enter a specific value in a text field, the value will look like `VALUE`.

Hints are also provided along the way and will look like this:

<details>
<summary>HINT</summary>

**Nice work, you just revealed a hint!**
</details>


*Click on the arrow to show the contents of the hint.*


## Let's Begin!

[Go to Lab-0 to set up your environment](Lab-0)

