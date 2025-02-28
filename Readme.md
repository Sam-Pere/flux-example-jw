export GITHUB_TOKEN=
export GITHUB_USER=
 
 flux bootstrap github \           
  --owner=$GITHUB_USER \
  --repository=flux-example-jw \
  --branch=main \
  --path=deployinfra \
  --personal
