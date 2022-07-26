# Creating a Git repository


Set up a Git repository to store the devfile stacks to package into the devfile registry.

**Procedure**

1. Fork the link:https://github.com/devfile/registry[devfile/registry] repository.
1. Name your forked repository.
1. Add or remove any stacks you need from this repository.
1. Create a `stacks/` directory for storing the devfile stacks. Each directory under `stacks/` must correspond to a specific stack, for example, `stacks/java-wildfly/`.
1. To package any external devfile stacks or samples in your devfile registry, go to the root of your repository and create an `extraDevfileEntries.yaml` file.
1. Add your devfile stacks to your `stacks/` directory.
1. Verify every devfile stack contains at least one `devfile.yaml` file. Add other required files to the stacks. These files can include VSX plug-ins, Dockerfiles, or Kubernetes manifests.

The registry build tool automatically validates your customized registry.

[role="_additional-resources"]
.Additional resources

* Example of link:https://github.com/devfile/registry/blob/main/extraDevfileEntries.yaml[extraDevfileEntries.yaml].
* To create devfile stacks, see xref:creating-a-devfile-stack.adoc[].
