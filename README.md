## Setting up  the environment

```bash
kind create cluster 
helm install external-secrets oci://ghcr.io/external-secrets/external-secrets
```
## Creating Manifests to Explore:
```bash
kubectl apply  -f  examples/base_secretstore.yaml
kubectl apply  -f  examples/1_multiple_stores.yaml
kubectl apply  -f  examples/2_data_from.yaml
kubectl apply  -f  examples/3_decoding_strategy.yaml
kubectl apply  -f  examples/4_generators.yaml
kubectl apply  -f  examples/5_templates.yaml
kubectl apply  -f  examples/6_template_from.yaml
kubectl apply  -f  examples/7_merge_policies.yaml
kubectl apply  -f  examples/8_delete_policy.yaml
```