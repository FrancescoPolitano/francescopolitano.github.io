# Kubernetes: Up and Running
by Kelsey Hightower, Brendan Burns, and Joe Beda

48 unrecognized

---

* Immutable container images are at the core of everything that you will build in Kubernetes.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 166-167 | Aggiunto in data domenica 24 maggio 2020 15:32:02</sup></p>

* declarative configuration is an alternative to imperative configuration, where the state of the world is defined by the execution of a series of instructions rather than a declaration of the desired state of the world.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 177-179 | Aggiunto in data domenica 24 maggio 2020 15:33:18</sup></p>

* It continuously takes actions to ensure that the current state matches the desired state. This

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 192-193 | Aggiunto in data domenica 24 maggio 2020 15:34:43</sup></p>

* The first thing to remember is that files that are removed by subsequent layers in the system are actually still present in the images;

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 441-442 | Aggiunto in data domenica 24 maggio 2020 18:13:29</sup></p>

* Remember that each layer is an independent delta from the layer below it. Every time you change a layer, it changes every layer that comes after it. Changing the preceding layers means that they need to be rebuilt, repushed, and repulled to deploy your image to development. To understand this more fully, consider two

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 447-449 | Aggiunto in data domenica 24 maggio 2020 18:13:15</sup></p>

* The official Kubernetes client is kubectl:

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 619-620 | Aggiunto in data martedì 26 maggio 2020 11:25:27</sup></p>

* You can see here the components that make up the Kubernetes cluster. The

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 638-640 | Aggiunto in data martedì 26 maggio 2020 11:28:05</sup></p>

* You can see here the components that make up the Kubernetes cluster. The controller-manager is responsible for running various controllers that regulate behavior in the cluster: for example, ensuring that all of the replicas of a service are available and healthy. The scheduler is responsible for placing different pods onto different nodes in the cluster. Finally, the etcd

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 638-642 | Aggiunto in data martedì 26 maggio 2020 11:28:27</sup></p>

* Kubernetes uses namespaces to organize objects in the cluster. You can think of each namespace as a folder that holds a set of objects.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 756-758 | Aggiunto in data martedì 26 maggio 2020 16:01:51</sup></p>

* One way to get slightly more information is to add the -o wide flag, which gives more details, on a longer

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 782-782 | Aggiunto in data martedì 26 maggio 2020 16:20:49</sup></p>

* One way to get slightly more information is to add the -o wide flag, which gives more details, on a longer line. If

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 782-782 | Aggiunto in data martedì 26 maggio 2020 16:20:54</sup></p>

* you specify the --no-headers flag, kubectl will skip the headers at the top of the human-readable table.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 785-786 | Aggiunto in data martedì 26 maggio 2020 16:39:51</sup></p>

* Objects in the Kubernetes API are represented as JSON or YAML files.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 793-797 | Aggiunto in data martedì 26 maggio 2020 17:19:27</sup></p>

* Labels and annotations are tags for your objects.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 815-817 | Aggiunto in data martedì 26 maggio 2020 17:23:04</sup></p>

* By default, label and annotate will not let you overwrite an existing label. To do this, you need to add the --overwrite flag.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 822-824 | Aggiunto in data martedì 26 maggio 2020 17:25:00</sup></p>

* you want to remove a label, you can use the -<label-name> syntax: $ kubectl label pods bar color-

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 824-825 | Aggiunto in data martedì 26 maggio 2020 17:25:16</sup></p>

* You can also use the exec command to execute a command in a running container: $ kubectl exec -it <pod-name> -- bash

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 836-838 | Aggiunto in data martedì 26 maggio 2020 17:25:52</sup></p>

* Finally, you can copy files to and from a container using the cp command: $ kubectl cp <pod-name>:/path/to/remote/file /path/to/local/file This will copy a file from a running container to your local machine.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 839-842 | Aggiunto in data martedì 26 maggio 2020 17:34:58</sup></p>

* Pods, not containers, are the smallest deployable artifact in a Kubernetes cluster.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 866-867 | Aggiunto in data mercoledì 27 maggio 2020 15:03:58</sup></p>

* Applications running in the same Pod share the same IP address and port space (network namespace), have the same hostname (UTS namespace), and can communicate using native interprocess communication channels over System V IPC or POSIX message queues

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 868-870 | Aggiunto in data mercoledì 27 maggio 2020 15:04:35</sup></p>

* By default, the kubectl command-line tool tries to be concise in the information it reports, but you can get more information via command-line flags. Adding -o wide to any kubectl command will print out slightly more information (while still trying to keep the information to a single line). Adding -o json or -o yaml will print out the complete objects in JSON or YAML, respectively.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 948-952 | Aggiunto in data mercoledì 27 maggio 2020 16:11:13</sup></p>

* CPU requests are implemented using the cpu-shares functionality in the Linux kernel.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1131-1132 | Aggiunto in data mercoledì 27 maggio 2020 18:06:40</sup></p>

* If a container is over its memory request, the OS can’t just remove memory from the process, because it’s been allocated. Consequently,

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1133-1134 | Aggiunto in data mercoledì 27 maggio 2020 18:07:20</sup></p>

* when the system runs out of memory, the kubelet terminates containers whose memory usage is greater than their requested memory.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1134-1135 | Aggiunto in data mercoledì 27 maggio 2020 18:07:11</sup></p>

* hostPath volume, which can mount arbitrary locations on the worker node into the container.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1196-1197 | Aggiunto in data mercoledì 27 maggio 2020 18:24:05</sup></p>

