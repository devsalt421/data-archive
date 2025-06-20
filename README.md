# data-archive

test
https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-archive

hello

# Node install 
curl -O https://nodejs.org/dist/v22.16.0/node-v22.16.0-x64.msi



2. AWS CDK 설치 (Offline 방식)
CDK는 NPM 패키지이므로 npm으로 오프라인 설치가 필요합니다.
🔹 2-1. 외부 인터넷이 되는 PC (또는 CloudShell)에서 CDK 설치 파일 준비

mkdir cdk-offline
cd cdk-offline
npm pack aws-cdk@2.141.0  # 최신 버전 확인 가능
이 명령으로 aws-cdk-2.141.0.tgz 같은 tarball 파일이 생성됩니다.

원하는 버전으로 설치하세요. 예: npm pack aws-cdk@2.130.0

또는 npm install --ignore-scripts로 디펜던시까지 다운로드할 수도 있습니다.
npm install aws-cdk@2.141.0 --ignore-scripts

🔹 2-2. 필요한 모든 패키지 포함한 오프라인 번들 생성 (선택)
CDK 자체만 쓰는 경우는 .tgz 하나로 충분하지만, 프로젝트를 생성하려면 dependency까지 필요하므로 다음 방법 추천:
npm install aws-cdk@2.141.0
npm install --package-lock-only
zip -r cdk-offline.zip node_modules package.json package-lock.json
또는 tar czf cdk-offline.tar.gz node_modules package.json package-lock.json

🔹 2-3. 파일을 보안망 Windows로 복사
	•	aws-cdk-2.141.0.tgz 또는 cdk-offline.zip 파일을 로컬 PC로 다운로드 후, 보안망 Windows로 복사

🔹 2-4. 보안망 Windows에서 설치

Node.js가 설치된 상태에서 다음 실행:
npm install -g aws-cdk-2.141.0.tgz

cd cdk-offline
npm install -g .


cdk --version

qMjPtQzjP472cHSi8ud25mcAbEBmKW0Pe







source ~/.aliases

alias alall="grep 'alias al' ~/.aliases"
alias alaws="grep 'alias alaws' ~/.aliases"

alias alaws_list="aws configure list-profiles"
alias alaws_stat="aws sts get-caller-identity"





