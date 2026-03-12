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
# Encrypt
openssl aes-256-cbc -salt -in myfile.txt -out myfile.txt.enc

# Decrypt
openssl aes-256-cbc -d -in myfile.txt.enc -out myfile.txt
    commit-message:
Track all DAG / RAG task execution logs
      prefix: "docker"
    open-pull-requests-limit: 5
    labels:
      - "docker"
      - "lion-team"
airflow dags pause <dag_id>