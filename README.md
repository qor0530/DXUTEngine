 순서 

1. 프로젝트 생성
2. 에러 수정
 - abs -> favs
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

11. Director 클래스 제작하다가
 - Init, ChangeScene(Scene* _scene), UpdateScene

12. Node 클래스 제작
- Node, ~Node, position, scale, pivot, layer, rotation, isactive, isui, color, imageRect
- GetMatrix() D3DXMatrixTransformation2D

13. Renderer 클래스 제작
- rendertargets, Comp(Node* a, Node *b)
- AddRenderTarget(Node *node), RemoveRenderTarget(Node * node),
Sort, Render, Clear

14. GameScene 클래스 제작

15.  Texture 클래스 제작

16. Sprite 클래스 제작

17. 이미지 출력으로 테스트 하기 

18. Camera 클래스 제작 

19. 충돌처리 

20. dsound.lib와 사운드 dxut 4개 추가

21. Sound 클래스 추가

22. 헬스바  추가

23. 애니메이션 추가

여기까지 기본 엔진 베이스
