# Hands On

## Create a cluster

```bash

```bash
kind create cluster --name k8s-workshop
```

## Check Kube Config

```bash
k config get-contexts
```

## Check Current Context

```bash
k config view
```

## Create a deployment

```bash
k apply -f hello-world-deployment.yaml
```

## View Pods

```bash
k get pods -A
```

## View Pod Details

```bash
k describe pod <pod-name>
```

## View Logs

```bash
k logs <pod-name>
```

## Delete Deployment

```bash
k get deployments
k delete deployment hello-world
```

## Deploy Nginx

```bash
k apply -f nginx-service.yaml
```

## Curl Nginx Deployment

```bash
curl <ip-address>
```

## Deploy As Service

```bash
k apply -f nginx-service.yaml
```

## Get Service

```bash
k get svc
```

## Forward Port

```bash
k port-forward service/nginx 5000:8080
```

## Curl Nginx Service

```bash
curl localhost:5000
```