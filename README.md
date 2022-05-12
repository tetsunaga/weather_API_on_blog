# weather_API_on_blog
1.概要
local strageの課題にweather APIの天気と気温のデータを表示できるようにしました。
2.工夫した点
ウェブサイトでweatherAPIを検索して比較、登録がしやすく、信頼性が高く取り込み簡単そうなweatherAPIを選び、コードを移植しました。表示については悪戦苦闘しましが、
まえたつさんに教えてもらいfunction ShowTodaysweather(response){
let obj=JSON.prise(response);
let weather = obj.weather[0].description;
let city = obj.name;
let temp =obj.main.temp;省略
const dom=document.getElementById("target");
dom.inner TEXT=Wで表示できるようになりました。
3.苦労した点
APIオブジェクトを取り込んで表示できるまで何度もトライした点でなんとか表示できるようになりました。
