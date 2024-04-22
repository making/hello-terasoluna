```
tanzu apps workload apply hello-terasoluna \
  --app hello-terasoluna \
  --git-repo https://github.com/making/hello-terasoluna \
  --git-branch main \
  --type web \
  --label apps.tanzu.vmware.com/has-tests=true \
  -n apps \
  --build-env BP_JVM_VERSION=17 \
  --build-env BP_TOMCAT_VERSION=10 \
  -y
```
