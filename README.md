# DXUTEngine
DXUT 엔진 연습


순서 

1. 프로젝트 생성
2. 에러 수정
 - abs -> fabs
3. DXUT.h 에서 Ctrl +F 후 dxerr.h 아래에
 auto __vsnwprintf = _vsnwprintf;

4. 빌드 해보기

5. 콜백함수 2개 삭제
 - ModifyDeviceSettings
 - MsgProc

6. 속성 - 링커 - 시스템  -> 하위시스템 
 콘솔로 바꾸기 

7. wWinMain -> int main() 변경 
 오류나는 코드 삭제

8. DXUT.h 마지막 줄에 추가
 - iostream, list, map, vector, algorithm, string, time 
 - using namespace std;
 - typedef Vec2, Vec3, Color
 - define DEVICE DELTATIME, ScreenW, ScreenH

9. Scene 클래스 제작
 - Init Update Exit PURE

10. Singleton 클래스 제작

11. Director 클래스 제작
 - ChangeScene, UpdateScene

12. OnD3D9FrameRender 에서 선언해주고 Render

13. GameScene 클래스 제작

14. Scene 할당해서 Render

15. 강제 릴리즈 

16.  Texture 클래스 제작

17. Node 클래스 제작

18. Sprite 클래스 제작

19. Renderer 클래스 제작

20. 이미지 출력으로 테스트 하기 

21. Camera 클래스 제작 

22. 충돌처리 

23. dsound.lib와 사운드 dxut 4개 추가

24. Sound 클래스 추가

25. 헬스바  추가

26. 애니메이션 추가
