## Exercise 12 - Service Isolation Using Mixer

This has not been tested with Istio 1.2.5!  Mixer has changed with recent versions of Istio and this might be out of date!

#### Service Isolation Using Mixer

We'll block access to the Guestbook Service by adding the `deny-guestbook-service.yaml` rule shown below.

```sh
kubectl apply -f istio/deny-guestbook-service.yaml
```

Visit Guestbook UI and see that Guestbook Service can no longer be accessed.

To remove denial, you can delete the rule.

```sh
kubectl delete -f istio/deny-guestbook-service.yaml
```

#### [Continue to Exercise 13 - Istio Mutual TLS](../exercise-13/README.md)
