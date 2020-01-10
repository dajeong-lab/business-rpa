

# RPA 1Day

1. 개발시 고려사항
    * 입출력 데이터
    * 개발 공수 산정
    * 예외처리
    * 테스트환경(인프라/운영/테스트데이터/데이터생성)
    * 테스트 
    
1. 설치파일 다운로드 경로
      * http://download.uipath.com/UiPathStudioSetup.exe

1. 기능
    * 글로벌 핸들러 : 에러 핸들러
    * ControlChars.NewLine
    * String.join
    * Computer Vision = Image
    * VDI 제어 = Runtime 설치(Windows Remote Desktop 설치) / 패키지 설치

# RPA 2Day

1. select
      * 단축키:F4, UI Explorer > UI 
2. Vision
      * 쿠다ML(무료)
3. 엘리멘트 쪼개기 click image property
      * Cursorposition > BottonRight
4. 핫키 반복하기
      * String.Join("", Enumerable.Repeat("[d(alt)] [u(alt)]",20))
5. 병렬 실행
      * Pick(Pick Brunch)


# RPA 3Day

1. 화면이 바뀔때 무조껀 find element 를 사용한다

2. anchor base의 anchor의 위치를 정확히 명시해야한다

3. 메일 발송시 body의 내용은 보통 텍스트 파일로 와꾸를 만들어놓고 파라메터에 의해 변해야 하는 경우 {0} 등으로 중괄호로 채워넣은 후 string.format(텍스트 string, 변수, 변수) 로 처리한다.

4. type into 클릭등은 엘리먼트를 찾으면 찾았다고 인지하여 시그널을 보내는데, 마우스 커서가 가기전의 경우에 시그널이 날라가서 텍스트가 정상적으로 들어가지 않을 수 도 있음
 - 이럴경우 click before typing을 체크해주고,  Find element 엑티비티를 써주고 waitvisible, waitactive 을 쓰면 좀더 안정적이다.
 
5. Library
      * New Project > Library > 코딩후 > Publish(Orchestrator 없다면 로컬PC)
      * New Process > Manage Package > Settings > Name/Source(로컬경로/Orchestrator) Add
      * Name 지정된 메뉴 이동 후 Library 설치
      
6. 나만의 템플릿
      * Save as a Template > Create > Home 확인
      
7. UiPathic 코드
      * Name = otherName : Name.Equals(otherName)
      * Name = "" : String.IsNullOrEmpty(Name)
      
8. 소스 쪼개기
      * Extract as Workflow
      
9. Word 파일 보고서 만들기
      * Replace Text 변수 [[test]]
      
10. Orchestrator 
      * 실행은 무조건 UR
