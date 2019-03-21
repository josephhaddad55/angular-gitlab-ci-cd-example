# Angular GitLab CI/CD Example Project

I've generated this project with the [Angular CLI](https://github.com/angular/angular-cli) version 7.1.0. I've also added the `appsepc.yml` and `.gitlab-ci.yml` files necessary to start building a simple automated CI/CD pipeline from GitLab to AWS EC2.

**Remember to change the name of the path to the files in `.gitlab-ci.yml` since you're group and project name will be different than mine.**

Follow this tutorial to get started [Simple Angular CI/CD pipeline with GitLab & AWS](https://joeonsoftware.com/2018/12/03/simple-angular-ci-cd-pipeline-with-gitlab-aws/)

On a high level the process will look like this:

1. Push changes to the master branch

2. GitLab will detect changes and start building the production bundle (via the instructions in `.gitlab-ci.yml`)

3. Once done building GitLab will push the build artifact to AWS S3

4. AWS CodeDeploy will detect a change in the S3 Bucket and deploy the build artifact (via the instructions in `.appsepc.yml`)

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.
