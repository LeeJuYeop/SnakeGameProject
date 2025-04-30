# 사용자 메뉴얼
리눅스 환경을 기준으로 한다.

1. 게임을 실행 시키기 위해서는 NCURSES 라이브러리를 다운 받아야 한다. 다운로드 방법
은 아래 ‘4.2 설치 방법’에서 기술하도록 한다.
2. Snake의 이동방법: w, a, s, d키를 이용하여 Snake 의 방향을 조종 할 수 있다. 대신 현재
진행 방향과 반대 방향의 키를 입력 할 경우 GameOver가 된다.
3. Apple아이템을 먹은 경우 Snake의 몸체 길이가 늘어나게 되고 Trap아이템을 먹은 경우
몸체 길이가 줄어 들게 된다. 하지만 이때 몸체의 길이가 3 이하로 줄어들게 되면
GameOver가 된다. 추가적으로, Speed아이템을 먹은 경우, 지정된 속도 단계로 Snake의
움직임 속도를 변화시켜 준다.
4. Warp에 Snake가 들어가게 되면 반대쪽 Warp로 나오게 된다.
5. MissionBoard에 있는 목표치를 달성하게 되면 다음 단계로 자동으로 넘어 가게 된다.
6. 4단계의 목표치까지 달성한다면 GameClear가 된다.

# NCURSES 설치 방법
1. 터미널에 “wget https://ftp.gnu.org/pub/gnu/ncurses/ncurses-6.2.tar.gz -P ~/Downloads”를
입력하여 NCURSES 라이브러리를 설치한다.
2. 설치한 파일을 압축 해제한다.
3. 해당 디렉토리로 이동하여 터미널에 “sudo apt install make”를 입력하여 설치한다.
프로그램 컴파일 및 실행 방법
1. 터미널에 “g++ -o [FileName] main.cpp board.cpp snake_game.cpp item.cpp -lncurses”를
입력하여 컴파일 하여, [FileName]의 이름을 갖는 실행 파일을 생성한다.
2. 터미널에 “./[FileName]”을 입력하여 정상적으로 스네이크 게임이 실행되는지 확인한다.
