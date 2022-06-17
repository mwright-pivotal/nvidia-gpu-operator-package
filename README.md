# nvidia-gpu-operator-package

This is a prototype for packaging Nvidia's GPU operator as a Carvel package to be used with VMwware Tanzu Kubernetes Grid or any Kubernetes distro that has kapp-controller deployed.

To learn more about Carvel tools and download, see https://carvel.dev/kapp-controller/docs/v0.34.0/packaging-tutorial/
To learn more about the NVidia GPU operator, see https://docs.nvidia.com/datacenter/cloud-native/gpu-operator/overview.html

1. kbld -f package-contents/config/ --imgpkg-lock-output package-contents/.imgpkg/images.yml
2. imgpkg push -b ${REPO_HOST}/nvidia-gpu/nvidia-gpu-operator-package:1.10.1 
