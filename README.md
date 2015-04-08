# Elastic(search) with Amazon AWS plugin

Based on the official Docker Elasticsearch image with the Amazon AWS plugin and
some configuration defaults added.
 
 * https://registry.hub.docker.com/_/elasticsearch/
 * https://github.com/elastic/elasticsearch-cloud-aws

## Usage

```
docker run --net=host \
  mikljohansson/elasticsearch-aws \
  -Des.cloud.aws.access_key=my-access-key-id \
  -Des.cloud.aws.secret_key=my-secret-access-key \
  -Des.cloud.aws.region=us-east-1 \
  -Des.discovery.ec2.availability_zones=us-east-1c \
  -Des.discovery.ec2.groups=my-security-group,another-security-group
```
