brew install kind
kind create cluster --name fluxcd
kind get clusters

brew install derailed/k9s/k9s
brew install fluxcd/tap/flux
flux check --pre 

export GITHUB_TOKEN=

export GITHUB_USER=
 
 flux bootstrap github \           
  --owner=$GITHUB_USER \
  --repository=flux-example-jw \
  --branch=main \
  --path=deployinfra \
  --personal

  kind get clusters
  kind delete cluster fluxcd
  
