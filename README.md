<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>내가 만든 League of Legends/OP.GG</title>
    <link rel="stylesheet" href="opgg프로젝트.css">
    <style>
        * {margin: 0; padding: 0; box-sizing: border-box;}

body { background-color: rgb(234, 234, 234);}

.container {margin: 0 auto; width: 1000px;}

.container section { 
    background-color: #FFF; margin: 20px 0;
    border-radius: 10px;
}

/* 검색메뉴 */
.search_menu {
    height: 100px; padding: 10px;
}
.search_menu .search_bar {
    width: 50%; height: 80px; 
    border: 1px solid #b8b8b8; border-radius: 40px;
    margin: 0 auto;
    display: flex; justify-content: space-around; align-items: center;
}
.search_menu .search_bar input {
    border: none; 
    border-right: 1px solid #000;
    font-size: 15pt;
    width: 150px; height: 40px; text-align: center;
}
.search_button { 
    background-color: skyblue; 
    border: none; width: 70px; height: 50px; border-radius: 25px;
    font-weight: 900; font-size: 15pt;
    cursor: pointer;
}

/* 플레이어 정보 메뉴 */
.player_menu {
    height: 130px; padding: 15px;
    display: flex;
}
.player_menu .player {flex: 3; display: flex;}
.player_menu .player img {width: 100px;}
.solo {flex: 2;}
.flex {flex: 2;}
.solo img {width: 75px;}
.flex img {width: 75px;}

