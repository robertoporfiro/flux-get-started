# TDMI Namaspace - Custom Limit Range - k8sm-dev-aks-01

Name:       tdmi-limit-range-mem-cpu-per-container
Namespace:  tdmi
Type        Resource  Min   Max    Default Request  Default Limit  Max Limit/Request Ratio
----        --------  ---   ---    ---------------  -------------  -----------------------
Container   memory    10Mi  200Mi  50Mi             100Mi          -
Container   cpu       10m   1      100m             600m           -
