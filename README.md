## 제목 : Azure App Service 및 Serverless 핸즈온랩 워크샵

클라우드는 IaaS를 넘어, PaaS로 그리고 PaaS를 넘어 마이크로 PaaS인 서버리스로 그 관심이 옮겨가고 있습니다. 서버의 인프라를 직접 관리하거나, 운영할 필요가 없는 PaaS 및 Serverless 기술은 이미 많은 기업의 개발자들이 주목하고 있는 핫한 기술입니다. 

이번 HOL에서는 Azure에서 제공하는 PaaS 서비스인 App Service의 일부 기능과 서버리스 기술인 Function App과 Logic App을 직접 코딩하고 개발하면서 그 뛰어난 유연성과 효율성을 직접 느낄 수 있도록 할 예정입니다. 우선 App Service와 Serverless의 기본적인 개요를 전문 강사의 기술 세션을 통해서 살펴본 뒤, 다양한 실습들을 자신의 노트북에서 직접 Coding 해 보는 시간을 갖습니다.

자주 접하기 쉽지 않은 '실습' 워크샵이기에 서버리스를 배워보고 싶으는 분들은 이번 HOL을 놓치지 마세요!

#### **기술 수준** : 
- 100 레벨(초급)
#### **대상** : 
- 기업에서 근무하는 초, 중급 개발자
- 프리랜서 개발자
- 모태솔로 개발자

#### **강사** : 
- 한상훈, ASP.NET Korea 유저그룹 운영자
- 박용준, Taeyo.NET 부운영자
- 김태영, 한국 마이크로소프트

#### 실습시간(예상) : 5-6 시간 

#### 참가자 특전 : 
- (원할 경우) ASP.NET Korea 번개 모임에 초대
- (원할 경우) 서버리스 관련 무료 컨설팅/핵페스트 프로그램 제공 

## HOL(Hands-on Lab) 진행 순서

- 실습 준비 (20분)
    - 필요한 Azure 리소스 생성
        - 리소스 그룹, 저장소 계정, 앱 서비스 계획 등

### 기술 세션 : Azure의 App Service 소개 (30분)

- 실습 1 : App Service 생성 및 개발 실습 (40분)
    - Git을 사용하여 다양한 코드 배포(HTML, ASPX, JSP 3단 변신)
	- 런타임 플랫폼 변경 및 실행
	- 실행 관련 이슈 트러블슈팅
    - Continous Deployment를 통한 자동 배포

- 실습 2 : Java WebApp(WAR) 배포 및 운영 실습 (30분)	 
	- 참고 링크 : https://github.com/Azure-Samples/app-service-web-java-get-started	 
	- 이미 만들어져 있는 WAR 파일을 App Service에 배포
	- 온라인 에디터로 실시간 소스 수정
	- SCM(Kudu)을 통해서 Web App의 내부 콘솔 살펴보기
	- WebApp의 Authentication 기능을 이용한 보안 설정
		- https://docs.microsoft.com/ko-kr/azure/app-service-mobile/app-service-mobile-how-to-configure-microsoft-authentication

### 기술 세션 : Azure의 Serverless 소개 (30분)

- 실습 3 : 온라인으로 Azure Functions 개발 실습 (20분)
    - Azure Portal을 통한 코딩 실습
    - 트리거, 바인딩 실습
	- 브라우저 및 PostMan을 사용한 테스트
    - Authorization Level에 따른 테스트
	- 모니터링 및 관리 실습

- 실습 4 : Azure CLI를 이용한 Function 개발 실습 (20분) 
	- Command Line Interface를 통해서 개발
    - 로컬 머신 테스트
    - VS Code를 이용한 Javascript(Node.js) 로컬 디버깅
    - Function pack을 이용한 서버 배포

- 실습 5 : 이미지 프로세싱 실습 (30분)
    - 원본 링크 : [https://github.com/lindydonna/CoderCards](https://github.com/lindydonna/CoderCards)
    - Blob 트리거와 이미지 프로세싱 실습 
    - 기존 개발되어 있는 소스를 사용하여 변형 실습
    - SCM(Kudu)을 이용한 폴더 업로드
    - 시나리오
        - 인물 사진을 Blob 저장소에 저장하면
        - 해당 이미지를 Microsoft AI : Face API로 분석하여
        - 행복 지수에 따라 이미지 배경을 변경 및 이름과 직급을 기입
        - Output용 Blob 저장소에 변형된 이미지를 저장

### 미니 세션 : 서버리스 핵페스트 프로그램 소개 (10분)


- 실습 6 : Logic 앱을 사용한 워크플로우 실습 (30분)
	- Facebook과 Blob Storage(Dropbox) 연계 실습
    - 원본 참조 : [https://github.com/options/choco](https://github.com/options/choco)
    - 시나리오
        - 자신의 페이스북 담벼락에 글을 남기면
        - 그 텍스트를 음성으로 변환(Text to Sppech)하고
        - 지정된 Blob 저장소에 파일로 생성함
        - (option) 음성 파일이 생성되었음을 메일로 알려줌

    
## 모든 참가자는 다음의 사항들을 반드시 본인의 노트북에 설치하고 오셔야 합니다. 

### 참가자 준비물 (필수)
> 1. 노트북 (Windows OS, Mac OS)
> 2. Azure 계정(무료 계정이든, MSDN 계정이든, 회사 계정이든)  
> 3. 테더링 가능한 스마트폰(네트워크 사정이 안 좋을 경우 테더링을 강추합니다)  

**준비물 미 준비 시에는 실습을 제대로 따라하실 수 없으며, 그 부분은 본인의 책임입니다**

### 강좌 참여 시 사전 준비 및 설치 사항(필수)
> - Visual Studio Code 설치 : https://code.visualstudio.com/  
> - Azure CLI 설치
>   - Windows : https://aka.ms/InstallAzureCliWindows    
>   - Mac OS : https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest  
> - Postman 설치
>   - https://www.getpostman.com/postman     
> - Azure Storage Explorer 설치
>   - https://azure.microsoft.com/en-us/features/storage-explorer/
> ### 다음은 순서대로 설치하시기 바랍니다
> 1.  Node 8.5 이상의 Stable 버전 설치 (9.X 버전은 안됩니다)
>       - https://nodejs.org/en/     
> 2. .NET Core 2.0 SDK 설치 
>       - https://www.microsoft.com/net/download/windows
> 3. Azure Functions Core Tools 설치 (CMD 명령 프롬프트에서 실행) 
>       - npm i -g azure-functions-core-tools@core    
>       - Mac OS인 경우 : sudo npm i -g azure-functions-core-tools@core --unsafe-perm   
> 4. Azure Functions Pack 설치 (CMD 명령 프롬프트에서 실행) 
>       - npm i -g azure-functions-pack    

    
> # 꼭 미리 설치하고 오세요!!!!