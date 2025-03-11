# component-cloudfront-s3-cdk
This is a component that uses Pulumi's CDK interop capability to deploy CloudFront with and S3 backend using an AWS CDK construct.

# Usage

In the folder of the project code that is using the component, run the following command using the release you want.
```bash
pulumi package add https://github.com/pulumi-pequod/component-cloudfront-s3-cdk@v0.1.0
```

# Example Programs
There are two test projects provided that use the component:
- Typescript (`test-project-ts`) and 
- YAML (`test-project-yaml`)

To use:
* cd to the test project folder you want to use.
* `pulumi package add https://github.com/MitchellGerdisch/component-random-abstracted@v0.1.0`
* `pulumi stack init`
* Modify the program as you want.
* `pulumi up`

