helm/
|-- charts/
    |-- app/
    |   |-- templates/
    |   |   |-- deployment.yaml
    |   |   |-- service.yaml
    |   |   `-- ... (other resource templates)
    |   `-- values.yaml
    `-- db/
        |-- templates/
        |   |-- deployment.yaml
        |   |-- pvc.yaml
        |   |-- service.yaml
        |   `-- ... (other resource templates)
        `-- values.yaml
