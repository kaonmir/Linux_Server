## OpenSSH로 아마존 접속하기
### OpenSSH 설치하기
1. 윈도우키 누르고 "선택적 기능 관리" 검색
2. 기능 추가를 누르고 OpenSSH 클라이언트를 설치
* (만약 윈도우를 서버로 쓸 거면 OpenSSH 서버도 설치하는데 우리는 아니니까 생략)

### 아마존 서버에 접속하기
 * 유저 이름은 Amazon Linux AMI의 경우 'ec2-user'다
  * 나머지 AMI는 [[여기](https://docs.aws.amazon.com/ko_kr/AWSEC2/latest/UserGuide/putty.html#putty-ssh)] 참조
 * 아마존 인스턴스 창을 통해 '퍼블릭 DNS(IPv4)를 복사한다.
 * 인스턴스를 만들 때 다운 받은 키페어의 경로를 기억합니다.
 * `ssh -i "키페어" "유저 이름@퍼블릭 DNS"`을 입력합니다.
  * 예시 : `ssh -i "MyKeypair.pem" ec2-user@ec2-00-000-0-000.us-east-2.compute.amazonaws.com`
 * 접속이 잘 이루어졌다면 최종적으로 `[유저 이름@ip-프라이빗 IP ~]$`이 나온다.
 * 저 같은 경우에는 이 명령어를 batch 파일로 만들어 실행했습니다.
