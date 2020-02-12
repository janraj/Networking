# **DSR**
DSR is an implementation of asymmetric network load distribution in load balanced systems, meaning that the request and response traffic use a different network path.
The use of different network paths helps avoid extra hops and reduces the latency by which not only speeds up the response time between the client and the service but also removes some extra load from the load balancer. Using DSR is a transparent way to achieve increased network performance for your applications with little to no infrastructure changes.

## **Pros**

1. Very fast load-balancing mode
2. Load-balancer network bandwith is not a bottleneck anymore
3. Total output bandwith is the sum of each backend bandwith
4. Less intrusive than the layer 4 load-balancing NAT mode

## **Cons**

1. No layer 7 advanced features are available

## **When use this architecture?**

1. Where response time matters. Example, video streaming.
2. Where no intelligence is required
3. When output capacity of the load-balancer could be the bottleneck

## **Who should read this?**

1. Who wants DSR solution for Kubernetes platform.


## **Deploy Citrix CPX ingress controller.**

1.Download the Citrix CPX Ingress controller. 
```
wget https://raw.githubusercontent.com/citrix/citrix-k8s-ingress-controller/master/deployment/baremetal/citrix-k8s-cpx-ingress.yml
```
2. Edit the namespace.
3. Edit the ingress class 

## **Deploy the Guestbook application.**
```

```
## **Expose the guestbook application using ingress.**
```
```


 

