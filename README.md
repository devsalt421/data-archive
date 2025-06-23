# data-archive
## Google Drive link
https://drive.google.com/file/d/파일아이디/view?usp=sharing, 
wget –no-check-certificate "https://docs.google.com/uc?export=download&id=파일아이디" -O "파일명"
---

wget --no-check-certificate "https://docs.google.com/uc?export=download&id=1Ix-NKGyZTMVs-ooVzVZ9gW2-DcO9-rgi" -O "de.z01"
wget --no-check-certificate "https://docs.google.com/uc?export=download&id=1FNnjoLBcANzjtVuhPDsiuTv-zD7MJN7C" -O "de.z02"



FILEID="1rm6YuIbOQuZfB5ZbyK1yswjjfHhps2W2"
FILENAME="cdkpack.zip"

CONFIRM=$(wget --quiet --save-cookies cookies.txt --keep-session-cookies --no-check-certificate \
  "https://docs.google.com/uc?export=download&id=${FILEID}" -O- \
  | sed -n 's/.*confirm=\(.*\)&amp;.*/\1/p')

wget --load-cookies cookies.txt \
  "https://docs.google.com/uc?export=download&confirm=${CONFIRM}&id=${FILEID}" \
  -O "${FILENAME}"

rm -f cookies.txt


$ cdk bootstrap
(node:34084) Warning: Setting the NODE_TLS_REJECT_UNAUTHORIZED environment variable to '0' makes TLS connections and HTTPS requests insecure by
 disabling certificate verification.
(Use `node --trace-warnings ...` to show where the warning was created)
 ⏳  Bootstrapping environment aws://523221107702/ap-northeast-2...
Trusted accounts for deployment: (none)
Trusted accounts for lookup: (none)
Using default execution policy of 'arn:aws:iam::aws:policy/AdministratorAccess'. Pass '--cloudformation-execution-policies' to customize.
CDKToolkit: creating CloudFormation changeset...
CDKToolkit |  0/12 | 오전 10:01:33 | REVIEW_IN_PROGRESS   | AWS::CloudFormation::Stack | CDKToolkit User Initiated
CDKToolkit |  0/12 | 오전 10:01:39 | CREATE_IN_PROGRESS   | AWS::CloudFormation::Stack | CDKToolkit User Initiated
CDKToolkit |  0/12 | 오전 10:01:41 | CREATE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  0/12 | 오전 10:01:41 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole
CDKToolkit |  0/12 | 오전 10:01:41 | CREATE_IN_PROGRESS   | AWS::S3::Bucket            | StagingBucket
CDKToolkit |  0/12 | 오전 10:01:41 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole
CDKToolkit |  0/12 | 오전 10:01:41 | CREATE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  0/12 | 오전 10:01:41 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole
CDKToolkit |  0/12 | 오전 10:01:42 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole
CDKToolkit |  0/12 | 오전 10:01:42 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole Resource creation Initiate
d
CDKToolkit |  0/12 | 오전 10:01:42 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:01:42 | CREATE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:01:42 | CREATE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:01:43 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:01:43 | CREATE_FAILED        | AWS::S3::Bucket            | StagingBucket Resource handler returned message: "cdk-
hnb659fds-assets-523221107702-ap-northeast-2 already exists (Service: S3, Status Code: 0, Request ID: null)" (RequestToken: 15f5f9e7-fd8d-d66b-
2da5-06631c897e3c, HandlerErrorCode: AlreadyExists)
CDKToolkit |  1/12 | 오전 10:01:43 | CREATE_COMPLETE      | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  2/12 | 오전 10:01:43 | CREATE_COMPLETE      | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  2/12 | 오전 10:01:43 | CREATE_FAILED        | AWS::IAM::Role             | CloudFormationExecutionRole Resource creation cancelle
 [ImagePublishingRole, FilePublishingRole, LookupRole, StagingBucket, CloudFormationExecutionRole]. Rollback requested by user.
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole
CDKToolkit |  2/12 | 오전 10:01:47 | DELETE_SKIPPED       | AWS::S3::Bucket            | StagingBucket
CDKToolkit |  2/12 | 오전 10:01:48 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole The role with name cdk-hnb659fds-cfn-exec-role-523221107702-ap-northeast-
2 cannot be found. (Service: Iam, Status Code: 404, Request ID: 0528c2c3-b0f4-497e-b9d5-dbccb9139eff) (SDK Attempt Count: 1)
CDKToolkit |  2/12 | 오전 10:01:48 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole The role with name cdk-hnb659fds-file-publishing-role-523221107702-ap-northeast-2
cannot be found. (Service: Iam, Status Code: 404, Request ID: ca3fd43d-2292-46f1-91cf-864292055bbe) (SDK Attempt Count: 1)
CDKToolkit |  2/12 | 오전 10:01:48 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole The role with name cdk-hnb659fds-lookup-role-523221107702-ap-northeast-2 cannot be found.
(Service: Iam, Status Code: 404, Request ID: a17ae843-b14f-4f51-a9d3-f91794bad8c1) (SDK Attempt Count: 1)
CDKToolkit |  1/12 | 오전 10:01:48 | DELETE_COMPLETE      | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  1/12 | 오전 10:01:48 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole The role with name cdk-hnb659fds-image-publishing-role-523221107702-ap-northeast-
2 cannot be found. (Service: Iam, Status Code: 404, Request ID: 158342e3-dc0b-417c-86ec-dbd67f3f4ca1) (SDK Attempt Count: 1)
CDKToolkit |  0/12 | 오전 10:01:48 | DELETE_COMPLETE      | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  1/12 | 오전 10:01:48 | DELETE_COMPLETE      | AWS::IAM::Role             | CloudFormationExecutionRole
CDKToolkit |  2/12 | 오전 10:01:48 | DELETE_COMPLETE      | AWS::IAM::Role             | FilePublishingRole
CDKToolkit |  3/12 | 오전 10:01:48 | DELETE_COMPLETE      | AWS::IAM::Role             | ImagePublishingRole
CDKToolkit |  4/12 | 오전 10:01:48 | DELETE_COMPLETE      | AWS::IAM::Role             | LookupRole
CDKToolkit |  5/12 | 오전 10:01:48 | ROLLBACK_COMPLETE    | AWS::CloudFormation::Stack | CDKToolkit

