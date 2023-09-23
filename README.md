# Crush the CKAD Exam... on your own cluster!

When accessing the "Crush the CKAD" labs, do the following steps:

1. Clone this repository to your kubectl environment with `git clone https://github.com/csfeeser/ckad.git`
0. Each lab starts with a `drill` command and a `teardown` command, but because you are running these labs on your personal environments you'll need to do those steps differently:
    - `cd` into the Git repo you downloaded with `cd ckad`
    - Instead of using `drill api-primitives`, execute `kubectl apply -f api-primitives.yaml`
    - Instead of using `teardown api-primitives`, execute `kubectl delete -f api-primitives.yaml`
