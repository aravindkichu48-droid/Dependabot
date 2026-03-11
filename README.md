#github/dependabot.yml:
Enable two factor authenticationUse 2fA 
version: 2
updates:
  # Python dependencies
  - package-ecosystem: "pip"
    directory: "/"  # root directory
    schedule:
      interval: "daily"
    commit-message:
      prefix: "deps"
    open-pull-requests-limit: 10
    labels:
      - "dependencies"
      - "lion-team"

  # Docker dependencies
  - package-ecosystem: "docker"
    directory: "/"
    schedule:
      interval: "weekly"
    commit-message:
      prefix: "docker"
    open-pull-requests-limit: 5
    labels:
      - "docker"
      - "lion-team"