Failed resources:
CDKToolkit | 오전 10:01:43 | CREATE_FAILED        | AWS::S3::Bucket            | StagingBucket Resource handler returned message: "cdk-hnb659fds-assets-523221107702-ap-northeast-2 already ex
ists (Service: S3, Status Code: 0, Request ID: null)" (RequestToken: 15f5f9e7-fd8d-d66b-2da5-06631c897e3c, HandlerErrorCode: AlreadyExists)
 ❌  Environment aws://523221107702/ap-northeast-2 failed bootstrapping: _ToolkitError: The stack named CDKToolkit failed creation, it may need to be manually deleted from the AWS console: R
OLLBACK_COMPLETE: Resource handler returned message: "cdk-hnb659fds-assets-523221107702-ap-northeast-2 already exists (Service: S3, Status Code: 0, Request ID: null)" (RequestToken: 15f5f9e7
-fd8d-d66b-2da5-06631c897e3c, HandlerErrorCode: AlreadyExists)
    at FullCloudFormationDeployment.monitorDeployment (C:\Users\devdbn\my-cdk\node_modules\aws-cdk\lib\index.js:145095:17)
    at process.processTicksAndRejections (node:internal/process/task_queues:105:5)
    at async _BootstrapStack.update (C:\Users\devdbn\my-cdk\node_modules\aws-cdk\lib\index.js:146674:21)
    at async C:\Users\devdbn\my-cdk\node_modules\aws-cdk\lib\index.js:326455:29 {
  type: 'toolkit',
  source: 'toolkit',
  cause: undefined
}
The stack named CDKToolkit failed creation, it may need to be manually deleted from the AWS console: ROLLBACK_COMPLETE: Resource handler returned message: "cdk-hnb659fds-assets-523221107702-
ap-northeast-2 already exists (Service: S3, Status Code: 0, Request ID: null)" (RequestToken: 15f5f9e7-fd8d-d66b-2da5-06631c897e3c, HandlerErrorCode: AlreadyExists)


---

(node:36456) Warning: Setting the NODE_TLS_REJECT_UNAUTHORIZED environment variable to '0' makes TLS connections and HTTPS requests insecure by disabling certificate verification.
(Use `node --trace-warnings ...` to show where the warning was created)
 ⏳  Bootstrapping environment aws://523221107702/ap-northeast-2...
