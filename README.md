LOGICCUBE's New HomePage under construction

www.logiccube.co.kr 은 예스닉을 통해 domain 등록되어 있습니다.

https://yesnic.com/ 로그인후 
네임서버 고급설정 >> CNAME 레코드 관리를 통해 현재의 github에 등록된 index.html로 연결됩니다.

<< 설정1 >>
📝 예스닉 CNAME 최종 입력 예시
예스닉의 CNAME 관리 화면에서 [신청란 추가] 버튼을 누른 후 다음과 같이 입력하세요.

신청 (체크박스): 체크(v) 선택
호스트명 (또는 서브도메인): www

CNAME (또는 연결주소): logiccubeinc.github.io
(만약 뒤에 점을 찍으라는 안내나 에러 메시지가 뜨지 않는다면 점 없이 깔끔하게 주소만 적으시면 됩니다.)

<img width="731" height="519" alt="image" src="https://github.com/user-attachments/assets/a8ae917b-4d5b-40fa-a852-4b9e57dc6d2f" />

<< 설정2 >>

1단계: 
예스닉에서 A 레코드 추가하기예전에 방문하셨던 [네임서버 고급설정 > DNS 관리] 
페이지(여러 레코드 목록이 쭉 있던 화면)로 다시 이동합니다.

A 레코드 관리(네임서버 호스팅) 메뉴의 [관리화면 열기 ▼]를 누릅니다.아래와 같이 4개의 레코드를 각각 한 줄씩 총 4번 추가해 줍니다. 
(이 IP들은 깃허브 페이지의 공식 고유 서버 주소입니다.)선택도메인명(호스트명)IP 주소신규(아무것도 적지 말고 빈칸으로 둠)
.logiccube.co.kr185.199.108.153 신규(아무것도 적지 말고 빈칸으로 둠)
.logiccube.co.kr185.199.109.153 신규(아무것도 적지 말고 빈칸으로 둠)
.logiccube.co.kr185.199.110.153 신규(아무것도 적지 말고 빈칸으로 둠)
.logiccube.co.kr185.199.111.153 신규(아무것도 적지 말고 빈칸으로 둠)

입력 후 하단의 [다음 단계로]를 눌러 설정을 저장합니다.

2단계: 
GitHub Settings에서 최종 확인하기예스닉 설정이 끝났다면, 깃허브가 두 주소를 알아서 하나로 묶어주도록 옵션을 켜야 합니다.

GitHub 레포지토리의 Settings > Pages 메뉴로 이동합니다.
Custom domain 칸에 이미 www.logiccube.co.kr이 들어가 있을 것입니다.

예스닉에서 설정한 A 레코드가 깃허브 시스템에 반영되면, 그 바로 아래에 있는 Redirect subdomains라는 안내 문구와 함께 관련 옵션이 활성화되거나 자동으로 리다이렉트 처리가 진행됩니다.
⏳ 적용 확인하기A 레코드 정보가 인터넷에 전파되는데도 약간의 시간(수 분 ~ 수 시간)이 걸립니다.

<img width="670" height="711" alt="image" src="https://github.com/user-attachments/assets/445e01c0-a3c4-47d6-bc6b-671d4828ee24" />
