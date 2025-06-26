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


June 26, 2025 at 11:16 (UTC+9:00)
DynamoDB 테이블 없으면 생성...
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
2025-06-26 11:16:59,158 - INFO - core.setup_dynamo - DynamoDB 테이블 설정 완료
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
2025-06-26 11:16:59,158 - INFO - root - config.production True
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Application startup complete.
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
DynamoDB 테이블 없으면 생성...
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
2025-06-26 11:16:59,155 - INFO - core.setup_dynamo - DynamoDB 테이블 설정 완료
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
2025-06-26 11:16:59,155 - INFO - root - config.production True
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Application startup complete.
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Waiting for application startup.
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
2025-06-26 11:16:58,666 - INFO - root - FastAPI 애플리케이션 시작
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Started server process [8]
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Started server process [9]
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Waiting for application startup.
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
2025-06-26 11:16:58,664 - INFO - root - FastAPI 애플리케이션 시작
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Uvicorn running on http://0.0.0.0:8000 (Press CTRL+C to quit)
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:16 (UTC+9:00)
INFO: Started parent process [1]
c923f5101624491b811b38ba48b289c2
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Waiting for child process [9]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Stopping parent process [1]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
2025-06-26 11:15:54,093 - INFO - root - FastAPI 애플리케이션 종료
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Application shutdown complete.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Finished server process [9]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Application shutdown complete.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Finished server process [8]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Waiting for application shutdown.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Waiting for application shutdown.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
2025-06-26 11:15:54,093 - INFO - root - FastAPI 애플리케이션 종료
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Shutting down
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Shutting down
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Received SIGTERM, exiting.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Terminated child process [8]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Terminated child process [9]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:15 (UTC+9:00)
INFO: Waiting for child process [8]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
2025-06-26 11:09:11,225 - INFO - core.setup_dynamo - DynamoDB 테이블 설정 완료
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
2025-06-26 11:09:11,226 - INFO - root - config.production True
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Application startup complete.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
DynamoDB 테이블 없으면 생성...
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
2025-06-26 11:09:11,224 - INFO - core.setup_dynamo - DynamoDB 테이블 설정 완료
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
2025-06-26 11:09:11,224 - INFO - root - config.production True
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Application startup complete.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
DynamoDB 테이블 없으면 생성...
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Waiting for application startup.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
2025-06-26 11:09:10,844 - INFO - root - FastAPI 애플리케이션 시작
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Started server process [9]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Started server process [8]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Waiting for application startup.
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
2025-06-26 11:09:10,733 - INFO - root - FastAPI 애플리케이션 시작
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Started parent process [1]
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:09 (UTC+9:00)
INFO: Uvicorn running on http://0.0.0.0:8000 (Press CTRL+C to quit)
8f5c8785689e41fd97ecd3e2bb38b1cb
web
June 26, 2025 at 11:07 (UTC+9:00)
2025-06-26 11:07:19,113 - INFO - root - config.production True
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Application startup complete.
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
DynamoDB 테이블 없으면 생성...
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
2025-06-26 11:07:19,113 - INFO - core.setup_dynamo - DynamoDB 테이블 설정 완료
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Application startup complete.
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
2025-06-26 11:07:19,110 - INFO - core.setup_dynamo - DynamoDB 테이블 설정 완료
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
2025-06-26 11:07:19,110 - INFO - root - config.production True
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
DynamoDB 테이블 없으면 생성...
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Started server process [9]
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Waiting for application startup.
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
2025-06-26 11:07:18,611 - INFO - root - FastAPI 애플리케이션 시작
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
2025-06-26 11:07:18,534 - INFO - root - FastAPI 애플리케이션 시작
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Started server process [8]
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Waiting for application startup.
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Uvicorn running on http://0.0.0.0:8000 (Press CTRL+C to quit)
fedc6fce2c524556996b0e00915f17d7
web
June 26, 2025 at 11:07 (UTC+9:00)
INFO: Started parent process [1]
fedc6fce2c524556996b0e00915f17d7
web



