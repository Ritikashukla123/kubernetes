# kubernetes
MYSQL

- Create a deployment manifest for MySQL, specifying the necessary configuration like image, environment variables (such as root password and database name), and volume mounts for persistent storage.
- Create a Kubernetes Secret to store database password
- Create Persistent Volume and Persistent Volume Claim to store database permanently
- Create a service manifest for MySQL to allow other pods in the cluster to access the MySQL database.
- The MySQL service should be configured as a ClusterIP type service to provide internal access.

WordPress

- Create a deployment manifest for the WordPress application, specifying the required configuration like image, environment variables (such as MySQL database details), and any additional settings.
- They should define volume mounts to persist WordPress data, such as uploaded files and plugins.
- Use the same secret for mysql password that you create in previous step
- Create a service manifest for WordPress, exposing it to external traffic.
- The service should be configured as a LoadBalancer or NodePort type service to allow access from outside the cluster.
- They should ensure that the MySQL and WordPress pods are running and the services are correctly created.
