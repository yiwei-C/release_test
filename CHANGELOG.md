# **Change Log**

This project adheres to [Semantic Versioning](http://semver.org/). Additionally, below are the change categories that may be associated with each release version.

- **Added** for new features.
- **Changed** for changes in existing functionality.
- **Deprecated** for once-stable features removed in upcoming releases.
- **Removed** for deprecated features removed in this release.
- **Fixed** for any bug fixes.
- **Security** for any security changes or fixes for vulnerabilities.

### **[Unreleased]**

### **[2.0.7] - 2017-02-02 [RELEASED]**

#### Added

*   Automated staging of release from TravisCI - [[BITE-1258](https://one-jira.pearson.com/browse/BITE-1258)]
*   Add automated versioning to TravisCI - [[BITE-1252](https://one-jira.pearson.com/browse/BITE-1252)]
*   Automated release candidate branching was added to TravisCI - [[BITE-1257](https://one-jira.pearson.com/browse/BITE-1257)]
*   Automation of Terraform TFvars for Bitesize deployment - [[BITE-1277](https://one-jira.pearson.com/browse/BITE-1277)]
*   Automate creation of Terraform TFvars via ST2 for Bitesize deployments - [[BITE-1248](https://one-jira.pearson.com/browse/BITE-1248)]

#### Changed

*   Updated terraform example for developers - [[BITE-1285](https://one-jira.pearson.com/browse/BITE-1285)]
*   Automate ingress re-deployment during cluster migration - [[BITE-1244](https://one-jira.pearson.com/browse/BITE-1244)]
*   Updated TravisCI to fail fast for failed Bitesize dependencies - [[BITE-1234](https://one-jira.pearson.com/browse/BITE-1234)]
*   Perform A/B migration validation during travisCI deployments - [[BITE-1096](https://one-jira.pearson.com/browse/BITE-1096)]
*   Set PaaS to live load balancer if it is a non-prod deployment of PaasA - [[BITE-999](https://one-jira.pearson.com/browse/BITE-999)]
*   Add ability to skip Bitesize VPC deployment if one exists - [[BITE-1243](https://one-jira.pearson.com/browse/BITE-1243)]

#### Fixed

*   Fixed failed TravisCI builds - [[BITE-1277](https://one-jira.pearson.com/browse/BITE-1277)]
*   Update bitesize-live-cluster.py script to return live cluster - [[BITE-1227](https://one-jira.pearson.com/browse/BITE-1227)]
*   Bug in bitesize tests for Ansible Branch Cloning - [[BITE-1226](https://one-jira.pearson.com/browse/BITE-1226)]
*   Update TravisCi Room ID for notifications to Hipchat - [[BITE-1222](https://one-jira.pearson.com/browse/BITE-1222)]

### **[2.0.6] - 2016-12-16 [RELEASED]**

#### Fixed

*   BTRFS issue with java oom in containers - [[BITE-1046](https://one-jira.pearson.com/browse/BITE-1046)]
*   Fix dynamic inventory in ansible_roles - [[BITE-1168](https://one-jira.pearson.com/browse/BITE-1168)]
*   Configure Pulse to get consul/vault access tokens from k8s secrets - [[BITE-1174](https://one-jira.pearson.com/browse/BITE-1174)]
*   Ensure consul container ignores invalid state pods - [[BITE-1196](https://one-jira.pearson.com/browse/BITE-1196)]
*   Update kubernetes-tests test-executor-app to have latest version of INSPEC - [[BITE-1208](https://one-jira.pearson.com/browse/BITE-1208)]
*   Handle deleting ingress configs in ingress controller - [[BITE-1209](https://one-jira.pearson.com/browse/BITE-1209)]

#### Added

*   ETCD Clean-up on Destroy - [[BITE-1111](https://one-jira.pearson.com/browse/BITE-1111)]

#### Changed

*   Remove Kubernetes root volume from from partition of docker containers. - [[BITE-1202](https://one-jira.pearson.com/browse/BITE-1202)]
*   Default resolv.conf search entry makes cross namespace resolution inefficient - [[BITE-761](https://one-jira.pearson.com/browse/BITE-761)]
*   Ensure Bastion has corp VPN endpoints whitelisted - [[COPS-283](https://one-jira.pearson.com/browse/COPS-283)]

### **[2.0.5] - 2016-11-17 [RELEASED]**

#### Fixed

*   Bump terraform version in Travis - [[BITE-1095](https://one-jira.pearson.com/browse/BITE-1095)]
*   Mongo shouldn't overwrite stanley ssh key - [[BITE-1127](https://one-jira.pearson.com/browse/BITE-1127)]
*   Unable to Terraform Apply With Existing Launch Configuration - [[BITE-1133](https://one-jira.pearson.com/browse/BITE-1133)]
*   Customer pods living on load balancers cannot access rds security group by default - [[BITE-1138](https://one-jira.pearson.com/browse/BITE-1138)]
*   Disable IPv6 on all nodes - [[COPS-266](https://one-jira.pearson.com/browse/COPS-266)]
*   Pulse STAGE - 504 Bad Gateway (Perf Testing) - [[COPS-290](https://one-jira.pearson.com/browse/COPS-290)]
*   504 Mypedia Bad Gateway - [[COPS-297](https://one-jira.pearson.com/browse/COPS-297)]
*   Pulse MYPEDIA - Mulitple faults - [[COPS-300](https://one-jira.pearson.com/browse/COPS-300)]
*   Test Container Sometimes Reports Failed Container Upon Success - [[BITE-1130](https://one-jira.pearson.com/browse/BITE-1130)]
*   Fix grafana url in terraform to add env - [[BITE-1134](https://one-jira.pearson.com/browse/BITE-1134)]
*   Fix KubeDNS Resolver Path - [[BITE-1139](https://one-jira.pearson.com/browse/BITE-1139)]
*   Jenkins disk space issue - [[COPS-141](https://one-jira.pearson.com/browse/COPS-141)]

#### Added

*   Add nfs-utils package to minions - [[BITE-1144](https://one-jira.pearson.com/browse/BITE-1144)]
*   Ability to drive consul and vault access control from outside terraform - [[BITE-562](https://one-jira.pearson.com/browse/BITE-562)]
*   Ingress Validator - [[BITE-987](https://one-jira.pearson.com/browse/BITE-987)]
*   New ubuntu/centos AMIs - [[COPS-230](https://one-jira.pearson.com/browse/COPS-230)]

#### Changed

*   User Data Scripts need to Clone and then Checkout Master by Tag - [[BITE-1059](https://one-jira.pearson.com/browse/BITE-1059)]
*   Externalize Private Keys from bitesize-test - [[BITE-1011](https://one-jira.pearson.com/browse/BITE-1011)]
*   Remove "name" from all aws_launch_configurations in terraform - [[BITE-957](https://one-jira.pearson.com/browse/BITE-957)]
*   Stackstorm self-configure vault access token - [[BITE-1142](https://one-jira.pearson.com/browse/BITE-1142)]
*   Process to migrate bastion user data from one instance to another - [[BITE-1159](https://one-jira.pearson.com/browse/BITE-1159)]
*   Add ansible inventory files for prod environments - [[BITE-1167](https://one-jira.pearson.com/browse/BITE-1167)]

### **[2.0.4] - 2016-10-26 [RELEASED]**

#### Fixed

*   Ensure consul restore restarts vault correctly - [[BITE-1074](https://one-jira.pearson.com/browse/BITE-1074)]
*   Bitesize Registry RC had Incorrect AWS S3 Tokens during Prod Release - [[BITE-1082](https://one-jira.pearson.com/browse/BITE-1082)]
*   Fix frontend LB security group - [[COPS-240](https://one-jira.pearson.com/browse/COPS-240)]

#### Added

*   Add bitesize-test clone and execution to master user-data script - [[BITE-1091](https://one-jira.pearson.com/browse/BITE-1091)]
*   Add labels to ThirdPartyResource types - [[BITE-1105](https://one-jira.pearson.com/browse/BITE-1105)]
*   Add nodeSelector: minion role to all kube-system resources - [[BITE-970](https://one-jira.pearson.com/browse/BITE-970)]
*   Create terraform.tfvars for prod deployments - [[BITE-1042](https://one-jira.pearson.com/browse/BITE-1042)]
*   Add counts to es config files - [[BITE-1081](https://one-jira.pearson.com/browse/BITE-1081)]
*   Add Test app deployment so we can have better confidence in our new releases. - [[BITE-1084](https://one-jira.pearson.com/browse/BITE-1084)]
*   Setup grafana rds isntance with yaml - [[BITE-1101](https://one-jira.pearson.com/browse/BITE-1101)]

#### Changed

*   Get rid of atlas vars from deploy example configs in terraform - [[BITE-1106](https://one-jira.pearson.com/browse/BITE-1106)]
*   Ensure the kubernetes-frontend-122-use-prod Load Balancer is persistently attached to the external_elb_sg Security Group. - [[COPS-166](https://one-jira.pearson.com/browse/COPS-166)]
*   Stackstorm rules not loaded by default - [[BITE-1094](https://one-jira.pearson.com/browse/BITE-1094)]
*   Separate consul_backups from cutover backups - [[BITE-1112](https://one-jira.pearson.com/browse/BITE-1112)]


### **[2.0.3] - 2016-10-14 [RELEASED]**

#### Fixed

*   Fix Travis CI Deployments - Still not building release branches - [[BITE-1078](https://one-jira.pearson.com/browse/BITE-1078)]

### **[2.0.2] - 2016-10-13 [RELEASED]**

#### Fixed

*   Ensure ST2 RDS deployments are region-configurable - [[BITE-1033](https://one-jira.pearson.com/browse/BITE-1033)]
*   Add curl timeout handling to bats - [[BITE-1037](https://one-jira.pearson.com/browse/BITE-1037)]
*   Fix broken setup_vault script - [[BITE-1053](https://one-jira.pearson.com/browse/BITE-1053)]
*   Update migrate_cluster st2 action to fix deployments - [[BITE-1071](https://one-jira.pearson.com/browse/BITE-1071)]
*   Fix st2 migrate_lb action to take account for all ELBs - [[BITE-1073](https://one-jira.pearson.com/browse/BITE-1073)]
*   ALERT - Pulse PROD - LB Issue - [[COPS-232](https://one-jira.pearson.com/browse/COPS-232)]
*   The builds are broken in Jenkins for all the modules. - [[COPS-239](https://one-jira.pearson.com/browse/COPS-239)]
*   Travis CI can't build branches with Dots - [[BITE-1060](https://one-jira.pearson.com/browse/BITE-1060)]
*   Test Container App Does not Run on Prod - [[BITE-1072](https://one-jira.pearson.com/browse/BITE-1072)]
*   Travis CI Still not building release branches. - [[BITE-1078](https://one-jira.pearson.com/browse/BITE-1078)]
*   ISSUE - Pulse PROD Loadbalancer - [[COPS-223](https://one-jira.pearson.com/browse/COPS-223)]

#### Added

*   Extend stackstorm to support multiple mongo versions - [[BITE-662](https://one-jira.pearson.com/browse/BITE-662)]
*   Extend stackstorm config to support multi-node cloudformation config - [[BITE-663](https://one-jira.pearson.com/browse/BITE-663)]
*   Add volume support to .bitesize files - [[BITE-995](https://one-jira.pearson.com/browse/BITE-995)]
*   GDS Pen test review and establish current status - [[BITE-1034](https://one-jira.pearson.com/browse/BITE-1034)]
*   bitesize demo - [[BITE-966](https://one-jira.pearson.com/browse/BITE-966)]
*   Deploy mongo cluster in ap-southeast-1 for pulse - [[BITE-997](https://one-jira.pearson.com/browse/BITE-997)]
*   Hosting Cost - Pulse & Reader+ - [[COPS-174](https://one-jira.pearson.com/browse/COPS-174)]
*   DEV SSL - www-aws-sin.dev.pulse.pearson.com - [[COPS-214](https://one-jira.pearson.com/browse/COPS-214)]
*   DEV SSL - api-aws-sin.dev.pulse.pearson.com - [[COPS-215](https://one-jira.pearson.com/browse/COPS-215)]
*   DEV SSL - moodle-aws-sin.dev.pulse.pearson.com - [[COPS-217](https://one-jira.pearson.com/browse/COPS-217)]
*   DEV SSL - status-aws-sin.dev.pulse.pearson.com - [[COPS-219](https://one-jira.pearson.com/browse/COPS-219)]
*   DEV SSL - admin-aws-sin.dev.pulse.pearson.com - [[COPS-220](https://one-jira.pearson.com/browse/COPS-220)]

#### Changed

*   Verify vault failover - [[BITE-851](https://one-jira.pearson.com/browse/BITE-851)]
*   Pulse uses non-expiring vault token - [[BITE-949](https://one-jira.pearson.com/browse/BITE-949)]
*   Set vault image to unseal on startup - [[BITE-1012](https://one-jira.pearson.com/browse/BITE-1012)]
*   Add Ingress check to Travis - [[BITE-1032](https://one-jira.pearson.com/browse/BITE-1032)]
*   Make ingress freeze config if vault is unavailable - [[BITE-1043](https://one-jira.pearson.com/browse/BITE-1043)]

### **[2.0.1] - 2016-10-07 [RELEASED]**

#### Fixed

*  Fix consul backup - [[BITE-1063](https://one-jira.pearson.com/browse/BITE-1063)]


#### Changed

*   Ensure rds DB config is automatically in st2 - [[BITE-1054](https://one-jira.pearson.com/browse/BITE-1054)]

### **[2.0.0] - 2016-10-04 [RELEASED]**

#### Fixed  

*   StackStorm needs to be in automated deploy through Terraform - [[BITE-592](https://one-jira.pearson.com/browse/BITE-592)]
*   Fix sysdig agent filling ingress logs with 404s - [[COPS-144](https://one-jira.pearson.com/browse/COPS-144)]
*   Need kubectl (Jenkins) to create namespace if namespace doesn't exist. - [[BITE-692](https://one-jira.pearson.com/browse/BITE-692)]
*   Consul backups stopped - [[BITE-771](https://one-jira.pearson.com/browse/BITE-771)]
*   Add target support to terraform wrapper - [[BITE-777](https://one-jira.pearson.com/browse/BITE-777)]
*   Resources Tuning: Ingress - [[BITE-791](https://one-jira.pearson.com/browse/BITE-791)]
*   Resources Tuning: Consul/Vault - [[BITE-792](https://one-jira.pearson.com/browse/BITE-792)]
*   Rotate docker container logs - [[BITE-794](https://one-jira.pearson.com/browse/BITE-794)]
*   Add pulse policies back in - [[BITE-795](https://one-jira.pearson.com/browse/BITE-795)]
*   Etcd restore process doesn't restore user namespace pods - [[BITE-798](https://one-jira.pearson.com/browse/BITE-798)]
*   Ensure All ASGs are config'd for FIFO - [[BITE-813](https://one-jira.pearson.com/browse/BITE-813)]
*   Lambda1-host-route53-shutdown function can delete wrong record - [[BITE-814](https://one-jira.pearson.com/browse/BITE-814)]
*   Roll out lambda1-host-route53-shutdown to us-west - [[BITE-815](https://one-jira.pearson.com/browse/BITE-815)]
*   Switch default TF state bucket to non-prod account - [[BITE-816](https://one-jira.pearson.com/browse/BITE-816)]
*   Workaround for bug in k8s thirdparyresource namespace - [[BITE-859](https://one-jira.pearson.com/browse/BITE-859)]
*   Hit maximum number of VPC's in AWS non-prod - [[BITE-870](https://one-jira.pearson.com/browse/BITE-870)]
*   Fix /etc/kubernetes dir to be created and cp --parent error - [[BITE-954](https://one-jira.pearson.com/browse/BITE-954)]
*   Fix nginx-ingress invalid field - [[BITE-955](https://one-jira.pearson.com/browse/BITE-955)]
*   Clean-up-route53-zone.py does not handle empty ResourceRecordSets - [[BITE-983](https://one-jira.pearson.com/browse/BITE-983)]
*   Handle alias records better in clean-up-route53-zone.py - [[BITE-984](https://one-jira.pearson.com/browse/BITE-984)]
*   Breakfix: Hashicorp http/s url change - [[BITE-1002](https://one-jira.pearson.com/browse/BITE-1002)]
*   Make A & B actions parallel in Travis - [[BITE-1003](https://one-jira.pearson.com/browse/BITE-1003)]
*   Daily build failed - [[BITE-1005](https://one-jira.pearson.com/browse/BITE-1005)]
*   Docker fails to start on bitesize EC2 instances (intermittent) - [[BITE-1006](https://one-jira.pearson.com/browse/BITE-1006)]
*   Docker fails to start on bitesize EC2 instances (intermittent) - [[BITE-1007](https://one-jira.pearson.com/browse/BITE-1007)]
*   Remove duplicate variables from terraform - [[BITE-1048](https://one-jira.pearson.com/browse/BITE-1048)]
*   Fix loadbalancers in calico setup - [[BITE-1049](https://one-jira.pearson.com/browse/BITE-1049)]
*   Mongo Errors - [[COPS-98](https://one-jira.pearson.com/browse/COPS-98)]
*   Determine why master.use-prod.kube DNS record was deleted - [[COPS-103](https://one-jira.pearson.com/browse/COPS-103)]
*   Pulse - New Relic alerts - possibly related to log export - [[COPS-135](https://one-jira.pearson.com/browse/COPS-135)]
*   Break-Fix for COPS-113, NonProd + Prod Registry Access - [[COPS-140](https://one-jira.pearson.com/browse/COPS-140)]
*   Grafana Prod Pulseauth GAB Only logs not displaying in the dashboard. - [[COPS-213](https://one-jira.pearson.com/browse/COPS-213)]
*   HTTPS is broken in Pulse - [[COPS-224](https://one-jira.pearson.com/browse/COPS-224)]


#### Added

*   Ability to specify the PaaS regions I want my application to automatically deploy into - [[BITE-116](https://one-jira.pearson.com/browse/BITE-116)]
*   Protect our keys to the private image registry from appearing plain-text in kubectl - move into Brain Vault. - [[BITE-151](https://one-jira.pearson.com/browse/BITE-151)]
*   Easily recognize what ASG launch configuration is tied to which environment - [[BITE-192](https://one-jira.pearson.com/browse/BITE-192)]
*   Basic docker image layout - [[BITE-237](https://one-jira.pearson.com/browse/BITE-237)]
*   Private docker registry to live outside of cluster. Test Google Container Registry - [[BITE-239](https://one-jira.pearson.com/browse/BITE-239)]
*   SonarQube usage - [[BITE-272](https://one-jira.pearson.com/browse/BITE-272)]
*   Approvals for deployments into upper environments - [[BITE-286](https://one-jira.pearson.com/browse/BITE-286)]
*   RBAC - [[BITE-291](https://one-jira.pearson.com/browse/BITE-291)]
*   Join an existing hipchat room - [[BITE-309](https://one-jira.pearson.com/browse/BITE-309)]
*   Ability to develop on a branch of my code independent of the other developers of my team with a consistent environment to dev and staging - [[BITE-398](https://one-jira.pearson.com/browse/BITE-398)]
*   Allow admin to modify Hubot to be capable of creating/modifying Consul ACLs - [[BITE-412](https://one-jira.pearson.com/browse/BITE-412)]
*   Add "test" action to bitesize terraform_wrapper.sh - [[BITE-427](https://one-jira.pearson.com/browse/BITE-427)]
*   StackStorm config for thirdpartyresource integration to create NFS cluster - [[BITE-432](https://one-jira.pearson.com/browse/BITE-432)]
*   DNS for apps coming onto PaaS - [[BITE-436](https://one-jira.pearson.com/browse/BITE-436)]
*   Internal CA Signing Requirements - [[BITE-437](https://one-jira.pearson.com/browse/BITE-437)]
*   Deploying Hubot into the Brain - [[BITE-439](https://one-jira.pearson.com/browse/BITE-439)]
*   Create locally clustered Consul - [[BITE-483](https://one-jira.pearson.com/browse/BITE-483)]
*   Add ability to set environment variables from Vault in .bitesize files - [[BITE-540](https://one-jira.pearson.com/browse/BITE-540)]
*   Add ability to  perform A/B releases where the B release is tested before being pushed live, not after. - [[BITE-542](https://one-jira.pearson.com/browse/BITE-542)]
*   Add ability to specify the room(s) in HipChat and/or Email address to send deployment notifications to - [[BITE-545](https://one-jira.pearson.com/browse/BITE-545)]dd
*   Introduce pod instance sizing - [[BITE-563](https://one-jira.pearson.com/browse/BITE-563)]
*   Add ability to migrate an app in production to my own cluster for testing - [[BITE-604](https://one-jira.pearson.com/browse/BITE-604)]
*   Add kubernetes actions to stackstorm pack - [[BITE-606](https://one-jira.pearson.com/browse/BITE-606)]
*   pentest - Containers Have Unrestricted Access to the Host's Docker Management Socket - [[BITE-668](https://one-jira.pearson.com/browse/BITE-668)]
*   pentest - Consul Administrative Application Account Using Weak Token - [[BITE-670](https://one-jira.pearson.com/browse/BITE-670)]
*   pentest - Insecure Sudoers Configuration - [[BITE-681](https://one-jira.pearson.com/browse/BITE-681)]
*   Set quotas by default to every namespace on create - [[BITE-695](https://one-jira.pearson.com/browse/BITE-695)]
*   Tuning Nginx Ingress - [[BITE-734](https://one-jira.pearson.com/browse/BITE-734)]
*   Registrar Certs not working for the new prsn.io domains - [[BITE-751](https://one-jira.pearson.com/browse/BITE-751)]
*   Dnsmasq or equivalent in container or namespace to lessen load on sky-dns - [[BITE-758](https://one-jira.pearson.com/browse/BITE-758)]
*   A/B deployments in pipeline - [[BITE-763](https://one-jira.pearson.com/browse/BITE-763)]
*   Investigate kubernetes-pipeline plugin - [[BITE-764](https://one-jira.pearson.com/browse/BITE-764)]
*   Create naming standard for our namespaces - [[BITE-766](https://one-jira.pearson.com/browse/BITE-766)]
*   Setup new Registrar domains with https in Staging and Prod for stg-openclass.com, stg-prsn.com, prd-prsn.com domains - [[BITE-769](https://one-jira.pearson.com/browse/BITE-769)]
*   As a paas user i must have read-only access to my docker application and base images - [[BITE-775](https://one-jira.pearson.com/browse/BITE-775)]
*   Setup Registrar domains with https in Staging for stg-openclass.com, stg-prsn.com domains - [[BITE-780](https://one-jira.pearson.com/browse/BITE-780)]
*   Automate the restore of ETCD, Consul/Vault, and associated core Kubernetes services. - [[BITE-801](https://one-jira.pearson.com/browse/BITE-801)]
*   Ensure production upgrade require no customer effort. - [[BITE-803](https://one-jira.pearson.com/browse/BITE-803)]
*   Blue/green deployment options in environments.bitesize - [[BITE-807](https://one-jira.pearson.com/browse/BITE-807)]
*   Service-manage should support bluegreen deployment - [[BITE-808](https://one-jira.pearson.com/browse/BITE-808)]
*   Deployment-pipeline-plugin must respect build promotion in bluegreen setup - [[BITE-809](https://one-jira.pearson.com/browse/BITE-809)]
*   Create reproducible client app deployment to any cluster - [[BITE-810](https://one-jira.pearson.com/browse/BITE-810)]
*   As a bitesize engineer I want to use the same AMI on both the Bitesize prod and non-prod accounts - [[BITE-820](https://one-jira.pearson.com/browse/BITE-820)]
*   Cjreate process/mechanism for migrating kube objects between arbitrary clusters - [[BITE-823](https://one-jira.pearson.com/browse/BITE-823)]
*   All Bitesize clusters should be able to access the same registry regardless of AWS account - [[BITE-825](https://one-jira.pearson.com/browse/BITE-825)]
*   As a Bitesize engineer I need a Design so that I can implement the Automated Test Framework for Bitesize - [[BITE-830](https://one-jira.pearson.com/browse/BITE-830)]
*   Push button process for migrating individual application between A and B clusters - [[BITE-832](https://one-jira.pearson.com/browse/BITE-832)]
*   Upgrade kube-dns to v18 for supporting PetSets - [[BITE-840](https://one-jira.pearson.com/browse/BITE-840)]
*   AWS limit increases on USW and EU - [[BITE-841](https://one-jira.pearson.com/browse/BITE-841)]
*   Migrate important bitbucket repos to Github - [[BITE-847](https://one-jira.pearson.com/browse/BITE-847)]
*   Use terraform's canonical format and style - [[BITE-855](https://one-jira.pearson.com/browse/BITE-855)]
*   Raise number of replicas for kube-dns - [[BITE-860](https://one-jira.pearson.com/browse/BITE-860)]
*   Create LGTM container for github review process - [[BITE-861](https://one-jira.pearson.com/browse/BITE-861)]
*   Register master's kubelet in the node API as non-schedulable - [[BITE-865](https://one-jira.pearson.com/browse/BITE-865)]
*   Setup Travis CI for Bitesize Team - [[BITE-872](https://one-jira.pearson.com/browse/BITE-872)]
*   Create initial sample unit tests for Bitesize Repo - [[BITE-873](https://one-jira.pearson.com/browse/BITE-873)]
*   Create & Deploy LGTM Docker - [[BITE-875](https://one-jira.pearson.com/browse/BITE-875)]
*   Create Stackstorm Test Framework Workflow - [[BITE-876](https://one-jira.pearson.com/browse/BITE-876)]
*   Basic kubernetes cluster tests - [[BITE-877](https://one-jira.pearson.com/browse/BITE-877)]
*   Implement a set of Inspec and Python tests to be used by the python test runner - [[BITE-878](https://one-jira.pearson.com/browse/BITE-878)]
*   Create Stackstorm Webhooks for Test Framework Workflow - [[BITE-880](https://one-jira.pearson.com/browse/BITE-880)]
*   Automated Tests: Deploy sample application to PaaS - [[BITE-882](https://one-jira.pearson.com/browse/BITE-882)]
*   Create Nessus Docker Container - [[BITE-883](https://one-jira.pearson.com/browse/BITE-883)]
*   Scan for Vulnerabilities using Nessus - [[BITE-884](https://one-jira.pearson.com/browse/BITE-884)]
*   Automated Tests: Smoke Test - [[BITE-885](https://one-jira.pearson.com/browse/BITE-885)]
*   Document 'Getting started' with Bitesize for developers - [[BITE-899](https://one-jira.pearson.com/browse/BITE-899)]
*   Wrap Ansible flipping of LBs into St2 workflow - [[BITE-900](https://one-jira.pearson.com/browse/BITE-900)]
*   Deployment pipeline: Add local apt repository to master Jenkins - [[BITE-906](https://one-jira.pearson.com/browse/BITE-906)]
*   Deployment pipeline: debian packages should use timestamps - [[BITE-907](https://one-jira.pearson.com/browse/BITE-907)]
*   Deployment pipeline: Docker images should use timestamps - [[BITE-908](https://one-jira.pearson.com/browse/BITE-908)]
*   Document Jenkins Build process - [[BITE-911](https://one-jira.pearson.com/browse/BITE-911)]
*   Get docs.prsn.io into the Jenkins build pipeline - [[BITE-912](https://one-jira.pearson.com/browse/BITE-912)]
*   Modify Bitesize Readme to add Terraform version - [[BITE-924](https://one-jira.pearson.com/browse/BITE-924)]
*   As a Bitesize engineer I need a clean-up service for AWS so that when I terraform apply/destroy fails I may clean-up unused resources in AWS - [[BITE-926](https://one-jira.pearson.com/browse/BITE-926)]
*   As a User, I would like to be able to create my own namespaces for a new project - [[BITE-933](https://one-jira.pearson.com/browse/BITE-933)]
*   As a User of Bitesize, I would like to have a log aggregation interface for all my log events. - [[BITE-934](https://one-jira.pearson.com/browse/BITE-934)]
*   A an Admin of the PaaS, I would like a proper networking solution for Bitesize - [[BITE-935](https://one-jira.pearson.com/browse/BITE-935)]
*   As a user I'd like Heapster to be updated - [[BITE-936](https://one-jira.pearson.com/browse/BITE-936)]
*   Logging: Create a fluentd container that will log to elastic search - [[BITE-938](https://one-jira.pearson.com/browse/BITE-938)]
*   Logging: Create a globally available Grafana container - [[BITE-939](https://one-jira.pearson.com/browse/BITE-939)]
*   Logging: Create a thirdpartyresource for database for Grafana storage - [[BITE-940](https://one-jira.pearson.com/browse/BITE-940)]
*   Logging: Create an Influxdb container to collect log messages - [[BITE-941](https://one-jira.pearson.com/browse/BITE-941)]
*   Logging: Create an elasticsearch cluster for Grafana - [[BITE-942](https://one-jira.pearson.com/browse/BITE-942)]
*   Increase m4.large EC2 limits to support TravisCI - [[BITE-950](https://one-jira.pearson.com/browse/BITE-950)]
*   Migrate docs site to Jenkins 3.4.21 - [[BITE-952](https://one-jira.pearson.com/browse/BITE-952)]
*   Remove SecurityContextDeny from admission control - [[BITE-953](https://one-jira.pearson.com/browse/BITE-953)]
*   Remove examples/brain from bitesize code base - [[BITE-956](https://one-jira.pearson.com/browse/BITE-956)]
*   Research: Multitenancy with nginx-controller - [[BITE-958](https://one-jira.pearson.com/browse/BITE-958)]
*   Remove Atlas from Consul cluster path - [[BITE-959](https://one-jira.pearson.com/browse/BITE-959)]
*   Add elasticsearch pack to st2 - [[BITE-963](https://one-jira.pearson.com/browse/BITE-963)]
*   Resolve TravisCI Build Issues - [[BITE-965](https://one-jira.pearson.com/browse/BITE-965)]
*   Enable Concurrent Builds in TravisCI - [[BITE-968](https://one-jira.pearson.com/browse/BITE-968)]
*   Move dev env back to hitting ansible roles 'testing' branch - [[BITE-972](https://one-jira.pearson.com/browse/BITE-972)]
*   Remove Kubernetes directory from bitesize repo - [[BITE-973](https://one-jira.pearson.com/browse/BITE-973)]
*   Remove extraneous files from ingress directory - [[BITE-974](https://one-jira.pearson.com/browse/BITE-974)]
*   Variablize CLUSTER_NAME in es data and es master rc yaml - [[BITE-977](https://one-jira.pearson.com/browse/BITE-977)]
*   Enable Hipchat notifications from TravisCI - [[BITE-979](https://one-jira.pearson.com/browse/BITE-979)]
*   Add elasticsearch deployments, upgrade version and remove hostnetwork from td-agent - [[BITE-982](https://one-jira.pearson.com/browse/BITE-982)]
*   Review HEd ILP questtionare results - [[BITE-985](https://one-jira.pearson.com/browse/BITE-985)]
*   Add bitesize questionnaire to docs.prsn.io - [[BITE-986](https://one-jira.pearson.com/browse/BITE-986)]
*   Add tdagent es yaml - [[BITE-988](https://one-jira.pearson.com/browse/BITE-988)]
*   Release Process - Define/Document Branching Strategy - [[BITE-989](https://one-jira.pearson.com/browse/BITE-989)]
*   Release Process - Enable TravisCI builds/tests for Master and ReleaseCandidate Branches - [[BITE-990](https://one-jira.pearson.com/browse/BITE-990)]
*   Release Process: Templatize Release Process Steps - [[BITE-992](https://one-jira.pearson.com/browse/BITE-992)]
*   Release Process: Complete Technical Documentation - [[BITE-993](https://one-jira.pearson.com/browse/BITE-993)]
*   Add strict validation for certain fields in .bitesize files - [[BITE-996](https://one-jira.pearson.com/browse/BITE-996)]
*   Add time key to td-agent-es.conf - [[BITE-1008](https://one-jira.pearson.com/browse/BITE-1008)]
*   Document how to use Grafana - [[BITE-1010](https://one-jira.pearson.com/browse/BITE-1010)]
*   Fix docs.prsn.io Markdown Formatting - [[BITE-1036](https://one-jira.pearson.com/browse/BITE-1036)]
*   Cascading cluster failure - [[BITE-1045](https://one-jira.pearson.com/browse/BITE-1045)]
*   Add kubernetes python v1 client to stackstorm kubernetes pack - [[BITE-698](https://one-jira.pearson.com/browse/BITE-698)]
*   Identify Bitesize Cassandra apps - [[BITE-714](https://one-jira.pearson.com/browse/BITE-714)]
*   Draft evaluation criteria - [[BITE-715](https://one-jira.pearson.com/browse/BITE-715)]
*   Initial Cassandra Kubernetes deployment - [[BITE-716](https://one-jira.pearson.com/browse/BITE-716)]
*   Investigate and define storage system requirements - [[BITE-717](https://one-jira.pearson.com/browse/BITE-717)]
*   High-level eval of Flocker - [[BITE-719](https://one-jira.pearson.com/browse/BITE-719)]
*   High-level eval of Portworx - [[BITE-720](https://one-jira.pearson.com/browse/BITE-720)]
*   High-level eval of StorageOS - [[BITE-721](https://one-jira.pearson.com/browse/BITE-721)]
*   Stand-up simple Torus PoC - [[BITE-724](https://one-jira.pearson.com/browse/BITE-724)]
*   Evaluate storage systems and propose candidates to promote to next round - [[BITE-725](https://one-jira.pearson.com/browse/BITE-725)]
*   Identify existing Cassandra provisioner for baseline analyses - [[BITE-726](https://one-jira.pearson.com/browse/BITE-726)]
*   Storage system performance tests - [[BITE-727](https://one-jira.pearson.com/browse/BITE-727)]
*   Prepare draft storage eval report - [[BITE-728](https://one-jira.pearson.com/browse/BITE-728)]
*   Create a repeatable demo (for all hands, intros etc) - [[BITE-762](https://one-jira.pearson.com/browse/BITE-762)]
*   Refactor Cloudformation/st2 scripts to remove VPC-dependency - [[BITE-805](https://one-jira.pearson.com/browse/BITE-805)]
*   Build Ceph PoC cluster - [[BITE-845](https://one-jira.pearson.com/browse/BITE-845)]
*   Validate & upgrade to stackstorm v1.5.1 - [[BITE-852](https://one-jira.pearson.com/browse/BITE-852)]
*   Create kubernetes python clients repos for v1 and v1beta1 in github.com/pearsontechnology - [[BITE-853](https://one-jira.pearson.com/browse/BITE-853)]
*   Extend stackstorm kubernetes pack to support v1 clients. - [[BITE-854](https://one-jira.pearson.com/browse/BITE-854)]
*   Build Portworx PoC cluster - [[BITE-863](https://one-jira.pearson.com/browse/BITE-863)]
*   Build Quobyte PoC cluster - [[BITE-864](https://one-jira.pearson.com/browse/BITE-864)]
*   Create a Registry Read Only Email alias - [[BITE-866](https://one-jira.pearson.com/browse/BITE-866)]
*   Create a Registry Read/Write Email Alias - [[BITE-867](https://one-jira.pearson.com/browse/BITE-867)]
*   Re-run Portworx performance - [[BITE-913](https://one-jira.pearson.com/browse/BITE-913)]
*   Extend MongoDB PetSet to replica sets - [[BITE-914](https://one-jira.pearson.com/browse/BITE-914)]
*   Release Process: Complete Dev Documentation - [[BITE-915](https://one-jira.pearson.com/browse/BITE-915)]
*   Integrate cloud-provider to EBS PV provisiong - [[BITE-916](https://one-jira.pearson.com/browse/BITE-916)]
*   Draft design approaches for persistent storage in cluster A/B - [[BITE-917](https://one-jira.pearson.com/browse/BITE-917)]
*   Deploy Pulse backed by MongoDB PetSet and persistent storage - [[BITE-918](https://one-jira.pearson.com/browse/BITE-918)]
*   Get update on stackstorm Enterprise edition - [[BITE-925](https://one-jira.pearson.com/browse/BITE-925)]
*   Stackstorm AWS pack should use IAM roles - [[BITE-931](https://one-jira.pearson.com/browse/BITE-931)]
*   Evaluate PetSet extensions to support cross-cluster migration - [[BITE-937](https://one-jira.pearson.com/browse/BITE-937)]
*   K8s 3rd Party resource config missing after prod upgrade - [[COPS-23](https://one-jira.pearson.com/browse/COPS-23)]
*   Check ETCD scripts to ensure Master pulls and restore ETCD on startup of new node PRIOR to starting ETCD - [[COPS-25](https://one-jira.pearson.com/browse/COPS-25)]
*   Minion nodes lost labels when they rejoined the new master - [[COPS-26](https://one-jira.pearson.com/browse/COPS-26)]
*   Sysdig Agent needs to start on reboot of Master - [[COPS-27](https://one-jira.pearson.com/browse/COPS-27)]
*   Subsequent terraform apply errors - [[COPS-37](https://one-jira.pearson.com/browse/COPS-37)]
*   Sysdig-agent errors on sdchecks & Consul - [[COPS-44](https://one-jira.pearson.com/browse/COPS-44)]
*   Etcd restore breaks cluster - [[COPS-45](https://one-jira.pearson.com/browse/COPS-45)]
*   Hubot created projects have bad ssh priv key embeded in RC - [[COPS-52](https://one-jira.pearson.com/browse/COPS-52)]
*   Kafka consumer sometimes get nothing from the first read - [[COPS-76](https://one-jira.pearson.com/browse/COPS-76)]
*   Slowness on remote kubectl commands - [[COPS-83](https://one-jira.pearson.com/browse/COPS-83)]
*   Research why a Restart of td-agent was required after use-prod upgrade - [[COPS-92](https://one-jira.pearson.com/browse/COPS-92)]
*   Fixed td-agent filter error - [[COPS-100](https://one-jira.pearson.com/browse/COPS-100)]
*   Td-agent return "undefined method strip with moodle-apache pods - [[COPS-102](https://one-jira.pearson.com/browse/COPS-102)]
*   Automate ELB changes - [[COPS-115](https://one-jira.pearson.com/browse/COPS-115)]
*   Moodle-php not deployed to PROD - [[COPS-143](https://one-jira.pearson.com/browse/COPS-143)]
*   Pulse STAGE - Gateway issue - [[COPS-151](https://one-jira.pearson.com/browse/COPS-151)]
*   Terraform: refactor IAM module so that policies would live next to the instances - [[COPS-155](https://one-jira.pearson.com/browse/COPS-155)]
*   As an Operations Team we need to ensure critical systems are documented and have runbooks. - [[COPS-2](https://one-jira.pearson.com/browse/COPS-2)]
*   As an Operations Team we need an easy and effective way to communicate upcoming changes and potential impacts. - [[COPS-3](https://one-jira.pearson.com/browse/COPS-3)]
*   As an Operations Team we need a standard SLA - [[COPS-4](https://one-jira.pearson.com/browse/COPS-4)]
*   As an Operations Team having insight of our customers is important - [[COPS-5](https://one-jira.pearson.com/browse/COPS-5)]
*   As we bring on new techs getting them up to speed properly is crucial. - [[COPS-6](https://one-jira.pearson.com/browse/COPS-6)]
*   As on Operations Team we need an effective way to communicate issues and outages - [[COPS-7](https://one-jira.pearson.com/browse/COPS-7)]
*   As an Operations Team we need a checklist of all needed access in order to do our job. - [[COPS-8](https://one-jira.pearson.com/browse/COPS-8)]
*   As an Operations Team we need to have better input around monitoring. - [[COPS-9](https://one-jira.pearson.com/browse/COPS-9)]
*   As a PaaS admin, I want to be sure I can safely restore etcd - [[COPS-24](https://one-jira.pearson.com/browse/COPS-24)]
*   Update td-agent pod and config in use-prod - [[COPS-29](https://one-jira.pearson.com/browse/COPS-29)]
*   As an operator of the PaaS I want a clear incident management plan to enact when we have an issue with the cluster - [[COPS-30](https://one-jira.pearson.com/browse/COPS-30)]
*   As a user I want sysdig agent to be installed when a CloudFormation template is instantiated - [[COPS-34](https://one-jira.pearson.com/browse/COPS-34)]
*   Terraform: assert dns names for all infrastructure services use cname pointing at elb - [[COPS-39](https://one-jira.pearson.com/browse/COPS-39)]
*   Hubot Regional identifier for multi-region deployments - [[COPS-40](https://one-jira.pearson.com/browse/COPS-40)]
*   Ingress Controller monitor required - [[COPS-46](https://one-jira.pearson.com/browse/COPS-46)]
*   Create Sysdig monitoring for losing Kubernetes minions/nodes - [[COPS-47](https://one-jira.pearson.com/browse/COPS-47)]
*   As a paas user i need to fetch my namespace as an environment variable from within my container - [[COPS-50](https://one-jira.pearson.com/browse/COPS-50)]
*   PasS - New release to Prod - [[COPS-61](https://one-jira.pearson.com/browse/COPS-61)]
*   Hubot - Jira - bot - [[COPS-62](https://one-jira.pearson.com/browse/COPS-62)]
*   kubeapi: rotate pod logs as part of a post-transport validation process - [[COPS-68](https://one-jira.pearson.com/browse/COPS-68)]
*   Registrar: provide 6 cassandra nodes for production - [[COPS-69](https://one-jira.pearson.com/browse/COPS-69)]
*   Mongodump: verify crontab functioning as should - [[COPS-90](https://one-jira.pearson.com/browse/COPS-90)]
*   Ensure sysdig is installed on Auth nodes. - [[COPS-95](https://one-jira.pearson.com/browse/COPS-95)]
*   nonprod/ terraform: grant account 602604727914 access to s3://bitesize-docker-registry - [[COPS-110](https://one-jira.pearson.com/browse/COPS-110)]
*   nonprod/ terraform: parameterize modules/dns/aws_route53_zone name - [[COPS-111](https://one-jira.pearson.com/browse/COPS-111)]
*   Bitesize nonprod must have access to bitesize prod registry - [[COPS-113](https://one-jira.pearson.com/browse/COPS-113)]
*   Update Prod CentOS AMI to ensure /data volume is mounted on deploy - [[COPS-114](https://one-jira.pearson.com/browse/COPS-114)]
*   Sysdig: obtain a key for nonprod instances - [[COPS-118](https://one-jira.pearson.com/browse/COPS-118)]
*   Provision Mongo in Bitesize reg-qa environment for Registrar Services - [[COPS-120](https://one-jira.pearson.com/browse/COPS-120)]
*   Provision Cassandra in Bitesize reg-qa environment for Registrar Services - [[COPS-121](https://one-jira.pearson.com/browse/COPS-121)]
*   Provision ElasticSearch node in Bitesize reg-qa environment for Registrar Services - [[COPS-122](https://one-jira.pearson.com/browse/COPS-122)]
*   Enable Nginx Status Page - [[COPS-127](https://one-jira.pearson.com/browse/COPS-127)]
*   Consume kafka logs in an efficient manner without the memory overhead - [[COPS-133](https://one-jira.pearson.com/browse/COPS-133)]
*   Lambda: log actions - sns topic or email when performing an action - [[COPS-134](https://one-jira.pearson.com/browse/COPS-134)]
*   Readerplus - DEV, TEST & STAGE environments - [[COPS-137](https://one-jira.pearson.com/browse/COPS-137)]
*   PaaS Jenkins Docker Deployment issue - [[COPS-139](https://one-jira.pearson.com/browse/COPS-139)]
*   PaaS Pulse - Possible Loadn Balancer Issue - [[COPS-142](https://one-jira.pearson.com/browse/COPS-142)]
*   Sysdig monitoring to capture total running processes per node - [[COPS-145](https://one-jira.pearson.com/browse/COPS-145)]
*   Adjust Nginx Ingress logging to discard SysDig healthcheck requests - [[COPS-146](https://one-jira.pearson.com/browse/COPS-146)]
*   Fix DNS deregistration from AutoScaling Groups - [[COPS-147](https://one-jira.pearson.com/browse/COPS-147)]
*   Registrar Services - As a user of PAAS, provision external http url with qa-prsn.io domain name just like dev for Bitesize reg-qa environment - [[COPS-150](https://one-jira.pearson.com/browse/COPS-150)]
*   Create dev-bite.io and stg-bite.io wildcard certs - [[COPS-152](https://one-jira.pearson.com/browse/COPS-152)]
*   Cloudformation.git / documentation/ operator instructions - [[COPS-156](https://one-jira.pearson.com/browse/COPS-156)]
*   Registrar Services - Add dev-prsn.com, stg-prsn.com, prd-prsn.com certs to PaaS - [[COPS-161](https://one-jira.pearson.com/browse/COPS-161)]
*   Singapore Cluster - [[COPS-164](https://one-jira.pearson.com/browse/COPS-164)]
*   Create MongoDB Dashboard for Pulse - [[COPS-173](https://one-jira.pearson.com/browse/COPS-173)]
*   Issue with Jenkins deployment - [[COPS-177](https://one-jira.pearson.com/browse/COPS-177)]
*   Jenkins - Disk Full - [[COPS-178](https://one-jira.pearson.com/browse/COPS-178)]
*   Pulse DB Mongo - Low disk space - [[COPS-181](https://one-jira.pearson.com/browse/COPS-181)]
*   Pulse MongoDB Backups - [[COPS-183](https://one-jira.pearson.com/browse/COPS-183)]
*   Document image bakery process - [[COPS-184](https://one-jira.pearson.com/browse/COPS-184)]
*   Pulse DEV TEST & STAGE Down - PROD UP - [[COPS-186](https://one-jira.pearson.com/browse/COPS-186)]
*   LB for Singapore Hub - [[COPS-187](https://one-jira.pearson.com/browse/COPS-187)]
*   Registrar Services - Add SAN certs for dev-prsn.com, stg-prsn.com, prd-prsn.com domains in Bitesize - [[COPS-189](https://one-jira.pearson.com/browse/COPS-189)]
*   Pulse Singapore Hub - Pulse Dev Web Logs - [[COPS-226](https://one-jira.pearson.com/browse/COPS-226)]
*   Vpc_peer: troubleshoot niburu prod -> bitesize bi-directional connection - [[COPS-71](https://one-jira.pearson.com/browse/COPS-71)]
*   Create mongo 2.x cluster for readerplus - [[COPS-74](https://one-jira.pearson.com/browse/COPS-74)]
*   Create 8x mongo 2.x clusters for Pulse - [[COPS-82](https://one-jira.pearson.com/browse/COPS-82)]
*   Ansible-roles/bitesize-hostname: update to reflect changes in bitesize.git/dns_fix branch - [[COPS-160](https://one-jira.pearson.com/browse/COPS-160)]

#### Changed

*   Ansible Roles for AWS user-data - [[BITE-565](https://one-jira.pearson.com/browse/BITE-565)]
*   Minimize user-data scripts - [[BITE-797](https://one-jira.pearson.com/browse/BITE-797)]
*   User-data: ansible-roles.git/ bitesize-common (kube-minion) - [[BITE-834](https://one-jira.pearson.com/browse/BITE-834)]
*   Use existing provisioning to build a Cassandra cluster - [[BITE-837](https://one-jira.pearson.com/browse/BITE-837)]
*   Share set-up and demo script for Cassandra/PX - [[BITE-838](https://one-jira.pearson.com/browse/BITE-838)]
*   Terraform/ iam: need consolidation of iam roles - [[BITE-842](https://one-jira.pearson.com/browse/BITE-842)]
*   Terraform/ iam: expansion of route53 Get*,List* contexts - [[BITE-848](https://one-jira.pearson.com/browse/BITE-848)]
*   User-data/setup_volumes.sh : add file marker so ansible can move on when it knows mount is successful - [[BITE-850](https://one-jira.pearson.com/browse/BITE-850)]
*   Refactor packer repo /tooling to pull and use ansible-roles.git - [[COPS-43](https://one-jira.pearson.com/browse/COPS-43)]
*   Import a production namespace, verify running, and document process - [[COPS-79](https://one-jira.pearson.com/browse/COPS-79)]
*   Migrate pulse-test mongo, single-instance->cluster - [[COPS-89](https://one-jira.pearson.com/browse/COPS-89)]
*   Resolve documentation gap on ingress - [[BITE-786](https://one-jira.pearson.com/browse/BITE-786)]
*   Refactor Terraform for A/B in a single VPC - [[BITE-821](https://one-jira.pearson.com/browse/BITE-821)]
*   Externalising Flannel network to support A/B deployment - [[BITE-824](https://one-jira.pearson.com/browse/BITE-824)]
*   Move etcd out of kubernetes-master - [[BITE-831](https://one-jira.pearson.com/browse/BITE-831)]
*   Make domain a variable within terraform - [[BITE-843](https://one-jira.pearson.com/browse/BITE-843)]
*   Set longer TTL for ingress tokens - [[BITE-960](https://one-jira.pearson.com/browse/BITE-960)]
*   Remove lambda functions for host-route53-shutdown - [[BITE-969](https://one-jira.pearson.com/browse/BITE-969)]
*   Unused dir in bitesize consul image - [[BITE-981](https://one-jira.pearson.com/browse/BITE-981)]
*   Vault/Consul token creation - [[BITE-1031](https://one-jira.pearson.com/browse/BITE-1031)]
*   Analyse and help with Console perf testing - [[COPS-59](https://one-jira.pearson.com/browse/COPS-59)]
*   Analyse and help with Registrar perf testing - [[COPS-60](https://one-jira.pearson.com/browse/COPS-60)]
*   Kafka instances - Expand storage  - [[COPS-65](https://one-jira.pearson.com/browse/COPS-65)]
*   Pulse team DB access - [[COPS-124](https://one-jira.pearson.com/browse/COPS-124)]
*   Monitor ingress controller - SysDig - [[COPS-126](https://one-jira.pearson.com/browse/COPS-126)]
*   Roll out logrotate for docker on use-prod - [[COPS-191](https://one-jira.pearson.com/browse/COPS-191)]

### **[1.2.0] - 2016-06-28 [RELEASED]**

- Initial Bitesize Release
