# Problem je bio u "previsokoj" verziji testcontainers.com Spustio sam verziju sa 1.18.3 na 1.17.0

Sada je:

<testcontainers.version>1.17.0</testcontainers.version>

Ali smo eksplicitno definsali verziju za k3s:

<dependency>
    <groupId>org.testcontainers</groupId>
    <artifactId>k3s</artifactId>
    <version>1.18.3</version>
    <scope>test</scope>
</dependency>

# Testing with Testcontainers on k3s
As I mentioned before, there are several tools we can use for testing with Kubernetes. This time we will see how to do it with Testcomntainers. We have already used it in the previous section for running the Mongo database. But there is also the Testcontainers module for Rancher’s k3s Kubernetes distribution. Currently, it is in the incubating state, but it doesn’t bother us to try it. In order to use it in the project we need to include the following Maven dependency:

<dependency>
  <groupId>org.testcontainers</groupId>
  <artifactId>k3s</artifactId>
  <scope>test</scope>
</dependency>

