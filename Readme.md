generate token from settings , near profile 

export GITHUB_TOKEN=<your-token>
export GITHUB_USER=<your-username>

flux check --pre


ex: flux bootstrap github \\
  --owner=$GITHUB_USER \\
  --repository=flux-example \\
  --branch=main \\
  --path=./clusters/my-cluster   or env name (ca-dev) \\
  --personal
  
  ----real----

flux bootstrap github \
  --owner=$GITHUB_USER \
  --repository=fluxtesting \
  --branch=main \
  --path=./clusters/docker-desktop \
  --personal
  
  
  kubectl get all -n flux-system 
