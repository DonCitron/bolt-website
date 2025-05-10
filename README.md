# filepath: /workspaces/bolt-website/.gitlab-ci.yml
pages:
  stage: deploy
  script:
    - mkdir .public
    - cp -r * .public
  artifacts:
    paths:
      - .public
  only:
    - main

