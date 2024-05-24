### pre
- install helm chart
- git clone code
### install opentelemetry collector
- cd hackaton/opentelemetry-helm-charts/charts/opentelemetry-collector/
- run command
  ```
  helm install opentelemetry-collector  .\
   --set image.repository="otel/opentelemetry-collector-k8s" \
   --set mode=daemonset \
   --set service.enabled=true
  ```
  ### install prometheus
  - cd hackaton/prometheus/
  - run command
    ```
      kubectl apply -k .
    ```
  ### install grafana
  -  cd hackaton/grafana/
  -  run command
   ```
   kubectl apply -k .
   ```