* You can organize, mark, and cross-index all of your resources to represent the groups that make the most sense for your application.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1244-1245 | Aggiunto in data mercoledì 27 maggio 2020 18:33:35</sup></p>

* Labels provide identifying metadata for objects.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1249-1250 | Aggiunto in data mercoledì 27 maggio 2020 18:34:16</sup></p>

* Labels have simple syntax. They are key/value pairs where both the key and value are represented by strings.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1259-1259 | Aggiunto in data mercoledì 27 maggio 2020 18:34:58</sup></p>

* There is a caveat to be aware of here. In this example, the kubectl label command will only change the label on the deployment itself; it won’t affect the objects (ReplicaSets and Pods) the deployment creates. To change those, you’ll need to change the template embedded in the deployment (see Chapter 12).

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1296-1299 | Aggiunto in data mercoledì 27 maggio 2020 18:36:32</sup></p>

* You can remove a label by applying a dash suffix: $ kubectl label deployments alpaca-test "canary-"

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1305-1306 | Aggiunto in data mercoledì 27 maggio 2020 18:37:30</sup></p>

* kubectl get endpoints alpaca-prod --watch

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1506-1506 | Aggiunto in data sabato 30 maggio 2020 12:31:55</sup></p>

* Reconciliation Loops The central concept behind a reconciliation loop is the notion of desired state and observed or current state. Desired state is the state you want.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1687-1691 | Aggiunto in data sabato 30 maggio 2020 13:18:19</sup></p>

* Though ReplicaSets create and manage Pods, they do not own the Pods they create.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1705-1705 | Aggiunto in data domenica 7 giugno 2020 11:05:09</sup></p>

* They then use the exact same Pod API that you used directly in Chapter 5 to create the Pods that they are managing.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1706-1707 | Aggiunto in data domenica 7 giugno 2020 11:05:16</sup></p>

* Instead, you can modify the set of labels on the

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1724-1725 | Aggiunto in data domenica 7 giugno 2020 11:29:11</sup></p>

* sick Pod. Doing so will disassociate it from the ReplicaSet (and service) so that you can debug the Pod.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1725-1725 | Aggiunto in data domenica 7 giugno 2020 11:29:18</sup></p>

* ReplicaSets are designed to represent a single, scalable microservice inside your architecture.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1730-1731 | Aggiunto in data domenica 7 giugno 2020 11:37:06</sup></p>

* The key characteristic of ReplicaSets is that every Pod that is created by the ReplicaSet controller is entirely homogeneous. Typically, these Pods are then fronted by a Kubernetes service load balancer, which spreads traffic across the Pods that make up the service. Generally speaking, ReplicaSets are designed for stateless (or nearly stateless) services. The elements created by the ReplicaSet are interchangeable; when a ReplicaSet is scaled down, an arbitrary Pod is selected for deletion. Your application’s behavior shouldn’t change because of such a scale-down operation.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1731-1735 | Aggiunto in data domenica 7 giugno 2020 11:37:41</sup></p>

* The Pods are created using a Pod template that is contained in the ReplicaSet specification.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1750-1751 | Aggiunto in data domenica 7 giugno 2020 11:57:28</sup></p>

* For example, with a web server like nginx, you may want to scale due to CPU usage. For an in-memory cache, you may want to scale with memory consumption.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1853-1854 | Aggiunto in data domenica 7 giugno 2020 12:36:26</sup></p>

* Because of the decoupled nature of Kubernetes, there is no direct link between the horizontal pod autoscaler and the ReplicaSet. While this is great for modularity and composition, it also enables some antipatterns. In particular, it’s a bad idea to combine both autoscaling and imperative or declarative management of the number of replicas. If both you and an autoscaler are attempting to modify the number of replicas, it’s highly likely that you will clash, resulting in unexpected behavior.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1881-1885 | Aggiunto in data domenica 7 giugno 2020 12:39:12</sup></p>

* direct link between the horizontal pod autoscaler and the

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1882-1882 | Aggiunto in data domenica 7 giugno 2020 12:38:43</sup></p>

* you don’t want to delete the Pods that are being managed by the ReplicaSet you can set the --cascade flag to false to ensure only the ReplicaSet object is deleted and not the Pods:

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1892-1894 | Aggiunto in data domenica 7 giugno 2020 12:39:45</sup></p>

* Another reason to replicate a set of Pods is to schedule a single Pod on every node within the cluster. Generally,

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1903-1904 | Aggiunto in data domenica 7 giugno 2020 14:38:06</sup></p>

* A DaemonSet ensures a copy of a Pod is running across a set of nodes in a Kubernetes cluster.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1905-1905 | Aggiunto in data domenica 7 giugno 2020 14:38:17</sup></p>

* daemons such as log collectors and monitoring agents,

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1906-1906 | Aggiunto in data domenica 7 giugno 2020 14:38:27</sup></p>

* reconciliation control loop that measures the desired state (a Pod is present on all nodes)

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1918-1919 | Aggiunto in data domenica 7 giugno 2020 15:12:53</sup></p>

* Kubernetes uses a decoupled approach where Pods are top-level objects. This means that every tool you have learned for introspecting Pods in the context of ReplicaSets (e.g., kubectl logs <pod-name>) is equally applicable to Pods created by DaemonSets.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1925-1927 | Aggiunto in data domenica 7 giugno 2020 15:13:44</sup></p>

