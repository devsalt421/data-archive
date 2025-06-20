# data-archive

test
https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-archive
https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user
https://code.visualstudio.com/sha/download?build=stable&os=win32-x64
hello
@IF EXIST "%~dp0\..\aws-cdk\bin\cdk.js" (
  node "%~dp0\..\aws-cdk\bin\cdk.js" %*
) ELSE (
  echo "cdk.js not found"
)





