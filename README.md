### Notes testing on OCP v4.1

#### [Deploy Tekton Pipelines](https://github.com/tektoncd/pipeline/blob/master/docs/install.md#installing-tekton-pipelines-on-openshiftminishift) 

    oc new-project tekton-pipelines
    oc adm policy add-scc-to-user anyuid -z tekton-pipelines-controller
    oc apply -f release.yaml 
    
    ### Source file: https://storage.googleapis.com/tekton-releases/latest/release.yaml ###

#### [Pipelines Documentation](https://github.com/tektoncd/pipeline/blob/master/docs/README.md)