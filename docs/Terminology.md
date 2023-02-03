# Terms

[Go Home](https://github.com/jaylong255/learning-k8s)

---

>   ## Deploying Workloads

---

### Pod
- The Basic deployable unit containing one or more processes in co-located containers.

---

### ReplicaSet
- Keeps one or more pod replicas running.

---

### ReplicationController

- The older, less-powerful equivalent of a ReplicaSet.

---

### Job

- Runs pods that perform a completable task.

---

### CronJob

- Runs a scheduled job once or periodically.

---

### DaemonSet

- Runs one pod replica per node (on all nodes or only on those matching a node sector)

---

### StatefulSet

- Runs stateful pods with a stateful identity.

---

### Deployment

- Declarative deployment and updates of pods.

---

>   ## Services

---

### Service

- Exposes one or more pods at a single and stable IP address and port pair.

---

### Endpoints

- Defines which pods (or other servers) are exposed through a service.

---

### Ingress

- Exposes one or more services to external clients through a single externally reachable IP address.

---

>   ## Config

---

### ConfigMap

- A key-value map for storing non-sensitive config options for apps and exposing it to them.

---

### Secret

- Like a ConfigMap, but for sensitive data.

---

>   ## Storage

---

### PersistenceVolume

- Points to persistent storage that can be mouinted into a pod through a PersistentVolumeClaim

---

### PersistenceVolumeClaim

- A request for and claim to a PersistentVolume.

---

### StorageClass

- Defines the type of dynamically-provisioned storage claimable in a PersistentVolumeClaim.

---

>   ## Scaling

---

### HorizontalPodAutoscaler

- Automatically scales number of pod replicas based on CPU usage or another metric.

---

### PodDisruptionBudget

- Defines the minimum number of pods that must remain running when evacuating nodes.

---

>   ## Resources

---

### LimitRange

- Defines the min, max, default limits, and default requests for pods in a namespace.

---

### ResourceQuota

- Defines the amount of computational resources available to pods in the namespace.

---

>   ## Cluster State

---

### Node

- Represents a Kubernetes worker node.

---

### Cluster

- A Kubernetes cluster (used in cluster federation)

---

### ComponentStatus

- Status of a Control Plane component.

---

### Event

- A report of something that occurred in the cluster

---

>   ## Security

---

### ServiceAccount

- An account used by apps running in pods.

---

### Role

- Defines which actions a subject may perform on which resources (per namespace)

---

### ClusterRole

- Like Role, but for cluster-level resources or to grant access to resources across all namespaces.

---

### ClusterRoleBinding

- Like RoleBinding, but across all namespaces.

---

### PodSecurityPolicy

- A cluster-level resource that defines which security-sensitive features pods can use.

---

### NetworkPolicy

- Isolates the network between pods by specifying chich pods can connect to each other.

---

### CertificateSigningRequest

- A request for signing a public key certificates.

---

>   ## Ext

---

### CustomResourceDefinition

- Defines a custom resource, allowing users to create instances of the custom resource.

---
