# github-action-example-node
a simple cicd pipeline (docker) build on github actions for a node-express app

On every push, perform these actions in order.

- git clone
- npm install
- npm lint
- npm test
- build the docker image
- login to docker hub
  - using the secrets which are passed as env vars, Settings -> Secrets in gh.
- push the image to docker hub

.github/workflows/push.yml defines this workflow.
