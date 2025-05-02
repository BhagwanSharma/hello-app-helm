Packaging "Hello App" Application with Helm -- Helm is a package manager for Kubernetes that allows us to define, install, and upgrade applications.
Creating new Helm Chart -- helm create hello-app-chart ---cd hello-app-chart
This creates a directory structure with common files for a Helm chart
hello-app-chart/
├── .helmignore
├── Chart.yaml
├── values.yaml
├── charts/
└── templates/
    └── tests/
Review and modify the templates in the templates directory to ensure they match "Hello-App" application requirements
Redeploying Your Hello App Using Helm --> 
First, uninstall the previous deployment--then Install the Helm chart "helm install hello-app ./hello-app-chart" 
Verify the deployment --> "helm list" -- kubectl get pods -- kubectl get services
Pushing Helm Chart to GitHub --Create a new repository for Helm chart -- Package Helm chart "helm package ./hello-app-chart"
Then pushed to this current Github library
