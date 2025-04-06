# ArgoCD Vault Plugin: cmp-sidecar

ArgoCD을 Helm 등으로 배포한 이후에 AVP, AVP-Helm, AVP-Kustomize 등을 추가하기 위해서는 repo-server의 메니페스트를 수정해야 합니다.

Helm으로 배포된 ArgoCD의 설정 중에서 Sidecar 컨테이너로 추가될 부분만 Patch 하기위해서 Kusomize의 `patches`을 활용하여 오버라이딩 할 수 있습니다.