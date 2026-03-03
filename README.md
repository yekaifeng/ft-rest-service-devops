# ft-rest-service-devops
Devops manifest for ft-rest-service app

## Kustomize structure

```text
.
├── base
│   ├── deployment.yaml
│   ├── kustomization.yaml
│   ├── route.yaml
│   └── service.yaml
└── overlays
	├── dev
	│   └── kustomization.yaml
	├── prod
	│   └── kustomization.yaml
	└── sit
		└── kustomization.yaml
```

## Build manifests

- Dev: `kustomize build overlays/dev`
- Sit: `kustomize build overlays/sit`
- Prod: `kustomize build overlays/prod`

