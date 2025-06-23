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

arn:aws:iam::523221107702:role/aws-reserved/sso.amazonaws.com/ap-northeast-2/AWSReservedSSO_ps-Admin-predef_3b0aa053c0ce074d


AdministratorAccess (Policy name)
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": "*",
            "Resource": "*"
        }
    ]
}

AwsSSOInlinePolicy
{
    "Statement": [
        {
            "Action": "aws-portal:ViewBilling*",
            "Effect": "Allow",
            "Resource": "*"
        },
        {
            "Action": "*",
            "Condition": {
                "Bool": {
                    "aws:ViaAWSService": "false"
                },
                "NotIpAddress": {
                    "aws:SourceIp": [
                        "15.164.58.36/32",
                        "52.78.134.62/32"
                    ]
                }
            },
            "Effect": "Deny",
            "Resource": "*"
        },
        {
            "Action": [
                "iam:CreateUser",
                "iam:CreateAccesskey",
                "iam:AddUserToGroup",
                "iam:CreateGroup"
            ],
            "Effect": "Deny",
            "Resource": "*"
        }
    ],
    "Version": "2012-10-17"
}



