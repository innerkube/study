kubectl create clusterrolebinding serviceaccounts-cluster-admin \
  --clusterrole=cluster-admin \
  --group=system:serviceaccounts


kubectl create clusterrolebinding kubernetes-dashboard-admin \
--clusterrole=cluster-admin \
--serviceaccount=kube-system:kubernetes-dashboard
