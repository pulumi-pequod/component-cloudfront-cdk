# component-cloudfront-s3-cdk

A component that uses Pulumi's CDK interop capability to deploy CloudFront with and S3 backend using an AWS CDK construct.

# Inputs

None

# Outputs

* cloudFrontDomain: The name of the Cloud Front Domain.
* websiteBucketName: The bucket backend.

# Usage
## Specify Package in `Pulumi.yaml`

Add the following to your `Pulumi.yaml` file:
Note: If no version is specified, the latest version will be used.

```
packages:
  stackmgmt: https://github.com/pulumi-pequod/component-cloudfront-s3-cdk[@vX.Y.Z]
``` 

## Use SDK in Program

### Python
```
from pulumi_pequod_cloudfront-s3-cdk import CloudFrontS3

cloudfront_s3 = CloudFrontS3("my-cloudfront") 
```

### Typescript
```
import { CloudFrontS3 } from "@pulumi-pequod/cloudfront-s3-cdk";

const cloudfront = new CloudFrontS3();
```

### Dotnet
```
using PulumiPequod.CloudfrontS3Cdk;

var cloudFront = new CloudFrontS3("mycloudfront");
```

### YAML
```
  stacksettings:
    type: cloudfront-s3-cdk:CloudFrontS3
```




