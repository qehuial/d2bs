수정, 추가된 파일
22.11.26
1. 봇 돌리면서 맵핵사용 가능
2. 간혹 라카니슈를 잡지않고 마을로 가는 오류 수정

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

