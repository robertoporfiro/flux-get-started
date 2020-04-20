
# TDMI - Default RBAC cluster access - k8sm-dev-aks-01

### Export Cluster Role Bindings

```sh

    $ kubectl get clusterrolebinding.rbac --all-namespaces -o yaml > clusterrolebinding.rbac.yaml

```

### Export Cluster Roles

```sh

    $ kubectl get clusterrole.rbac --all-namespaces -o yaml > clusterrole.rbac.yaml

```


### Export Role Bindings

```sh

    $ kubectl get rolebinding.rbac --all-namespaces -o yaml > rolebinding.rbac.yaml

```


### Export Roles

```sh

    $ kubectl get role.rbac --all-namespaces -o yaml > role.rbac.yaml

```


### List all current available roles (Cluster Rolebinding, Cluster Role, Role Binding and Role)

```sh

    $ kubectl get clusterrolebindings.rbac,clusterroles.rbac,rolebindings.rbac,roles.rbac --all-namespaces

```


| Cluster 	| k8sm-dev-aks-01 	|   	|   	|
|-----------------	|---------------------------------------------------------------------------------------------------------------	|-----	|---------	|
|   	| Cluster Role Binding 	|   	|   	|
| NAMESPACE 	| NAME                                                                                                 	| AGE 	| TYPE 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/aks-cluster-admin-binding                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/calico-node                                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/cluster-admin                                           	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/container-health-read-logs-global                       	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/kubernetes-dashboard                                    	| 33d 	| Custom 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/metrics-server:system:auth-delegator                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/omsagentclusterrolebinding                              	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/psp-cluster-rolebinding                                 	| 20d 	| Custom 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/sre-cluster-role-binding-admins                         	| 25m 	| Custom 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:aks-client-node-proxier                          	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:aks-client-nodes                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:aws-cloud-provider                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:azure-cloud-provider                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:azure-cloud-provider-secret-getter               	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:basic-user                                       	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:attachdetach-controller               	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:certificate-controller                	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:clusterrole-aggregation-controller    	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:cronjob-controller                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:daemon-set-controller                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:deployment-controller                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:disruption-controller                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:endpoint-controller                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:expand-controller                     	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:generic-garbage-collector             	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:horizontal-pod-autoscaler             	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:job-controller                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:namespace-controller                  	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:node-controller                       	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:persistent-volume-binder              	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:pod-garbage-collector                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:pv-protection-controller              	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:pvc-protection-controller             	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:replicaset-controller                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:replication-controller                	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:resourcequota-controller              	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:route-controller                      	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:service-account-controller            	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:service-controller                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:statefulset-controller                	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:controller:ttl-controller                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:coredns                                          	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:coredns-autoscaler                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:discovery                                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:kube-controller-manager                          	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:kube-dns                                         	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:kube-proxy                                       	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:kube-scheduler                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:metrics-server                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:node                                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:node-proxier                                     	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:persistent-volume-binding                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:public-info-viewer                               	| 20d 	| Custom 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/system:volume-scheduler                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/tdmi-cluster-role-binding-admins                        	| 23m 	| Custom 	|
| cluster-wide 	| clusterrolebinding.rbac.authorization.k8s.io/typha-cpha                                              	| 81d 	| Default 	|
|   	| Cluster Role 	|   	|   	|
| NAMESPACE 	| NAME                                                                                                          	| AGE 	| TYPE 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/admin                                                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/calico-node                                                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/cluster-admin                                                           	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/container-health-log-reader                                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/edit                                                                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/omsagent-reader                                                         	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/policy-agent                                                            	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/psp-cluster-role                                                        	| 20d 	| Custom 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/psp:privileged                                                          	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:aggregate-to-admin                                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:aggregate-to-edit                                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:aggregate-to-view                                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:auth-delegator                                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:aws-cloud-provider                                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:azure-cloud-provider                                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:azure-cloud-provider-secret-getter                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:basic-user                                                       	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:certificates.k8s.io:certificatesigningrequests:nodeclient        	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:certificates.k8s.io:certificatesigningrequests:selfnodeclient    	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:attachdetach-controller                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:certificate-controller                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:clusterrole-aggregation-controller                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:cronjob-controller                                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:daemon-set-controller                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:deployment-controller                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:disruption-controller                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:endpoint-controller                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:expand-controller                                     	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:generic-garbage-collector                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:horizontal-pod-autoscaler                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:job-controller                                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:namespace-controller                                  	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:node-controller                                       	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:persistent-volume-binder                              	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:pod-garbage-collector                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:pv-protection-controller                              	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:pvc-protection-controller                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:replicaset-controller                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:replication-controller                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:resourcequota-controller                              	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:route-controller                                      	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:service-account-controller                            	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:service-controller                                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:statefulset-controller                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:controller:ttl-controller                                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:coredns                                                          	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:coredns-autoscaler                                               	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:csi-external-attacher                                            	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:csi-external-provisioner                                         	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:discovery                                                        	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:heapster                                                         	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:kube-aggregator                                                  	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:kube-controller-manager                                          	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:kube-dns                                                         	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:kube-scheduler                                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:kubelet-api-admin                                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:metrics-server                                                   	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:node                                                             	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:node-bootstrapper                                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:node-problem-detector                                            	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:node-proxier                                                     	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:persistent-volume-provisioner                                    	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:persistent-volume-secret-operator                                	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:public-info-viewer                                               	| 20d 	| Custom 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/system:volume-scheduler                                                 	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/typha-cpha                                                              	| 81d 	| Default 	|
| cluster-wide 	| clusterrole.rbac.authorization.k8s.io/view                                                                    	| 81d 	| Default 	|
|   	| Role Binding 	|   	|   	|
| NAMESPACE       	| NAME                                                                                       	| AGE 	| TYPE 	|
| azure-policy    	| rolebinding.rbac.authorization.k8s.io/policy-agent                                         	| 81d 	| Default 	|
| kube-public     	| rolebinding.rbac.authorization.k8s.io/system:controller:bootstrap-signer                   	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/default:privileged                                   	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/kubernetes-dashboard-minimal                         	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/metrics-server-auth-reader                           	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/node-view                                            	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/system::extension-apiserver-authentication-reader    	| 20d 	| Custom 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/system::leader-locking-kube-controller-manager       	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/system::leader-locking-kube-scheduler                	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/system:controller:bootstrap-signer                   	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/system:controller:cloud-provider                     	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/system:controller:token-cleaner                      	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/tunnelfront                                          	| 81d 	| Default 	|
| kube-system     	| rolebinding.rbac.authorization.k8s.io/typha-cpha                                           	| 81d 	| Default 	|
| tdmi            	| rolebinding.rbac.authorization.k8s.io/psp-cluster-rolebinding                              	| 20d 	| Custom 	|
|   	| Role 	|   	|   	|
| NAMESPACE      	| NAME                                                                             	| AGE 	| TYPE 	|
| kube-public    	| role.rbac.authorization.k8s.io/system:controller:bootstrap-signer                	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/extension-apiserver-authentication-reader         	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/kubernetes-dashboard-minimal                      	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/system::leader-locking-kube-controller-manager    	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/system::leader-locking-kube-scheduler             	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/system:controller:bootstrap-signer                	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/system:controller:cloud-provider                  	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/system:controller:token-cleaner                   	| 81d 	| Default 	|
| kube-system    	| role.rbac.authorization.k8s.io/typha-cpha                                        	| 81d 	| Default 	|
