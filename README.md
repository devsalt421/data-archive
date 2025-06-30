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

https://lgu-workagent-word-templates-5232.s3.amazonaws.com/reports/test-session-id-123.docx?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=ASIAXTUTIQP3BFJFNM4G%2F20250630%2Fap-northeast-2%2Fs3%2Faws4_request&X-Amz-Date=20250630T134952Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEMb%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaDmFwLW5vcnRoZWFzdC0yIkcwRQIgfWTnCBrJHMJ9BNACYzT6feVoGBjzyxmHm5%2FRuQSbCCgCIQC7RvCuhhX%2BF%2BVgy86%2FbikoyJZRsV8iBi3omRdtVrD1HiqRAwi%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAAaDDUyMzIyMTEwNzcwMiIM5pbuaO37MSoF5%2BsHKuUCoFGeRuYbj8j%2BUgdW4qL780LR66Oj%2B0K%2FbEzUQ5FiSRvexHvVg73nAiQGrmpTl4wUc3lpN%2Bqwf5i2kS3a%2BImcaSI%2FEuYQQ8rwOs%2FroBKEMEDo1FWX0rUhQwNrBfLwiN%2BnRqETdsT43LSAzmjYQIrQz0kvO5vw6ZCPCX7%2BIAENbxadG9BETFCbw1bdnxMS5ZF9j5JRhXBEQIICi7UMLAdStb9PMMhofHmYGuOkGrYnHwkDYWgrGU%2BTXRiajjqSBe29K0ZeAPBEAYNF4eR6g27ORjbUQgmzuKz%2FsUiPp2JvRteBrIgmMwq7utU0oQiJW304cNkNWSG7JQ0YT7gniDTXptOfDAE5AG9WLKUVhmyJYVDNWRC5WyOoyya9dtNOwt2E3Bv6x8Wce3KRTZ3V%2BwIjHdM3uNqS7GYFBdJwJjvLLIVgy9Jh9uK40e2Aap0MyfpkRGSznhVDEOFKzvNuQ%2B%2FU8Kd159QiMPqqisMGOp0BxdBlepKAoxpU1ik9vttrhZam8wU%2BsfAyS7GeRfB03GOqS6zmfAiJDONOglgZ6z1YbK3ZBqP7qMWL%2BHrz1G3kS62eDMeyZr67gV3Xv495p0PtYTSKmp%2FBesB%2BqcAjuy%2FCTx2v%2FW9sPPa4u4hnD0ymw02waKDP5F07VVBUoKeSkC9LJKhqTUxYk06zp6lTQgXEbD2UgoH92WLBZGXhLw%3D%3D&X-Amz-Signature=7190e9f93e67262885aa637d3ad4f88ab36a6d50daa3dde2e11ccabdcf308cf6



