CI    -> CD 
build -> deploy 

## build steps

* build ( Unit Tests + Jar file generation )

* Generate Code Coverage reports and publish them to Github Pages 

* SonarQube 

* Dockerfile -> container image generation 

* push container image to conatiner regestry ( github package, DockerHub, Azure Container regestry ect)


## Deploy steps

* login to Cloud evniornment ( example Azure Az login -sp client id client secret)

* Do Helm upgrade --install passing image tag 

* verify deployment


## quick check workflows

* when ever a PR is created these workflows will run 

* check if Unit test cases are passing

* check if SornarQube quality gate checkes are passing 

* check for linting issues 

* check for any version updates ( dependabot)

* check for any vunrubilityes tools ( tool wise dependency-chec, OpenVAS  )

    # https://github.com/marketplace/actions/dependency-check


* check for Helm chart quality using Datree

* 
