#  This command gives the application controller service account admin privileges in the httpd-example namespace, allowing it to create and manage resources like services, deployments, and routes

oc policy add-role-to-user system:image-puller system:serviceaccount:openshift-gitops:openshift-gitops-argocd-application-controller -n httpd-example
oc policy add-role-to-user system:image-builder system:serviceaccount:openshift-gitops:openshift-gitops-argocd-application-controller -n httpd-example


