# DevOps-01-P2-TeamH

DevOps Bootcamp second Project TEAM H

## Tech
<img src="https://img.shields.io/badge/Amazon AWS-232F3E?style=flat-square&logo=Amazon%20AWS&logoColor=white"/>
<img src="https://img.shields.io/badge/fastify-000000?style=flat-square&logo=fastify&logoColor=white"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=MongoDB&logoColor=white"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white"/>
<img src="https://img.shields.io/badge/Gihub--Action-2088FF?style=flat-square&logo=GitHub Actions&logoColor=white"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white"/>

## 주제
소비자/라이더/사장님(주문 관리)/사장님(매장 관리) 팀 중 한 부서를 선택하여<br/>
해당 기능 명세를 API 서버로 구현 프로젝트


## 소비자 팀
* 기능 명세: [고객API](https://app.swaggerhub.com/apis/cs-kimcoding/customer/1.0) [배달원 API](https://app.swaggerhub.com/apis/gotoweb/courier/1.0) [메뉴 및 리뷰관리 API](https://app.swaggerhub.com/apis/gotoweb/courier/1.0)
* 메뉴를 선택하고 주문을 생성할 수 있다.
* 현재 배달 상태를 조회할 수 있다.
* 지난 주문 내역을 조회할 수 있고, 리뷰를 남길 수 있다.

## 배포 방식 ( 프론트 & 백엔드 CI/CD)

### 프론트엔드
>node.js + React를 이용하여 개발.<br/>
>프론트 엔드 소스는 제공받은 것을 사용.<br/>
>Git Repository에 소스가 올라오면 Github-Action에 의해 빌드.<br/>
>Build Artifact들이 S3 bucket에 저장.

![image](https://user-images.githubusercontent.com/98450173/173182995-314c8e71-4d49-4c05-b968-8902bf2ce1e6.png)


### 백엔드
>백엔드 WAS는 Node.js를 이용했고, fastify 프레임워크를 사용.<br/>
>이미지를 Github Action에 의해 Build해 ECR로 Dockerizing.<br/>
>Push 된 이미지가 AWS CodePipline의 Codebuild를 통해 ECR에서 ECS로 배포에 적합한 이미지로 변경.

![image](https://user-images.githubusercontent.com/98450173/173186382-e0353325-ada4-4c82-a433-6e3f54dcff7e.png)











## Team
| 이름   | GitHub                                            |
| ------ | ------------------------------------------------- |
| 김정원 | [@devopskims](https://github.com/devopskims)  |
| 이재민 | [@Jaeminst](https://github.com/Jaeminst)  |















