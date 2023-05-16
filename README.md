
23.05.16
1. 횃불퀘스트 진행 시 겹치지 않도록 일정범위 안에서 랜덤하게 이동 후 포탈 오픈 기능 추가

2. 이전 버전 사용자는 아래 내용을 참고하셔서 파일 교체와 현재 사용하시는 캐릭터 이니를 조금 수정하시면 되겠습니다.

→ d2bs\kolbot\libs\bots폴더 OrgTorch.js파일 교체

→ d2bs\kolbot\libs\common폴더 Config.js파일 교체

→ 캐릭터이니 Scripts.OrgTorch = false; 밑에 아래 내용 추가

→ Config.OrgTorch.OpenAfterMove = false; // 이동 후 포탈 오픈(창고가 아닌 인벤토리에 큐브를 소지하고 있어야 함)



![1](https://github.com/qehuial/d2bs/assets/100043245/a6c2f6a3-b342-415a-8334-55eec2e0c16c)


![2](https://github.com/qehuial/d2bs/assets/100043245/890275e8-7033-4fba-970c-98aa086ba851)




﻿
23.04.18


룬 큐빙을 안한다는 글이 많아서 살펴보니 그 이전에 이것저것 실험한다고 큐빙의 일부분을 삭제했었는데

원래대로 복구는 해놨었지만 요걸 깜빡하고 업로드 할 압축파일에는 추가하지 않고 올렸었습니다..

죄송합니다.

1. 룬 큐빙을 제대로 하지 않던점 수정..

→ 이전버전을 사용하시던 분은 d2bs\kolbot\libs\common\Cubing.js 파일만 바꿔주시면 되겠습니다.

 
2. 아케인 생츄어리 전체사냥 오류 수정도 추가되어 있습니다.

→ 이전버전을 사용자분은 d2bs\kolbot\libs\bots\Summoner.js 파일만 교체해주세요
﻿
  
  
23.03.12


1. 인벤토리에 무조건 활력포션을 1개씩 들고다니던 현상 수정

→ 대량의활력포션 인벤토리 보관 수량 > 캐릭터이니에서 수정하도록 변경

→ [ Config.FullRejuvBuffer = 0; // 인벤토리에 0~40개 만큼의 대량의 활력포션을 보관함 ]


2. 포탈책 또는 스크롤이 있음에도 오류나는 현상 수정


3. 벨트에 포탈스크롤 사용 시 인벤토리에 있는 포탈책은 상점에 판매

(다만 벨트 포탈스크롤 사용하다가 비활성화 시 벨트에 있는 포탈 스크롤은 수동으로 버려주셔야 합니다.)
﻿

23.03.11

여러가지 버그들로 인하여 22년 8월 20일자로 롤백했습니다.
(맵핵만 21일자로 적용)


23.02.19

1. d2bs\kolbot\default.dbj

→ D2BotMap.dbj 진입점 실행 시 약간의 오류 수정

2. 한글 매니저 - 기존 매니저 창 크기로 된 매니저 파일 추가

23.02.14

포탈 스크롤 추가 후 제대로 작동하지 않고 엄청난 오류가 발생하여 수정...했지만

제대로 다 고쳐졌는진 모르겠습니다 오류 있으면 말씀해주세요..

일단 제가 싱글로 돌렸을 땐 문제는 없었습니다.

﻿

캐릭터 이니에서 아래 예시와 같이 해주시면 되겠습니다.

![제목 없음](https://user-images.githubusercontent.com/100043245/218508750-46145d45-e469-45f0-8f6d-33c67456900d.png)


위 예시는 아래와 같이 작동 합니다.


1. 벨트 4번째 칸에 포탈스크롤 장착 및 사용


2. 사냥 중 벨트 4번째칸에 1~4개의 포탈스크롤 습득

(벨트 미착용 시 1개 습득하여 4번째 벨트에 보관, 2칸짜리 벨트일 경우 2개 ..등등 )


3. 벨트에 포탈스크롤이 4개가 아닐 때 마을로 이동 시 포탈스크롤 구매

(보통 4개만 가지고 다니니 부족할 듯 싶어 마을 갈때마다 구매 합니다.)


4. 스크롤이 1개가 남았을 때 마을로 이동하여 포탈스크롤 구매

(이 부분은 2개 있을때 사용해서 1개만 남아버리면 바로 소모하여 마을로 이동하여 구매합니다.)

(죄송합니다 너무 귀찮아서... 더 수정을 할 수가 없어요ㅎ;;)

﻿


-수정, 추가된 파일-

1. d2bs\kolbot\libs\NTItemAlias.dbl

→ 하마님 한글 이니 명령어 데센 추가

1. d2bs\kolbot\default.dbj
2. d2bs\kolbot\tools\MapThread.js

→ 맵핵 관련 미적용 되던 부분 수정

1. d2bs\kolbot\libs\common\Pather.js
2. d2bs\kolbot\libs\common\Pickit.js
3. d2bs\kolbot\libs\common\Town.js
4. d2bs\kolbot\libs\common\Misc.js

→ 포탈 스크롤 관련 수정...

1. d2bs\kolbot\libs\common\Attack.js

→ 리더가 디아런에서 포탈을 너무 자주 열던 점 수정..


23.02.13

-수정, 추가된 파일-

1. d2bs\kolbot\pickit\하마님 한글 이니\00_레어.nip

→ 한글 이니 오타 수정

23.02.12

수정, 추가된 파일

1. d2bs\kolbot\tools\MapThread.js
2. d2bs\kolbot\libs\config\ManualPlay.js

→ 기존 BS와 같이 방 입장 시 맵핵 활성화

1. d2bs\kolbot\libs\config\캐릭터 이니파일
2. d2bs\kolbot\libs\common\Misc.js
3. d2bs\kolbot\libs\common\Pather.js
4. d2bs\kolbot\libs\common\Town.js
5. d2bs\kolbot\libs\common\Config.js

→ 벨트에 포탈스크롤 넣어서 사용할 수 있도록 수정

1. d2bs\kolbot\libs\NTItemAlias.dbl
2. d2bs\kolbot\libs\NTItemParser.dbl
3. d2bs\kolbot\pickit\하마님 한글 이니 폴더, 파일 추가

→ 하마님이 번역해주신 한글화 이니 적용 + 이니 명령어 중 갯수 외 수량도 사용 가능하게 변경

→ 한글화 사용하려면 캐릭터 이니에서 추가하셔야 합니다.



23.01.25
1. 한글판 매니저 추가 (오류가 있을 시 기존 매니저로 사용해주세요.)

→ 기본 창 크기 수정

![1](https://user-images.githubusercontent.com/100043245/214550293-022ca636-6508-4e08-9edd-0b3cf4c49a81.png)



22.11.26
1. 기존: 자동사냥 중 맵핵 불가능
   
   수정이후: 자동사냥 + 맵핵 사용가능
2. 간혹 라카니슈를 잡지않고 마을로 이동 현상 수정 (약간의 딜레이[0.1초] 추가)

22.8.23
1. 활력포션 구동방식 변경
→ 이전 버전 쓰시는분들은 kolbot\libs\common 폴더만 덮어쓰기 해주시면 됩니다.

→ 큐빙 후 창고에 보관하지 않습니다.

→ 캐릭터이니에서 대량의 활력포션 큐빙 활성화 하면 아래와 같이 작동합니다.
활력포션 3개 습득 > 큐빙 > 대량의 활력포션 들어갈 자리가 있으면 벨트로 이동 > 벨트에 자리가 없으면 인벤토리에 보관 > 아이템 이니에 설정한 맥스 수치가 초과되면 바닥에 드랍


22.8.22
1. 활력포션 큐빙 후 인벤토리에 끝도 없이 모으던 현상..수정

→ 아이템 이니에서 아래처럼 숫자를 기입하시면 그 이상 큐빙된 것들은 바닥에 버리도록 해놨습니다.

→ 인벤토리에 보관된 대량의 활력포션은 알바가 알아서 사용 및 벨트로 옮깁니다.

![1](https://user-images.githubusercontent.com/100043245/185920847-fd172e3b-7b90-4210-bb07-b8575106edca.png)



22.8.21
1. 활력포션 큐빙 추가

![2](https://user-images.githubusercontent.com/100043245/185921121-afa4efe3-ea78-42ef-9199-a6b852dfaeb5.png)

2. 맵핵 몹표시 수정

![1](https://user-images.githubusercontent.com/100043245/185794996-700e4a0b-d465-4cc8-a31a-6b68151536a0.png)



22.8.20
1. 사냥 종료 후 나가기 딜레이 추가

1-2. 방 퇴장 딜레이 0초 표기 안되는 문제 수정, 시간초 이상으로 대기하다가 나가는 문제 수정

2. 맵핵 사용 시 상세정보 보기 기능 추가 단축키 넘버패드 <6> 입력 시 아이템(아이템 숨렙, 소켓, id 등..), 몬스터, NPC 상세정보 보기 가능

→ 아이템에 마우스 올려놓고 OFF 시킬 시 상세정보 창이 안사라집니다. 그때는 마우스를 아이템에서 떼고 다시 ON 했다가 OFF 하시면 됩니다.

![1](https://user-images.githubusercontent.com/100043245/185675097-7c408004-2fe4-4b56-aa05-da8d718539a8.png)



22.8.17
1. d2bs\kolbot\libs\common\Attacks\Paladin.js

→ 22.8.15일자 업데이트 후 스킬(스마이트, 질) 사용시 오오라 사용안하던 문제 수정

2. d2bs\kolbot\default.dbj

3. d2bs\kolbot\D2BotLead.dbj

4. d2bs\kolbot\libs\config\각 캐릭터 이니

→ 방 나가기 전 대기 시간이 작동하지 않던 부분 수정


![22](https://user-images.githubusercontent.com/100043245/185172808-061e8160-3100-461d-a33c-7008beafe9e1.png)
![33](https://user-images.githubusercontent.com/100043245/185172833-ececd5b8-63e5-44bf-9c54-58d5c9ef4993.png)



22.8.15
1. 밀리 캐릭 공격속도 전체적으로 수정

→ 이것저것 건들여서 수정한 파일 목록은 제외


22.8.14
1. d2bs\kolbot\libs\common\Attacks\Wereform.js

→ 사냥 중 변신 풀지 않도록 수정

→ 곰,늑대 변신 후 연속 공격이 느린점 수정

2. d2bs\kolbot\libs\config\Druid.곰,늑드루(캐릭터명으로 바꿔주세요).js 파일 추가

3. d2bs\kolbot\libs\common\Pather.js

→ 문 오픈 시 캐릭터 위에 나오는 문구 번역

22.7.10

1. MF헬퍼 오류 수정
→ 제대로 확인해보지 못했습니다. 오류가 있으면 카페에 글 올려주시면 감사하겠습니다.


22.3.27

1. d2bs\kolbot\D2BotMule.dbj

2. d2bs\kolbot\libs\AutoMule.js

3. d2bs\kolbot\libs\NTItemParser.dbl

→ Skeptic님이 올려주셨던 FinalSorc의 창고지기를 추가했습니다(NT방식 창고지기)

→ 초기단계라 오류가 있을 수 있습니다 원래 파일은 꼭 백업해주세요!


![6](https://user-images.githubusercontent.com/100043245/161565628-92097794-e913-423c-b56c-7aae3d6da472.png)


22.2.20

1. 꽤 지나서 기억은 안나는데 자잘한것들 수정했습니다.


9.25

1. d2bs\kolbot\libs\common\Config.js

2. d2bs\kolbot\libs\bots\NecroPindle.js파일추가

3. d2bs\kolbot\libs\config\네크, 조폭네크, 조폭독네크 이니 수정

→ 니라트하크 사원에 입장해서 소환물 소환

![5](https://user-images.githubusercontent.com/100043245/161564203-7450033f-f23a-4635-9add-44d0a241d52f.png)

4. d2bs\kolbot\libs\bots\MFHelper.js

→ 문구 오류 수정


9.17 - 추가 수정

수정, 추가된 파일

1. d2bs\kolbot\libs\common\Config.js

2. d2bs\kolbot\libs\bots\Nihlathak.js

3. d2bs\kolbot\libs\config\ 캐릭터 이니파일

→ 추가 번역

→ 니라트하크 길목 사냥 따로 추가(요청사항)

![9999](https://user-images.githubusercontent.com/100043245/161565559-e63f36d0-a3db-4217-8cd9-0c65c265bb6d.png)



4. d2bs\kolbot\libs\common\Misc.js

→ 오역 수정

![3](https://user-images.githubusercontent.com/100043245/161565070-71903139-2cc3-4744-a19a-0a3758e5076b.png)
![4](https://user-images.githubusercontent.com/100043245/161565077-3a28f59e-db01-4f41-b98b-2412930f62e5.png)



9.15 - 추가 수정

수정, 추가된 파일

1. d2bs\kolbot\libs\config\ 캐릭터 이니파일 수정

캐릭터이니 파일 설명 몇가지 추가 번역 및 몇가지 수정

- 추가 수정 내용

1. d2bs\kolbot\libs\config\Amazon.활아마이니(캐릭터명으로 바꿔주세요) 파일 추가

→ 화살 구매 방식 선택 가능 추가 (기존 방식과 수정 후 방식)

→ Config.ArrowsBuy가 true일 때 화살통 1개 인벤토리 보관

![2](https://user-images.githubusercontent.com/100043245/161563656-3d04f617-4240-44fe-9757-e5ac6e496529.png)

2. d2bs\kolbot\libs\common\Town.js 수정

3. d2bs\kolbot\libs\common\Config.js 수정


9.13

수정, 추가된 파일

1. d2bs\kolbot\libs\common\Town.js 수정

2. d2bs\kolbot\libs\config\Amazon.아마이니(캐릭터명으로 바꿔주세요).js

- Config.PickitFiles.push("arrows.nip"); 구문 추가

3. d2bs\kolbot\pickit\arrows.nip 파일 추가

아마존 화살 구매 수정

기존

화살 잔여수 * 100 / 화살최대수량 <= Config.RepairPercent개 마을로 이동 상점에서 화살 구매

변경

화살 잔여수 = 0개 마을로 이동 상점에서 화살 구매

arrows.nip파일 >> 화살통 1개 인벤토리에 보관


9.12

1. 인게임, 매니저 콘솔창 등 표시 되는 글 부분한글화

![997](https://user-images.githubusercontent.com/100043245/161561896-8b33bd52-1e7e-4676-959c-77fb33098de3.png)

2. ClearAnyArea를 이용한 전체사냥 중 특정 사냥터 Attack.clear: range must be a number.오류 수정


9.11

1. 상세정보 볼때 착용 아이템에 결빙 옵션이 있을때와 없을때 나오는 글 추가

![0](https://user-images.githubusercontent.com/100043245/161562670-a50b67c8-06ee-47ab-b9dc-400f2606ed0e.png)

2. 창고지기 부를때 나오는 영어 채팅 한글로 번역


-----------------------------------------------------------------------------------------------------------------------

![998-2](https://user-images.githubusercontent.com/100043245/161561903-23c14090-e3a4-4d8b-82e6-cde7a50a0b08.png)
![998-3](https://user-images.githubusercontent.com/100043245/161561906-da057f42-de96-40fd-906a-e0da015b438f.png)
![999](https://user-images.githubusercontent.com/100043245/161561909-9481e0a5-5a76-4fa9-b54d-50becf0ace5e.png)
![999-2](https://user-images.githubusercontent.com/100043245/161561910-7f96b0f2-e9a5-4e91-baa5-80a8b4913703.png)
![999-4](https://user-images.githubusercontent.com/100043245/161561913-d2c6dd30-3230-4798-aaed-0d8ca27ab55b.png)

