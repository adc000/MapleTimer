# 사용 전 주의사항
- 해당 프로그램을 사용함에 있어 발생할 수 있는 모든 사항은 사용자 개인의 책임입니다.
- 해당 프로그램을 사용하여 발생하는 모든 사항에는 개발자는 책임이 없음을 알려드립니다.

# 프로그램의 권한
- 해당 프로그램은 타 프로세스(MapleStory)에 접근하여 화면을 Read합니다. 
    - Discord의 화면 공유와 같은 권한
    - 이미지 검출용
- 해당 프로그램은 키보드의 입력을 확인합니다.
    - 게임 키뷰어와 같은 권한
    - 키를 입력받아 마지막 입력된 key의 시간을 검출하기 위함.

# Issue
비 개발자의 경우 닷넷프레임워크(.Net Framework)가 설치되어 있지 않을 수 있습니다.

이 경우 프로그램이 실행되지 않을 수 있습니다.

관련된 오류가 발생하는 경우 [link](https://dotnet.microsoft.com/ko-kr/download/dotnet-framework/net472)에서 다운로드 받으시면 해결됩니다.

화면이 제대로 나오지 않을 경우 디스플레이 -> 배율 및 레이아웃 -> 텍스트, 앱 및 기타항목의 크기 변경 이 100%가 맞는지 확인해주세요

![Alt text](img/image-7.png)

# 사용방법
1. 처음 프로그램을 켜면 같은 폴더 내 config라는 파일이 생성됩니다.
해당 파일은 설정값을 개인에 맞게 저장하는 파일입니다.
기본적으로 해당 프로그램은 본캐가 비숍인 개발자에 맞게 제작되어있습니다.

![Alt text](img/image.png)

2. option 좌측 checkbox를 눌러 초기 옵션을 설정합니다.

![Alt text](img/image-1.png)

3. 본인의 상황에 맞게 쿨감, 벞지를 설정합니다.
- 쿨감의 경우 에르다파운틴 재설치 시간 알림에 영향을 미칩니다.
- 벞지의 경우 추가 버프 스킬의 지속시간에 영향을 미칩니다.

4. 에르다 파운틴은 설치기로 사용하도록 미리 마우스 우클릭을 통해 설정해주세요

5. 스킬 1과 스킬 2는 모두 버프스킬의 재사용 알림 시간을 초기화시킵니다. 언스테이블메모리를 고려하여 구현되어있기 때문에 필요 없는 경우 스킬 1과 스킬 2를 같은 버튼으로 설정해두면 됩니다.

6. [인피니티] 에 적힌 글씨는 음성 알림시에 사용됩니다. 이상한 글씨를 적을 경우 오류를 발생시킬 수 있습니다.

7. 예시의 40은 버프의 기본 지속시간을 의미합니다. 예를들어 쓸만한 스킬의 경우 180을 입력하면 됩니다.

8. 기본으로 인피니티가 아이콘으로 설정되어있으나, icon.png의 이름으로 같은 폴더내 다른 이미지가 들어있을 경우 해당 아이콘이 설정됩니다.

![Alt text](img/image-2.png)

(재획비 이미지를 icon.png로 변경하여 폴더에 넣은 경우.)

9. 추가 표시는 좌측에 표시할 퀵슬롯창 아이콘의 표시 여부와 위치입니다.
아래 이미지를 참조하여 위치를 설정하면 됩니다.

![Alt text](img/image-4.png) ![Alt text](img/image-5.png)

![Alt text](img/image-3.png)

10. 상단 slide bar를 움직이면 투명도를 조절할 수 있습니다.

11. 해상도를 바꾸면 맞게 퀵슬롯을 조절할 수 있습니다.

12. 창을 움직이고 싶으면 바탕으로 보이는 아무 위치를 클릭 후 드래그 하면 됩니다.

13. Stop 으로 타이머를 멈출수 있으며, Close로 창을 종료할 수 있습니다.

14. sub에 체크할 경우 창이 1개 더 load됩니다. 기본 창의 모든 기능을 복제하며,
듀얼모니터 유저를 위해 양쪽에 모두 Timer를 켜고 싶은 경우 사용하면 됩니다.

15. ES check box를 check할 경우 필요한 이미지를 제외하고는 모두 투명화 됩니다.
또한, 마우스 클릭을 통해 창을 움직일 수 없게 됩니다.

![Alt text](img/image-6.png)

16. 시간이 거의 만료되면 배경이 붉게 변하며, 시간이 모두 종료될 경우 음성으로 알림이 울립니다.

# Release Note
[v0.5]
- Config 저장 관련 순서가 잘못되어, 정상적으로 저장되지 않던 문제가 수정되었습니다.
config data는 값이 변경될 때 마다 저장됩니다.
(버그 수정에 도움을 주신 인벤닉 : 경경이님 감사합니다.)
- 아이콘의 배경이 투명해졌습니다.
(투명 파일 제공해주신 인벤닉 : 유니쿠님 감사합니다.)
- key bind에 ALT를 추가했습니다. 모든 alt, shift, control은 좌측키만 해당됩니다.

[v0.4]
- config load후 data가 progress bar에 적용되지 않아 발생한 문제를 수정했습니다.
- 재사용 대기시간 감소 % 효과에 10, 11, 15, 16 %를 추가했습니다.(프리드용)

[v0.3]
- 에르다파운틴을 (없음) 으로 선택할 경우 관련 UI가 사라집니다.
- 스킬 1과 스킬 2를 모두 (없음) 으로 선택할 경우 관련 UI가 사라집니다.

![Alt text](img/image-8.png)

- 음성 알림옵션 중, 5초 전 미리 알림, 짧게 알림 기능이 추가되었습니다.
- 키보드 선택에 좌측 CTRL과 좌측 SHIFT가 추가되었습니다.


# 추후 개발 예정 사항 (일정 미정)
- 