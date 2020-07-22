# Relay Workflows
This repository contains workflows for [Relay](https://relay.sh). Feel free to use these workflows to get started. If you make fixes or improvements to any of these, [send us a pull request](https://github.com/puppetlabs/relay/blob/master/CONTRIBUTING.md)! To file issues or enhancement requests for these workflows, use the [issue tracker on the main Relay repo](https://github.com/puppetlabs/relay/issues).

| Category | Workflow      | Description  | Run it! |
| ---------| --------------| ------------ | ------- |
| Cost Optimization | [Terminate EC2 instances without valid lifetime tag](./ec2-reaper) | Terminates EC2 instances not in compliance with a tagging policy: specifying a `lifetime` or `termination_date` tag. | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=ec2-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fec2-reaper%2Fec2-reaper.yaml) |
| Cost Optimization | [Delete unattached EBS volumes](./ebs-reaper) | Deletes EBS volumes that are unattached | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=ebs-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Febs-reaper%2Febs-reaper.yaml) |
| Cost Optimization | [Delete empty ELBv2 load balancers](./elbv2-delete-empty-loadbalancers) | Deletes empty ELBv2 load balancers | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=delete-empty-elbv2-loadbalancers&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Felbv2-delete-empty-loadbalancers%2Felbv2-delete-empty-loadbalancers.yaml) |
| Cost Optimization | [DynamoDB capacity monitor](./dynamodb-capacity-monitor) | Monitors DynamoDB provisioned capacity | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/development/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=dynamodb-capacity-monitor&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fdynamodb-capacity-monitor%2Fdynamodb-capacity-monitor.yaml) |
| Cost Optimization | [Delete unattached Azure Disks](./azure-disk-reaper) | Deletes Azure Disks that are unattached | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=azure-disk-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-disk-reaper%2Fazure-disk-reaper.yaml) |
| Cost Optimization | [Delete untagged Azure Virtual Machines](./azure-vm-reaper) | Deletes Azure Virtual Machines that don't have any tags | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=azure-vm-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-vm-reaper%2Fazure-vm-reaper.yaml) |
| Cost Optimization | [Delete empty Azure Load Balancers](./azure-delete-empty-loadbalancers) | Deletes empty Azure Load Balancers | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=azure-delete-empty-lbs&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-delete-empty-loadbalancers%2Fazure-delete-empty-loadbalancers.yaml) |
| Cost Optimization | [Delete unused Azure Network Interfaces](./azure-delete-unused-nics) | Deletes unused Azure Network Interfaces | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=azure-delete-unused-nics&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fazure-delete-unused-nics%2Fazure-delete-unused-nics.yaml) |
| Cost Optimization | [Delete GCP instances without valid lifetime tag](./gcp-instance-reaper) | Deletes GCP instances not in compliance with a tagging policy: specifying a `lifetime` or `termination_date` tag. | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=gcp-instance-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fgcp-instance-reaper%2Fgcp-instance-reaper.yaml) |
| Cost Optimization | [Delete unattached GCP disks](./gcp-disk-reaper) | Deletes GCP disks that are unattached | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=gcp-disk-reaper&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fgcp-disk-reaper%2Fgcp-disk-reaper.yaml) |
| Incident Response | [When a Datadog event is received, send a message to Slack](./datadog-to-slack) | Sends a message to Slack when a Datadog event is received| [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=datadog-to-slack&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fdatadog-to-slack%2Fdatadog-to-slack.yaml) |
| Incident Response | [When a Datadog event is received, create a Jira issue](./datadog-to-jira) | Creates a Jira Server issue when a Datadog event is received | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=datadog-to-jira&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fdatadog-to-jira%2Fdatadog-to-jira.yaml) |
| Incident Response | [When a PagerDuty incident is triggered, send a message to Slack](./pagerduty-to-slack) | Sends a message to Slack when a PagerDuty incident is triggered based on incident severity| [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=pagerduty-to-slack&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fpagerduty-to-slack%2Fpagerduty-to-slack.yaml) |
| Incident Response | [When a PagerDuty incident is triggered, create a Jira ticket](./pagerduty-to-jira) | Creates a Jira Server issue when a PagerDuty incident is triggered | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=pagerduty-to-jira&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fpagerduty-to-jira%2Fpagerduty-to-jira.yaml) |
| Incident Response | [When a PagerDuty incident is triggered, send an SMS via Twilio](./pagerduty-to-twilio) | Deliver a custom notification via SMS when a PagerDuty incident is triggered | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=pagerduty-to-twilio&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fpagerduty-to-twilio%2Fpagerduty-to-twilio.yaml) |
| Security | [Stop untagged EC2 instances](./ec2-stop-untagged-instances) | Stops untagged EC2 instances | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=stop-untagged-instances&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fec2-stop-untagged-instances%2Fec2-stop-untagged-instances.yaml) |
| Security | [Assume role and stop untagged EC2 instances](./sts-stop-untagged-instances) | Stops untagged EC2 instances by first assuming an IAM role with EC2 permissions | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=sts-stop-untagged-instances&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fsts-stop-untagged-instances%2Fsts-stop-untagged-instances.yaml) |
| Security | [Restrict public WRITE S3 buckets](./s3-restrict-public-write-buckets) | Finds all buckets with public 'WRITE' permissions and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-public-write-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-public-write-buckets%2Fs3-restrict-public-write-buckets.yaml) |
| Security | [Restrict public READ S3 buckets](./s3-restrict-public-read-buckets) | Finds all buckets with public 'READ' permissions and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-public-read-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-public-read-buckets%2Fs3-restrict-public-read-buckets.yaml) |
| Security | [Restrict public WRITE_ACP S3 buckets](./s3-restrict-public-write_acp-buckets) | Finds all buckets with public 'WRITE_ACP' permissions and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-public-write_acp-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-public-write_acp-buckets%2Fs3-restrict-public-write_acp-buckets.yaml) |
| Security | [Restrict public READ_ACP S3 buckets](./s3-restrict-public-read_acp-buckets) | Finds all buckets with public 'READ_ACP' permissions and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-public-read_acp-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-public-read_acp-buckets%2Fs3-restrict-public-read_acp-buckets.yaml) |
| Security | [Restrict S3 buckets with READ access to all Authenticated Users](./s3-restrict-authenticated_user-read-buckets) | Finds all buckets with 'READ' permissions to all Authenticated Users and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-authenticated_user-read-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-authenticated_user-read-buckets%2Fs3-restrict-authenticated_user-read-buckets.yaml) |
| Security | [Restrict S3 buckets with WRITE access to all Authenticated Users](./s3-restrict-authenticated_user-write-buckets) | Finds all buckets with 'WRITE' permissions to all Authenticated Users and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-authenticated_user-write-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-authenticated_user-write-buckets%2Fs3-restrict-authenticated_user-write-buckets.yaml) |
| Security | [Restrict S3 buckets with READ_ACP access to all Authenticated Users](./s3-restrict-authenticated_user-read_acp-buckets) | Finds all buckets with 'READ_ACP' permissions to all Authenticated Users and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-authenticated_user-read_acp-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-authenticated_user-read_acp-buckets%2Fs3-restrict-authenticated_user-read_acp-buckets.yaml) |
| Security | [Restrict S3 buckets with WRITE_ACP access to all Authenticated Users](./s3-restrict-authenticated_user-write_acp-buckets) | Finds all buckets with 'WRITE_ACP' permissions to all Authenticated Users and marks them `private` | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-restrict-authenticated_user-write_acp-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-restrict-authenticated_user-write_acp-buckets%2Fs3-restrict-authenticated_user-write_acp-buckets.yaml) |
| Security | [Remediate unencrypted S3 buckets](./s3-remediate-unencrypted-buckets) | Finds all unencrypted S3 buckets and encrypts them with default encryption | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=s3-remediate-unencrypted-buckets&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fs3-remediate-unencrypted-buckets%2Fs3-remediate-unencrypted-buckets.yaml) |
| Security | [Remove unused EC2 key pairs](./ec2-remove-unused-key-pairs) | Finds all unused EC2 key pairs and deletes them | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=ec2-remove-unused-key-pairs&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fec2-remove-unused-key-pairs%2Fec2-remove-unused-key-pairs.yaml) |
| Operations | [Assume role and describe EC2 objects](./sts-describe-ec2-objects) | Assumes IAM role and describes the EC2 instances, images, key pairs, and volumes in the account | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=sts-describe-ec2-objects&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fsts-describe-ec2-objects%2Fsts-describe-ec2-objects.yaml) |
| Operations | [Update other workflows on PR commit](./update-workflow-on-merge) | Enables GitOps for Relay by updating workflows stored on the service when a pull request gets merged | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=update-workflow-on-merge&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fupdate-workflow-on-merge%2Fupdate-workflow-on-merge.yaml) |
| Continuous Delivery | [Run Terraform when Pull Request merged in GitHub](./terraform-continuous-deployment) | Apply a Terraform configuration when a Pull Request is merged to a repository in GitHub. | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=terraform-continuous-deployment&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fterraform-continuous-deployment%2Fterraform-continuous-deployment.yaml) |
| Continuous Delivery | [Update Kubernetes deployment image tag on Docker Hub push](./kubectl-apply-on-dockerhub-push) | Updates a deployment image using a Docker Hub webhook to inform relay when a new Docker image is available | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=kubectl-apply-on-dockerhub-push&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fkubectl-apply-on-dockerhub-push%2Fkubectl-apply-on-dockerhub-push.yaml) |
| Continuous Delivery | [Provision an EC2 instance and configure with a Bolt plan](./ec2-provision-and-configure-with-bolt) | Uses terraform to create and provision a new EC2 instance, then uses a remote Bolt plan to configure it | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=ec2-provision-and-configure-with-bolt&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fec2-provision-and-configure-with-bolt%2Fec2-provision-and-configure-with-bolt.yaml) |
| Operations | [Restart EC2 instance on http health check](./http-health-check) | Restarts an EC2 instance your choosing when a HTTP health check does not return 200 status | [![Run with Relay](https://raw.githubusercontent.com/puppetlabs/relay-workflows/master/images/runbutton.svg)](https://app.relay.sh/create-workflow?workflowName=restart-instance-http-health-check&initialContentURL=https%3A%2F%2Fraw.githubusercontent.com%2Fpuppetlabs%2Frelay-workflows%2Fmaster%2Fhttp-health-check%2Fhttp-health-check.yaml) |