/* 20개 게임 요약 메뉴 */
.summary_menu { 
    display: flex; justify-content: space-around;
    text-align: center;
    padding: 20px;
}
.record {flex: 1; border-right: 1px solid #AAA;}
.lately_champion {flex: 1; border-right: 1px solid #AAA;}
.lately_position {flex: 1;}
.lately_position > div{
    display: flex;
    justify-content: space-evenly;
}

/* 20개 게임들 */
.game20_menu {padding: 20px; text-align: center;}
.game {display: flex; align-items: center; padding: 10px; margin-bottom: 20px;}
.victory {background-color: rgb(215, 244, 255); border-left: 6px solid skyblue;}
.defeat {background-color: rgb(255, 219, 225); border-left: 6px solid rgb(255, 159, 175);}

.mod {flex:1}
.champion {flex:1}
.champion img {width: 50px;}
.multikill {flex:1}
.rune {flex:1}
.rune img { width: 30px;}
.score {flex:2}
.score .kda {font-size: 20pt; font-weight: 900;}
.score .death {color: #F00;}
.item {flex:3}
.item img {width: 25px;}
.users {flex:3; display: flex; justify-content: space-between; text-align: left;}
.users .team1 {flex: 1;}
.users .team2 {flex: 1;}
    </style>
</head>
<body>
    <div class="container">
        <section class="search_menu">
            <div class="search_bar">
                <input type="text" class="name" value="만득아달려" placeholder="이름">
                <input type="text" class="tag" value="티모사랑" placeholder="태그">
                <button class="search_button">검색</button>
            </div>
        </section>
    
        <section class="player_menu">
            <div class="player">
                <img src="https://opgg-static.akamaized.net/meta/images/profile_icons/profileIcon5314.jpg" alt="프사">
                <div class="player_info">
                    <h1>닉네임</h1>
                    <h2>level <span>100</span></h2>
                </div>
            </div>
            <div class="solo">
                <h1>솔로랭크</h1>
                <img src="https://opgg-static.akamaized.net/images/medals_new/challenger.png" alt="솔랭티어">
                <span class="win">ㅇ</span>승 <span class="lose">ㅇ</span>패 / <span class="rate">ㅇ</span>%
            </div>
            <div class="flex">
                <h1>자유랭크</h1>
                <img src="https://opgg-static.akamaized.net/images/medals_new/challenger.png" alt="자랭티어">
                <span class="win">ㅇ</span>승 <span class="lose">ㅇ</span>패 / <span class="rate">ㅇ</span>%
            </div>
        </section>
    
        <section class="summary_menu">

            <div class="record">
                전적
                <h2><span class="win">0</span>승 <span class="lose">0</span>패 <span class="draw">0</span>무 / <span class="rate">0</span>%</h2>
                <h2>KDA <span class="kda">10.0</span></h2>
                <p> <span class="kill">0</span> / <span class="death">0</span> / <span class="assist">0</span></p>
            </div>
            <div class="lately_champion">
                <p>최근 챔피언</p>
            </div>
            <div class="lately_position">
                <p>최근 포지션</p>
                <div>
                    <div class="top">
                        <img src="https://s-lol-web.op.gg/images/icon/icon-position-top.svg" alt="탑">
                        <br>
                        <span>10</span>
                    </div>
                    <div class="jungle">
                        <img src="https://s-lol-web.op.gg/images/icon/icon-position-jng.svg" alt="정글">
                        <br>
                        <span>10</span>
                    </div>
                    <div class="mid">
                        <img src="https://s-lol-web.op.gg/images/icon/icon-position-mid.svg" alt="미드">
                        <br>
                        <span>10</span>
                    </div>
                    <div class="bot">
                        <img src="https://s-lol-web.op.gg/images/icon/icon-position-bot.svg" alt="원딜">
                        <br>
                        <span>10</span>
                    </div>
                    <div class="supporter">
                        <img src="https://s-lol-web.op.gg/images/icon/icon-position-sup.svg" alt="서폿">
                        <br>
                        <span>10</span>
                    </div>
                    <div class="etc">
                        <img src="https://s-lol-web.op.gg/images/icon/icon-position-all.svg" alt="등등">
                        <br>
                        <span>10</span>
                    </div>
                </div>
                
            </div>
        </section>
    
        <section class="game20_menu">
            <div class="game">
                <div class="mod">게임모드</div>
                <div class="champion">챔피언</div>
                <div class="multikill">멀티킬</div>
                <div class="rune">룬</div>
                <div class="score">KDA CS</div>
                <div class="item">아이템</div>
                <div class="users">유저들</div>
            </div>

            <div class="game defeat">
                <div class="mod">자유랭크</div>
                <div class="champion">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/champion/Teemo.png" alt="챔피언프사">
                    <p>레벨 <span>5</span></p>
                </div>
                <div class="multikill">펜타킬</div>
                <div class="rune">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/perk/8439.png" class="rune1" alt="룬1">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/perkStyle/8300.png" class="rune2" alt="룬2">
                </div>
                <div class="score">
                    <p><span class="kda">4.0:1</span>
                        <br>
                        <span class="kill">7</span> / <span class="death">1</span> / <span class="assist">2</span></p>
                    <p>GOLD <span class="gold">20000</span></p>
                    <p>CS <span class="cs">127</span></p>
                </div>
                <div class="item">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item1" alt="아이템1">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item2" alt="아이템2">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item3" alt="아이템3">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item4" alt="아이템4">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item5" alt="아이템5">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item6" alt="아이템6">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item6" alt="아이템7">
                </div>
                <div class="users">
                    <div class="team1">
                        <p class="user1">유저1</p>
                        <p class="user2">유저2</p>
                        <p class="user3">유저3</p>
                        <p class="user4">유저4</p>
                        <p class="user5">유저5</p>
                    </div>
                    <div class="team2">
                        <p class="user1">유저1</p>
                        <p class="user2">유저2</p>
                        <p class="user3">유저3</p>
                        <p class="user4">유저4</p>
                        <p class="user5">유저5</p>
                    </div>
                </div>
            </div>

            <div class="game victory">
                <div class="mod">자유랭크</div>
                <div class="champion">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/champion/Teemo.png" alt="챔피언프사">
                    <p>레벨 <span>5</span></p>
                </div>
                <div class="multikill">펜타킬</div>
                <div class="rune">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/perk/8439.png" class="rune1" alt="룬1">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/perkStyle/8300.png" class="rune2" alt="룬2">
                </div>
                <div class="score">
                    <p><span class="kda">4.0:1</span>
                        <br>
                        <span class="kill">7</span> / <span class="death">1</span> / <span class="assist">2</span></p>
                    <p>GOLD <span class="gold">20000</span></p>
                    <p>CS <span class="cs">127</span></p>
                </div>
                <div class="item">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item1" alt="아이템1">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item2" alt="아이템2">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item3" alt="아이템3">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item4" alt="아이템4">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item5" alt="아이템5">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item6" alt="아이템6">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/3031.png" class="item7" alt="아이템7">
                </div>
                <div class="users">
                    <div class="team1">
                        <p class="user1">유저1</p>
                        <p class="user2">유저2</p>
                        <p class="user3">유저3</p>
                        <p class="user4">유저4</p>
                        <p class="user5">유저5</p>
                    </div>
                    <div class="team2">
                        <p class="user1">유저1</p>
                        <p class="user2">유저2</p>
                        <p class="user3">유저3</p>
                        <p class="user4">유저4</p>
                        <p class="user5">유저5</p>
                    </div>
                </div>
            </div>

        </section>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
    <script>

        const API_KEY = "RGAPI-ddddfeb1-8930-4b24-8522-d712e6789d52"
        let 닉네임 = document.querySelector(".name")
        let 태그 = document.querySelector(".tag")

        let puuid
        let 레벨
        let 프사번호
        let id

        let position = {
            "TOP": 0,
            "JUNGLE": 0,
            "MIDDLE": 0,
            "BOTTOM": 0,
            "SUPPORT": 0,
            "Invalid": 0,
        }

        // 검색 버튼을 클릭하면 모든 검색이 실행된다. 기능 추가해야함
        const 검색버튼 = document.querySelector(".search_button") // 버튼 지정
        검색버튼.addEventListener("click", async function() { // 검색버튼 클릭하면 이벤트 실행

            // 1. ACCOUNT API 들어가기 : puuid 가져오기
            await axios.get(`https://asia.api.riotgames.com/riot/account/v1/accounts/by-riot-id/${닉네임.value}/${태그.value}?api_key=${API_KEY}`)
            .then(function (response) {
                console.log(response);
                puuid = response.data.puuid

                document.querySelector(".player_info h1").textContent = response.data.gameName +"#" + response.data.tagLine
            })

            // 2. SUMMONER API 들어감 : 유저의 레벨, 프로필이미지, id
            await axios.get(`https://kr.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/${puuid}?api_key=${API_KEY}`)
            .then(function (response) {
                console.log(response);
                레벨 = response.data.summonerLevel
                프사번호 = response.data.profileIconId
                id = response.data.id

                document.querySelector(".player_info h2 span").textContent = 레벨 //레벨 변경
                document.querySelector(".player img").setAttribute("src", `https://opgg-static.akamaized.net/meta/images/profile_icons/profileIcon${프사번호}.jpg`) // 프사 변경
            })

            // 3-1. LEAGUE API 들어감 : 티어, 승패 등등의 전적
            await axios.get(`https://kr.api.riotgames.com/lol/league/v4/entries/by-summoner/${id}?api_key=${API_KEY}`)
            .then(function (response) {
                console.log(response);

                // 솔랭 데이터 변경
                if(response.data[0] != undefined) {
                    const 솔랭이미지 = document.querySelector(".player_menu .solo img")
                    솔랭이미지.setAttribute("src", `https://opgg-static.akamaized.net/images/medals_new/${(response.data[0].tier).toLowerCase()}.png`)

                    document.querySelector(".solo .win").textContent = response.data[0].wins //솔랭 승리
                    document.querySelector(".solo .lose").textContent = response.data[0].losses //솔랭 패배
                    document.querySelector(".solo .rate").textContent = (response.data[0].wins / (response.data[0].wins + response.data[0].losses) * 100).toFixed(2)  // 솔랭 승률
                }

                // 자랭 데이터 변경
                if(response.data[1] != undefined && response.data[1].queueType == "RANKED_FLEX_SR") {
                    const 자랭이미지 = document.querySelector(".player_menu .flex img")
                    자랭이미지.setAttribute("src", `https://opgg-static.akamaized.net/images/medals_new/${(response.data[1].tier).toLowerCase()}.png`) // 티어이미지 변경

                    document.querySelector(".flex .win").textContent = response.data[1].wins //자랭 승리
                    document.querySelector(".flex .lose").textContent = response.data[1].losses //자랭 패배
                    document.querySelector(".flex .rate").textContent = (response.data[1].wins / (response.data[1].wins + response.data[1].losses) * 100).toFixed(2) // 자랭 승률
                }
                else if (response.data[2] != undefined && response.data[2].queueType == "RANKED_FLEX_SR") {
                    const 자랭이미지 = document.querySelector(".player_menu .flex img")
                    자랭이미지.setAttribute("src", `https://opgg-static.akamaized.net/images/medals_new/${(response.data[2].tier).toLowerCase()}.png`) // 티어이미지 변경

                    document.querySelector(".flex .win").textContent = response.data[2].wins //자랭 승리
                    document.querySelector(".flex .lose").textContent = response.data[2].losses //자랭 패배
                    document.querySelector(".flex .rate").textContent = (response.data[2].wins / (response.data[2].wins + response.data[2].losses) * 100).toFixed(2) // 자랭 승률
                }
            })

            // 3-2. MATCH API 들어감 : puuid로 20개 게임 불러오기
            await axios.get(`https://asia.api.riotgames.com/lol/match/v5/matches/by-puuid/${puuid}/ids?start=0&count=20&api_key=${API_KEY}`)
            .then(async function (response) {
                console.log(response);

                // 20개 게임의 코드 불러오기
                let 코드들20개 = response.data
                console.log(코드들20개);


                // 각 게임의 코드를 가지고 게임데이터 20개를 하나씩 가져옴
                for(let i=0; i<=19; i = i+1) {
                    await 게임데이터가져오기(코드들20개[i])
                }
            })

                // 20개 게임을 다 불러온 후, 승률 계산
                const 승 = document.querySelector(".summary_menu .record h2 .win")
                const 패 = document.querySelector(".summary_menu .record h2 .lose")
                const 승률 = document.querySelector(".summary_menu .record h2 .rate")
                승률.textContent = (Number(승.textContent) / (Number(승.textContent) + Number(패.textContent)) * 100).toFixed(2)
                
                const kda = document.querySelector(".summary_menu .record h2 .kda")
                const total_kill = document.querySelector(".summary_menu .record p .kill")
                const total_death = document.querySelector(".summary_menu .record p .death")
                const total_assist = document.querySelector(".summary_menu .record p .assist")
                kda.textContent = (Number(total_kill.textContent) + Number(total_assist.textContent)) / Number(total_death.textContent)
                kda.textContent = Number(kda.textContent).toFixed(2) + ":1"
                total_kill.textContent = Number(total_kill.textContent / 20)
                total_death.textContent = Number(total_death.textContent / 20)
                total_assist.textContent = Number(total_assist.textContent / 20)

                console.log(position)

                document.querySelector(".top span").textContent = position.TOP
                document.querySelector(".jungle span").textContent = position.JUNGLE
                document.querySelector(".mid span").textContent = position.MIDDLE
                document.querySelector(".bot span").textContent = position.BOTTOM
                document.querySelector(".supporter span").textContent = position.SUPPORT
                document.querySelector(".etc span").textContent = position.Invalid
        })

        async function 게임데이터가져오기( 매치코드 ) {
            await axios.get(`https://asia.api.riotgames.com/lol/match/v5/matches/${매치코드}?api_key=${API_KEY}`)
            .then(function (response) {
                console.log(response)

                let 게임모드
                if(response.data.info.queueId == 490) { //일반게임
                    게임모드 = "일반"
                }
                else if (response.data.info.queueId == 450) { // 칼바람
                    게임모드 = "ARAM"
                }
                else if (response.data.info.queueId == 440) { // 자랭
                    게임모드 = "자유랭크"
                }
                else if (response.data.info.queueId == 420) { // 솔랭
                    게임모드 = "솔로랭크"
                }
                else if (response.data.info.queueId == 1810 || response.data.info.queueId == 1830 || response.data.info.queueId == 1840) { // 집중포화
                    게임모드 = "집중포화"
                }

                let win, 포지션, 챔피언, 레벨, 룬1, 룬2, kill, death, assist, kda, cs, gold, item0, item1, item2, item3, item4, item5, item6
                for(let i=0; i<=9; i = i+1) { // 10개 유저들의 데이터 스캔
                    if(response.data.info.participants[i].puuid == puuid) { // 이 조건이 성립하는 사람이 오제무
                        console.log(response.data.info.participants[i].riotIdGameName)
                        console.log(i)
                        console.log("게임모드", 게임모드)
                        console.log("챔피언", response.data.info.participants[i].championName)

                        win = response.data.info.participants[i].win // 승리여부
                        챔피언 = response.data.info.participants[i].championName // 챔피언 픽
                        레벨 = response.data.info.participants[i].champLevel // 레벨
                        // 멀티킬
                        if(response.data.info.participants[i].pentaKills >= 1) {
                            멀티킬 = "펜타킬"
                        }
                        else if (response.data.info.participants[i].quadraKills >= 1) {
                            멀티킬 = "쿼드라킬"
                        }
                        else if (response.data.info.participants[i].tripleKills >= 1) {
                            멀티킬 = "트리플킬"
                        }
                        else if (response.data.info.participants[i].doubleKills >= 1) {
                            멀티킬 = "더블킬"
                        }
                        else {
                            멀티킬 = "없음"
                        }
                        룬1 = response.data.info.participants[i].perks.styles[0].selections[0].perk //룬1
                        룬2 = response.data.info.participants[i].perks.styles[1].style //룬2
                        kill = response.data.info.participants[i].kills // kill
                        death = response.data.info.participants[i].deaths // death
                        assist = response.data.info.participants[i].assists // assist
                        kda = (response.data.info.participants[i].kills + response.data.info.participants[i].assists) / response.data.info.participants[i].deaths // kda
                        cs = response.data.info.participants[i].totalMinionsKilled + response.data.info.participants[i].totalAllyJungleMinionsKilled + response.data.info.participants[i].totalEnemyJungleMinionsKilled // cs
                        gold = response.data.info.participants[i].goldEarned //gold
                        item0 = response.data.info.participants[i].item0 // 아이템
                        item1 = response.data.info.participants[i].item1 // 아이템
                        item2 = response.data.info.participants[i].item2 // 아이템
                        item3 = response.data.info.participants[i].item3 // 아이템
                        item4 = response.data.info.participants[i].item4 // 아이템
                        item5 = response.data.info.participants[i].item5 // 아이템
                        item6 = response.data.info.participants[i].item6 // 아이템

                        포지션 = response.data.info.participants[i].individualPosition
                        console.log(포지션)
                        position[포지션] += 1

                        document.querySelector(".summary_menu .record p .kill").textContent = Number(document.querySelector(".summary_menu .record p .kill").textContent) + kill
                        document.querySelector(".summary_menu .record p .death").textContent = Number(document.querySelector(".summary_menu .record p .death").textContent) + death
                        document.querySelector(".summary_menu .record p .assist").textContent = Number(document.querySelector(".summary_menu .record p .assist").textContent) + assist
                        break; 
                    }
                }

                // 페이지에 게임 정보를 div태그로 만들어서 집어넣어야 함
                // 1. div 태그 생성
                let 게임 = document.createElement("div")
                게임.classList.add("game")
                                
                if(win == true) { // 지거나 이기거나에 따라 
                    게임.classList.add("victory") 
                    document.querySelector(".summary_menu .record h2 .win").textContent = Number(document.querySelector(".summary_menu .record h2 .win").textContent) + 1
                }
                else {
                    게임.classList.add("defeat") 
                    document.querySelector(".summary_menu .record h2 .lose").textContent = Number(document.querySelector(".summary_menu .record h2 .lose").textContent) + 1
                }

                // 집중포화인 경우 그냥 끝냄
                if(게임모드 == "집중포화") {
                    게임.innerHTML = `
                    <div class="mod">
                        <h1>${게임모드}</h1>
                    </div> `
                    const 게임20개들의부모 = document.querySelector(".game20_menu")
                    게임20개들의부모.appendChild(게임)
                    return 0;
                }
                
                // 2. 내용을 쭉 수정
                게임.innerHTML = `      
                <div class="mod">${게임모드}</div>
                <div class="champion">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/champion/${챔피언}.png" alt="챔피언프사">
                    <p>레벨 <span>${레벨}</span></p>
                </div>
                <div class="multikill">${멀티킬}</div>
                <div class="rune">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/perk/${룬1}.png" class="rune1" alt="룬1">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/perkStyle/${룬2}.png" class="rune2" alt="룬2">
                </div>
                <div class="score">
                    <p><span class="kda">${kda.toFixed(2)+":1"}</span> <br> <span class="kill">${kill}</span> / <span class="death">${death}</span> / <span class="assist">${assist}</span></p>
                    <p>GOLD <span class="gold">${gold}</span></p>
                    <p>CS <span class="cs">${cs}</span></p>
                </div>
                <div class="item">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item0}.png" class="item1" onerror="this.src='https://www.trendsintile.com/plogger/plog-content/thumbs/signature-ceramic/color--dimensions-4x16-colors/large/6642-dk_grey_mt.jpg'">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item1}.png" class="item2" onerror="this.src='https://www.trendsintile.com/plogger/plog-content/thumbs/signature-ceramic/color--dimensions-4x16-colors/large/6642-dk_grey_mt.jpg'">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item2}.png" class="item3" onerror="this.src='https://www.trendsintile.com/plogger/plog-content/thumbs/signature-ceramic/color--dimensions-4x16-colors/large/6642-dk_grey_mt.jpg'">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item3}.png" class="item4" onerror="this.src='https://www.trendsintile.com/plogger/plog-content/thumbs/signature-ceramic/color--dimensions-4x16-colors/large/6642-dk_grey_mt.jpg'">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item4}.png" class="item5" onerror="this.src='https://www.trendsintile.com/plogger/plog-content/thumbs/signature-ceramic/color--dimensions-4x16-colors/large/6642-dk_grey_mt.jpg'">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item5}.png" class="item6" onerror="this.src='https://www.trendsintile.com/plogger/plog-content/thumbs/signature-ceramic/color--dimensions-4x16-colors/large/6642-dk_grey_mt.jpg'">
                    <img src="https://opgg-static.akamaized.net/meta/images/lol/14.14.1/item/${item6}.png" class="item6" >
                </div>
                <div class="users">
                    <div class="team1">
                        <p class="user1">${response.data.info.participants[0].riotIdGameName}</p>
                        <p class="user2">${response.data.info.participants[1].riotIdGameName}</p>
                        <p class="user3">${response.data.info.participants[2].riotIdGameName}</p>
                        <p class="user4">${response.data.info.participants[3].riotIdGameName}</p>
                        <p class="user5">${response.data.info.participants[4].riotIdGameName}</p>
                    </div>
                    <div class="team2">
                        <p class="user1">${response.data.info.participants[5].riotIdGameName}</p>
                        <p class="user2">${response.data.info.participants[6].riotIdGameName}</p>
                        <p class="user3">${response.data.info.participants[7].riotIdGameName}</p>
                        <p class="user4">${response.data.info.participants[8].riotIdGameName}</p>
                        <p class="user5">${response.data.info.participants[9].riotIdGameName}</p>
                    </div>
                </div>`

                // 3. 생성한 태그를 .game20_menu 에다가 자식으로 집어넣어야 함
                const 게임20개들의부모 = document.querySelector(".game20_menu")
                게임20개들의부모.appendChild(게임)
            })

        }

    </script>
</body>
</html>
