export default function GangColorApp() {
  const gangs = [
    {
      name: "lvy半グレ / まっくろくろす",
      aliases: ["lvy半グレ", "まっくろくろす", "パープル", "紫"],
      main: "アノダイズドパープル（カメレオン）",
      sub: "アノダイズドパープル（カメレオン）",
      pearlescent: "スピネーカーパープル（メタリック）",
      note: "紫系"
    },
    {
      name: "Fisher（青ギャング）",
      aliases: ["Fisher", "青ギャング", "青", "ブルー"],
      main: "アノダイズドブルー（カメレオン）",
      sub: "-",
      pearlescent: "-",
      note: "青系"
    },
    {
      name: "オレンジギャング",
      aliases: ["オレンジギャング", "オレンジ"],
      main: "オレンジ（マット）",
      sub: "-",
      pearlescent: "-",
      note: "オレンジ系"
    },
    {
      name: "Lui白 / アデルウルフ",
      aliases: ["Lui", "白", "アデルウルフ", "ミッドナイトブルー"],
      main: "ミッドナイトブルー（マット）",
      sub: "-",
      pearlescent: "ブラック（マット）",
      note: "白系呼称あり"
    },
    {
      name: "ばり紫",
      aliases: ["ばり紫", "紫", "パープル"],
      main: "アノダイズドパープル（カメレオン）",
      sub: "アノダイズドパープル（カメレオン）",
      pearlescent: "オフホワイト（カメレオン）",
      note: "紫系"
    },
    {
      name: "白ギャング",
      aliases: ["白ギャング", "白", "ホワイト"],
      main: "アイスホワイト",
      sub: "-",
      pearlescent: "-",
      note: "白系"
    },
    {
      name: "水色（旧水色ではない方）",
      aliases: ["水色", "新水色", "旧水色ではない方", "RGB(34,158,186)"],
      main: "RGB(34,158,186)",
      sub: "RGB(34,158,186)",
      pearlescent: "ブラック（マット）",
      note: "水色系"
    },
    {
      name: "水色ギャング",
      aliases: ["水色ギャング", "水色", "フブキ"],
      main: "フブキ（カメレオン）",
      sub: "フブキ（カメレオン）",
      pearlescent: "-",
      note: "水色系"
    },
    {
      name: "水色（おやま半ぐれ）",
      aliases: ["水色", "おやま半ぐれ", "RGB(143,229,255)"],
      main: "RGB(143,229,255)",
      sub: "RGB(143,229,255)",
      pearlescent: "アイスホワイト（メタリック）",
      note: "水色系"
    },
    {
      name: "空色",
      aliases: ["空色", "ライトブルー"],
      main: "55.ライトブルー（メタリック）",
      sub: "アイスホワイト（メタリック）",
      pearlescent: "アイスホワイト（メタリック）",
      note: "空色系"
    },
    {
      name: "黄緑半グレ",
      aliases: ["黄緑半グレ", "黄緑", "ライムグリーン"],
      main: "ライムグリーン（メタリック）",
      sub: "ライムグリーン（メタリック）",
      pearlescent: "ブラック（メタリック）",
      note: "黄緑系"
    },
    {
      name: "緑半ぐれ（白上さん）",
      aliases: ["緑半ぐれ", "白上さん", "ミッドナイトパープル"],
      main: "ミッドナイトパープル（マット）",
      sub: "ミッドナイトパープル（マット）",
      pearlescent: "ウルトラブルー（メタリック）",
      note: "名称は緑だが実色は紫寄り"
    },
    {
      name: "ザウバー",
      aliases: ["ザウバー", "RGB(0,50,50)", "青緑"],
      main: "RGB(0,50,50)（クラシック）",
      sub: "ブラック（メタリック）",
      pearlescent: "シルバー（メタリック）",
      note: "深青緑系"
    },
    {
      name: "青緑半ぐれ",
      aliases: ["青緑半ぐれ", "青緑", "グラファイト"],
      main: "グラファイト（メタリック）",
      sub: "ブラック（メタリック）",
      pearlescent: "ミッドナイトシルバー（メタリック）",
      note: "青緑系"
    },
    {
      name: "かすみさん半ぐれ",
      aliases: ["かすみさん半ぐれ", "RGB(14,43,43)", "RGB(8,8,8)"],
      main: "RGB(14,43,43)",
      sub: "RGB(8,8,8)",
      pearlescent: "アノダイズトグリーン（カメレオン）",
      note: "深緑黒系"
    },
    {
      name: "ノーネーム（紫ギャング）",
      aliases: ["ノーネーム", "紫ギャング", "シャフターパープル"],
      main: "メタリック シャフターパープル",
      sub: "メタリック ライムグリーン",
      pearlescent: "マット シャフターパープル",
      note: "紫＋黄緑"
    },
    {
      name: "影班（ロギアさん）",
      aliases: ["影班", "ロギアさん", "モノクローム"],
      main: "モノクローム（カメレオン）",
      sub: "モノクローム（カメレオン）",
      pearlescent: "モノクローム（カメレオン）",
      note: "モノクロ系"
    },
    {
      name: "青半グレ（かぶさん）",
      aliases: ["青半グレ", "かぶさん", "ブルー"],
      main: "ブルー（メタリック）",
      sub: "ブルー（メタリック）",
      pearlescent: "フブキ（カメレオン）",
      note: "青系"
    },
    {
      name: "茶色（リップ）",
      aliases: ["茶色", "リップ", "RGB(61,52,44)"],
      main: "RGB(61,52,44)",
      sub: "RGB(61,52,44)",
      pearlescent: "パイソンブラウン（メタリック）",
      note: "茶系"
    },
    {
      name: "黄色",
      aliases: ["黄色", "イエロー", "レースイエロー"],
      main: "レースイエロー（メタリック）",
      sub: "レースイエロー（メタリック）",
      pearlescent: "-",
      note: "黄系"
    },
    {
      name: "ピンク（Rosalia）",
      aliases: ["ピンク", "Rosalia", "RGB(245,150,189)", "RGB(174,165,212)"],
      main: "RGB(245,150,189) / RGB(174,165,212)",
      sub: "RGB(245,150,189)",
      pearlescent: "ホットピンク（メタリック）",
      note: "ピンク系"
    }
  ];

  const [query, setQuery] = React.useState("");
  const [copied, setCopied] = React.useState("");

  const normalized = (text) =>
    String(text || "")
      .toLowerCase()
      .replace(/[（）()\s　\-]/g, "");

  const filtered = gangs.filter((gang) => {
    const haystack = [
      gang.name,
      gang.main,
      gang.sub,
      gang.pearlescent,
      gang.note,
      ...(gang.aliases || []),
    ]
      .join(" ")
      .toLowerCase();

    return normalized(haystack).includes(normalized(query));
  });

  const copyText = async (gang) => {
    const text = `【${gang.name}】\nメイン: ${gang.main}\nサブ: ${gang.sub}\nパールセント: ${gang.pearlescent}`;
    try {
      await navigator.clipboard.writeText(text);
      setCopied(gang.name);
      setTimeout(() => setCopied(""), 1800);
    } catch (e) {
      console.error(e);
    }
  };

  const statStyle = "rounded-2xl border border-white/10 bg-white/5 px-4 py-3 shadow-sm";
  const cardStyle = "rounded-3xl border border-white/10 bg-white/5 p-5 shadow-xl backdrop-blur";

  return (
    <div className="min-h-screen bg-neutral-950 text-white">
      <div className="mx-auto max-w-7xl px-4 py-6 md:px-8 md:py-10">
        <div className="mb-6 grid gap-4 md:grid-cols-[1.4fr_0.6fr]">
          <div className="rounded-3xl border border-white/10 bg-gradient-to-br from-white/10 to-white/5 p-6 shadow-2xl">
            <div className="mb-2 text-sm text-white/60">FiveM / Gang Color Search App</div>
            <h1 className="text-3xl font-bold tracking-tight md:text-4xl">ギャングカラー検索</h1>
            <p className="mt-3 max-w-3xl text-sm leading-6 text-white/70 md:text-base">
              チーム名、色名、RGB、通称で即ヒット。現場で「どの色やっけ？」が一瞬で片づく、街のカラーレーダーです。
            </p>
          </div>

          <div className="grid gap-3 md:grid-cols-1">
            <div className={statStyle}>
              <div className="text-xs text-white/50">登録チーム数</div>
              <div className="mt-1 text-2xl font-bold">{gangs.length}</div>
            </div>
            <div className={statStyle}>
              <div className="text-xs text-white/50">検索結果</div>
              <div className="mt-1 text-2xl font-bold">{filtered.length}</div>
            </div>
          </div>
        </div>

        <div className="mb-6 rounded-3xl border border-white/10 bg-white/5 p-4 shadow-xl">
          <div className="grid gap-3 md:grid-cols-[1fr_auto]">
            <input
              value={query}
              onChange={(e) => setQuery(e.target.value)}
              placeholder="検索: チーム名 / 色 / RGB / 通称 例) 青、ロギア、RGB(34,158,186)"
              className="w-full rounded-2xl border border-white/10 bg-neutral-900 px-4 py-3 text-sm outline-none ring-0 placeholder:text-white/35 focus:border-white/25"
            />
            <button
              onClick={() => setQuery("")}
              className="rounded-2xl border border-white/10 bg-white/10 px-4 py-3 text-sm font-medium transition hover:bg-white/15"
            >
              クリア
            </button>
          </div>
        </div>

        <div className="grid gap-4 md:grid-cols-2 xl:grid-cols-3">
          {filtered.map((gang) => (
            <div key={gang.name} className={cardStyle}>
              <div className="mb-3 flex items-start justify-between gap-3">
                <div>
                  <h2 className="text-lg font-semibold leading-6">{gang.name}</h2>
                  <p className="mt-1 text-xs text-white/50">{gang.note}</p>
                </div>
                <button
                  onClick={() => copyText(gang)}
                  className="rounded-xl border border-white/10 bg-white/10 px-3 py-2 text-xs font-medium transition hover:bg-white/15"
                >
                  {copied === gang.name ? "コピー済" : "コピー"}
                </button>
              </div>

              <div className="space-y-2 text-sm">
                <div className="rounded-2xl bg-neutral-900/80 p-3">
                  <div className="text-xs text-white/45">メイン</div>
                  <div className="mt-1 font-medium">{gang.main}</div>
                </div>
                <div className="rounded-2xl bg-neutral-900/80 p-3">
                  <div className="text-xs text-white/45">サブ</div>
                  <div className="mt-1 font-medium">{gang.sub}</div>
                </div>
                <div className="rounded-2xl bg-neutral-900/80 p-3">
                  <div className="text-xs text-white/45">パールセント</div>
                  <div className="mt-1 font-medium">{gang.pearlescent}</div>
                </div>
                <div className="rounded-2xl bg-neutral-900/80 p-3">
                  <div className="text-xs text-white/45">検索タグ</div>
                  <div className="mt-1 text-white/80">{gang.aliases.join(" / ")}</div>
                </div>
              </div>
            </div>
          ))}
        </div>

        {filtered.length === 0 && (
          <div className="rounded-3xl border border-dashed border-white/15 bg-white/5 p-10 text-center text-white/60">
            該当なし。検索ワードを変えてみてください。
          </div>
        )}
      </div>
    </div>
  );
}
