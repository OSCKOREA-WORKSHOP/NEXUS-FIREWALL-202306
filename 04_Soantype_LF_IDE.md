<br><br><br>

# 1. 개발자 IDE Tool integration

## 1-1. IntelliJ IDEA 설치 (Community Edition)
<br>
Ultimate 유료 버전 계정이 있으시면 그대로 사용합니다. <br>
없을경우 무료 버전에서 사용해도 무방합니다. <br>
<br>
Intellij 설치가 안되어있다면 아래 링크로 접속하여 설치합니다. <br>
자신의 환경에 맞게 설치를 진행합니다. <br> 
URL : https://www.jetbrains.com/idea/download/#section=windows <br>

![img](https://github.com/OSCKOREA-WORKSHOP/NEXUS-FIREWALL-202306/blob/master/img/Nexus_LF_ID_img/Intellij_IDE_Install.png)
<br>
<br>

설치가 완료 되었다면 재부팅 합니다. <br><br>

---

## 1-2. Sonatype Nexus IQ Plugin 설치
<br>
아래 그림과 같이 Marketplace를 이용하여 Sonatype Nexus IQ Plugin을 설치합니다.

![img](https://github.com/OSCKOREA-WORKSHOP/NEXUS-FIREWALL-202306/blob/master/img/Nexus_LF_ID_img/Intellij_sonatype_Nexus_IQ_Plugin_install.png)
<br>
<br>

---
## 1-3. 자신의 Project에서 Plugin 적용
<br>
진행중인 Project에서 아래 그림과 같이 구성설정을 진행하여 IQServer와 연동 합니다. 

![img](https://github.com/OSCKOREA-WORKSHOP/NEXUS-FIREWALL-202306/blob/master/img/Nexus_LF_ID_img/Intellij_IQ_Plugin_Configration.png)
<br>
<br>

---

## 2. IQ-Server 확인

이제 IQ-Server와 연동된 자신의 IDE에서 취약점, Policy 정보를 확인합니다.
<br><br>

![img](https://github.com/OSCKOREA-WORKSHOP/NEXUS-FIREWALL-202306/blob/master/img/Nexus_LF_ID_img/Intellij_IDE_result.png)

* 빨간색 박스 : Nexus IQ 확인 및 Component Scan 실행
* 주황색 박스 : Project Component 확인 및 IQ Policy 확인
* 초록색 박스 : 주황색 박스에서 클릭한 Component의 세부 정보 권장버전 추천, Version 별 인기도, Policy 등급 등
* * In use : 현재 사용하고 있는 버전
* * Recommended : 권장 버전 추천
* 보라색 박스 :
* * Details : 초록색 박스에서 클릭한 Component의 세부정보 확인 (CVE)
* * Migrate to Selected : 초록색 박스에서 클릭한 Component Version으로 Pom.xml에 자동으로 반영

