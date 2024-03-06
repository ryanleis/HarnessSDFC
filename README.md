# HarnessSDFC


Steps:
1. Step Template
2. DeploymentTemplate
3. Environment
4. Infra definition
5. Service
6. Pipeline

Depnedning on what scope you create you templates you will need to ensure you update/add the following:

- Account:
  - *templateRef: _"account.salesforce_download_artifact"_

- Organisation:
    - orgIdentifier: _Organisation-Name_
    - *templateRef: _"org.salesforce_download_artifact"_
      
- Project:
    - orgIdentifier: _Organisation-Name_
    - projectIdentofer: _Project-Name_
    - *templateRef: _"salesforce_download_artifact"_
