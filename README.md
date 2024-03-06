# HarnessSDFC


**Steps:**
1. Step Template
2. DeploymentTemplate
3. Environment
4. Infra definition
5. Service
6. Pipeline

**Customise to fit:**
Depending on what scope you create your templates you will need to update/add the following to reference correctly:

- Account:
  - *templateRef: _"account.salesforce_download_artifact"_

- Organisation:
    - orgIdentifier: _Organisation-Name_
    - *templateRef: _"org.salesforce_download_artifact"_
      
- Project:
    - orgIdentifier: _Organisation-Name_
    - projectIdentofer: _Project-Name_
    - *templateRef: _"salesforce_download_artifact"_

**Documentation:**
https://developer.harness.io/docs/continuous-delivery/deploy-srv-diff-platforms/custom-deployment-tutorial/#deployment-template-sample-library
