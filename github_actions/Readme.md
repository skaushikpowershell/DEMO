apiVersion: v1
 # The type of workload we are creating 
kind: Service
metadata:
# Name of Service - Required
  name: justanimage
# Specific details about the Service
spec:
# Type of Service to be deployed
  type: LoadBalancer
  ports:
  - port: 8080
    targetPort: 80
  # Used to tell the Service which Pods to associate with
  selector:
    app: justanimage