Trusted accounts for deployment: (none)
Trusted accounts for lookup: (none)
Using default execution policy of 'arn:aws:iam::aws:policy/AdministratorAccess'. Pass '--cloudformation-execution-policies' to customize.
CDKToolkit: creating CloudFormation changeset...
CDKToolkit |  0/12 | 오전 10:17:46 | REVIEW_IN_PROGRESS   | AWS::CloudFormation::Stack | CDKToolkit User Initiated
CDKToolkit |  0/12 | 오전 10:17:51 | CREATE_IN_PROGRESS   | AWS::CloudFormation::Stack | CDKToolkit User Initiated
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole
CDKToolkit |  0/12 | 오전 10:17:54 | CREATE_IN_PROGRESS   | AWS::S3::Bucket            | StagingBucket
CDKToolkit |  0/12 | 오전 10:17:55 | CREATE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:17:55 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:17:55 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:17:55 | CREATE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:17:55 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole Resource creation Initiated
CDKToolkit |  0/12 | 오전 10:17:56 | CREATE_IN_PROGRESS   | AWS::S3::Bucket            | StagingBucket Resource creation Initiated
CDKToolkit |  1/12 | 오전 10:17:56 | CREATE_COMPLETE      | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  2/12 | 오전 10:17:56 | CREATE_COMPLETE      | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  2/12 | 오전 10:17:56 | CREATE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole Resource creation Initiated
CDKToolkit |  2/12 | 오전 10:18:00 | CREATE_FAILED        | AWS::S3::Bucket            | StagingBucket Resource handler returned message: "User: arn:aws:sts::523221107702:assumed-role/AWSRes
ervedSSO_ps-Admin-predef_3b0aa053c0ce074d/devdbn@lgupluspartners.co.kr is not authorized to perform: s3:PutBucketPublicAccessBlock on resource: "arn:aws:s3:::cdk-hnb659fds-assets-52322110770
2-ap-northeast-2" with an explicit deny in a service control policy (Service: S3, Status Code: 403, Request ID: DBA6F8CK4KAFTEPH, Extended Request ID: OO4PD4rI0RvAXy5REpLYuF6fMSROWYiA+TYdpvP
YOk1OE/i5XLCvS9C51Y0RaMTZKe8hcg5GL5cBX/Hvqut2Y3hfIIGDvK4o53Gl9ebUGQE=) (SDK Attempt Count: 1)" (RequestToken: e414feb6-3d06-4044-bb95-b687e5c2b85f, HandlerErrorCode: GeneralServiceException)
CDKToolkit |  2/12 | 오전 10:18:00 | CREATE_FAILED        | AWS::IAM::Role             | CloudFormationExecutionRole Resource creation cancelled
CDKToolkit |  2/12 | 오전 10:18:00 | CREATE_FAILED        | AWS::IAM::Role             | LookupRole Resource creation cancelled
CDKToolkit |  2/12 | 오전 10:18:00 | CREATE_FAILED        | AWS::IAM::Role             | ImagePublishingRole Resource creation cancelled
CDKToolkit |  2/12 | 오전 10:18:00 | CREATE_FAILED        | AWS::IAM::Role             | FilePublishingRole Resource creation cancelled
CDKToolkit |  2/12 | 오전 10:18:01 | ROLLBACK_IN_PROGRESS | AWS::CloudFormation::Stack | CDKToolkit The following resource(s) failed to create: [ImagePublishingRole, FilePublishingRole, Look
upRole, StagingBucket, CloudFormationExecutionRole]. Rollback requested by user.
CDKToolkit |  2/12 | 오전 10:18:08 | DELETE_IN_PROGRESS   | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  2/12 | 오전 10:18:08 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | ImagePublishingRole
CDKToolkit |  2/12 | 오전 10:18:08 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | CloudFormationExecutionRole
CDKToolkit |  2/12 | 오전 10:18:08 | DELETE_IN_PROGRESS   | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  2/12 | 오전 10:18:08 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | LookupRole
CDKToolkit |  2/12 | 오전 10:18:09 | DELETE_IN_PROGRESS   | AWS::IAM::Role             | FilePublishingRole
CDKToolkit |  2/12 | 오전 10:18:09 | DELETE_SKIPPED       | AWS::S3::Bucket            | StagingBucket
CDKToolkit |  1/12 | 오전 10:18:09 | DELETE_COMPLETE      | AWS::ECR::Repository       | ContainerAssetsRepository
CDKToolkit |  0/12 | 오전 10:18:09 | DELETE_COMPLETE      | AWS::SSM::Parameter        | CdkBootstrapVersion
CDKToolkit |  1/12 | 오전 10:18:21 | DELETE_COMPLETE      | AWS::IAM::Role             | ImagePublishingRole
CDKToolkit |  2/12 | 오전 10:18:21 | DELETE_COMPLETE      | AWS::IAM::Role             | CloudFormationExecutionRole
CDKToolkit |  3/12 | 오전 10:18:21 | DELETE_COMPLETE      | AWS::IAM::Role             | LookupRole
CDKToolkit |  4/12 | 오전 10:18:25 | DELETE_COMPLETE      | AWS::IAM::Role             | FilePublishingRole
CDKToolkit |  5/12 | 오전 10:18:26 | ROLLBACK_COMPLETE    | AWS::CloudFormation::Stack | CDKToolkit

