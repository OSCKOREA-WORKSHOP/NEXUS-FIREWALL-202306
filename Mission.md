# Mission #1 (Private Repo 설정)
가장 많이 사용하는 패키지 관리 툴을 설치하고, Public Repository를 사용하지 않고도 Nexus Repository를 통한 컴포넌트/디펜더시 다운로드할 수 있도록 환경 설정.


개인별 3개의 Repository (Individually allocated repository) 가 제공되므로, 아래 내용을 참고해서 본인의 환경에 맞게 설정합니다.
(참조용이며, 이미 각 환경에 맞게 설정이 되어 있다면 개인 환경에서 Proxy 설정만 진행하면 됩니다.)

<br><br>

# Mission #2 (각 언어별 Build 및 패키지 설치, Policy 적용)

  * **[NPM]** :  NPM Malicious 설치 진행해 보고, 관련 내용에 대해서 살펴 봅니다.
   
        npm install @sonatype/policy-demo

    >
    
    
  * **[Maven]** : Sample Maven build 후 보안관련 상황을 살펴보고 IQ Server 를 접속해서, 관련 내용에 대해서 살펴 봅니다.
  
        mvn install
    
 
   
  * **[PiPy]** : PYPI Malicious 패키지 설치하고, IQ Server 를 접속해서, 관련 내용대해서 살펴 봅니다.
   
        pip install Django
   
<br><br>

# Mission #3 (Waiver 를 통한 패키지/Artifact 다운로드 허용)



mission#2 에서의 Malicious 패키지들은 IQ Server 정책에 의해 다운로드가 막혀 있는 상태입니다. 하지만 필요에 의해 일정 기간 불가피하게 사용해야 하는 패키지가 있거나, 아직 보안 패치가 나오지 않은 컴포넌트들도 존재합니다. 이때 보안팀과의 검토를 통해 유예(Waive) 설정을 할 수 있습니다. <br/><br/>

