# Spark-3.0

### What
- This repository has a single Dockerfile which builds on top of GCR image of Spark-3.0. It adds `hadoop-common`, `hadoop-aws` and `aws-java-sdk-bundle` which is required in order to use AWS as hadoop FS. Keep in mind that this is not the application image. Its the base container image and actual application jar can be different and most probably will be different

### How
- `docker build . -t spark`
- `<user_name>/spark:<tag>`
