<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ギャングカラー検索</title>

<style>
body {
  margin: 0;
  background: #0a0a0a;
  color: white;
  font-family: sans-serif;
}

.container {
  max-width: 1000px;
  margin: auto;
  padding: 20px;
}

input {
  width: 100%;
  padding: 12px;
  border-radius: 10px;
  border: none;
  margin-bottom: 20px;
  background: #111;
  color: white;
}

.card {
  background: #111;
  border-radius: 12px;
  padding: 15px;
  margin-bottom: 10px;
}

button {
  padding: 6px 10px;
  border: none;
  border-radius: 6px;
  background: #333;
  color: white;
  cursor: pointer;
}
</style>
</head>

<body>
<div class="container">

<h1>🎨 ギャングカラー検索</h1>

<input id="search" placeholder="検索：青 / RGB / チーム名">

<div id="list"></div>

</div>

<script>
const gangs = [
{
name:"lvy半グレ",
main:"アノダイズドパープル",
sub:"アノダイズドパープル",
pear:"スピネーカーパープル",
tags:"紫 パープル"
},
{
name:"Fisher",
main:"アノダイズドブルー",
sub:"-",
pear:"-",
tags:"青 ブルー"
},
{
name:"オレンジギャング",
main:"オレンジ",
sub:"-",
pear:"-",
tags:"オレンジ"
},
{
name:"白ギャング",
main:"アイスホワイト",
sub:"-",
pear:"-",
tags:"白"
},
{
name:"水色ギャング",
main:"RGB(34,158,186)",
sub:"RGB(34,158,186)",
pear:"ブラック",
tags:"水色"
},
{
name:"黄緑半グレ",
main:"ライムグリーン",
sub:"ライムグリーン",
pear:"ブラック",
tags:"黄緑"
},
{
name:"ノーネーム",
main:"シャフターパープル",
sub:"ライムグリーン",
pear:"シャフターパープル",
tags:"紫"
},
{
name:"影班",
main:"モノクローム",
sub:"モノクローム",
pear:"モノクローム",
tags:"黒 白"
},
{
name:"青半グレ",
main:"ブルー",
sub:"ブルー",
pear:"フブキ",
tags:"青"
},
{
name:"ピンク",
main:"RGB(245,150,189)",
sub:"RGB(245,150,189)",
pear:"ホットピンク",
tags:"ピンク"
}
];

const list = document.getElementById("list");
const search = document.getElementById("search");

function render(data){
  list.innerHTML = "";
  data.forEach(g=>{
    const div = document.createElement("div");
    div.className="card";
    div.innerHTML = `
      <b>${g.name}</b><br>
      メイン: ${g.main}<br>
      サブ: ${g.sub}<br>
      パール: ${g.pear}<br>
      <button onclick="copy('${g.name}\\n${g.main}')">コピー</button>
    `;
    list.appendChild(div);
  });
}

function copy(text){
  navigator.clipboard.writeText(text);
}

search.addEventListener("input",()=>{
  const q = search.value.toLowerCase();
  const filtered = gangs.filter(g =>
    (g.name + g.main + g.tags).toLowerCase().includes(q)
  );
  render(filtered);
});

render(gangs);
</script>

</body>
</html>
