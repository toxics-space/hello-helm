Search chart in repos
```
  helm search repo <chart_name>
  helm search repo -l 
```

Update deps of current chart ./charts - folder with charts, Chart.yaml/dependencies - current deps
```
  helm dependency update
```

Select objects managed by Helm
```
  kubectl get pods -l app.kubernetes.io/managed-by=Helm
```

Helm workflow:
```
  helm install --generate-name . --set githubRegistry.pass=<github_reg_pass>
  helm install <name> . --set githubRegistry.pass=<github_reg_pass>
  helm list
  helm uninstall <name>
```