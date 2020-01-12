

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
    * 줄바꿈 : ControlChars,  Environment.NewLine
    * 문자열 연결 : String.join
    * Computer Vision = Image
    * VDI 제어 = Runtime 설치(Windows Remote Desktop 설치) / 패키지 설치

# RPA 2Day

1. select(Element 가 안잡힐 때)
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

1. 화면 변환시 find element 사용

2. anchor base의 anchor의 위치를 정확히 명시

3. 메일 body : string.format(텍스트 string, 변수, 변수)

4. type into : click before typing 체크, Find element 엑티비티 사용 waitvisible, waitactive 사용
 
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