Failed resources:
CDKToolkit | 오전 10:18:00 | CREATE_FAILED        | AWS::S3::Bucket            | StagingBucket Resource handler returned message: "User: arn:aws:sts::523221107702:assumed-role/AWSReservedSSO
_ps-Admin-predef_3b0aa053c0ce074d/devdbn@lgupluspartners.co.kr is not authorized to perform: s3:PutBucketPublicAccessBlock on resource: "arn:aws:s3:::cdk-hnb659fds-assets-523221107702-ap-nor
theast-2" with an explicit deny in a service control policy (Service: S3, Status Code: 403, Request ID: DBA6F8CK4KAFTEPH, Extended Request ID: OO4PD4rI0RvAXy5REpLYuF6fMSROWYiA+TYdpvPYOk1OE/i
5XLCvS9C51Y0RaMTZKe8hcg5GL5cBX/Hvqut2Y3hfIIGDvK4o53Gl9ebUGQE=) (SDK Attempt Count: 1)" (RequestToken: e414feb6-3d06-4044-bb95-b687e5c2b85f, HandlerErrorCode: GeneralServiceException)
 ❌  Environment aws://523221107702/ap-northeast-2 failed bootstrapping: _ToolkitError: The stack named CDKToolkit failed creation, it may need to be manually deleted from the AWS console: R
OLLBACK_COMPLETE: Resource handler returned message: "User: arn:aws:sts::523221107702:assumed-role/AWSReservedSSO_ps-Admin-predef_3b0aa053c0ce074d/devdbn@lgupluspartners.co.kr is not authori
zed to perform: s3:PutBucketPublicAccessBlock on resource: "arn:aws:s3:::cdk-hnb659fds-assets-523221107702-ap-northeast-2" with an explicit deny in a service control policy (Service: S3, Sta
tus Code: 403, Request ID: DBA6F8CK4KAFTEPH, Extended Request ID: OO4PD4rI0RvAXy5REpLYuF6fMSROWYiA+TYdpvPYOk1OE/i5XLCvS9C51Y0RaMTZKe8hcg5GL5cBX/Hvqut2Y3hfIIGDvK4o53Gl9ebUGQE=) (SDK Attempt C
ount: 1)" (RequestToken: e414feb6-3d06-4044-bb95-b687e5c2b85f, HandlerErrorCode: GeneralServiceException)
    at FullCloudFormationDeployment.monitorDeployment (C:\Users\devdbn\my-cdk\node_modules\aws-cdk\lib\index.js:145095:17)
    at process.processTicksAndRejections (node:internal/process/task_queues:105:5)
    at async _BootstrapStack.update (C:\Users\devdbn\my-cdk\node_modules\aws-cdk\lib\index.js:146674:21)
    at async C:\Users\devdbn\my-cdk\node_modules\aws-cdk\lib\index.js:326455:29 {
  type: 'toolkit',
  source: 'toolkit',
  cause: undefined
}
The stack named CDKToolkit failed creation, it may need to be manually deleted from the AWS console: ROLLBACK_COMPLETE: Resource handler returned message: "User: arn:aws:sts::523221107702:as
sumed-role/AWSReservedSSO_ps-Admin-predef_3b0aa053c0ce074d/devdbn@lgupluspartners.co.kr is not authorized to perform: s3:PutBucketPublicAccessBlock on resource: "arn:aws:s3:::cdk-hnb659fds-a
ssets-523221107702-ap-northeast-2" with an explicit deny in a service control policy (Service: S3, Status Code: 403, Request ID: DBA6F8CK4KAFTEPH, Extended Request ID: OO4PD4rI0RvAXy5REpLYuF
6fMSROWYiA+TYdpvPYOk1OE/i5XLCvS9C51Y0RaMTZKe8hcg5GL5cBX/Hvqut2Y3hfIIGDvK4o53Gl9ebUGQE=) (SDK Attempt Count: 1)" (RequestToken: e414feb6-3d06-4044-bb95-b687e5c2b85f, HandlerErrorCode: General
ServiceException)


