# 游戏音乐与配音

下列配乐均由 Kevin MacLeod 发布（incompetech.com），采用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 授权。《Gymnopedie No. 1》原曲为 Erik Satie。所有片段约 49 秒，经过剪辑、响度处理和首尾淡化。进入新场景时，游戏会交叉淡化两段配乐。原音源和作者见各曲的官方页面。

| 曲目 | 游戏用途 | 原始出处 | 剪辑位置 |
| --- | --- | --- | --- |
| Gymnopedie No. 1 | 校门序曲 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100787) | 8 秒起 |
| Carefree | 报到与社团 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1400037) | 12 秒起 |
| Almost in F | 图书馆与自习 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100394) | 21 秒起 |
| Unwritten Return | 实验与复验 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1500037) | 36 秒起 |
| Bossa Antigua | 社区与食堂 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1700069) | 18 秒起 |
| Easy Lemon (60 second) | 宿舍与朋友 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1200077) | 0 秒起 |
| Clean Soul | 附院与见习 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1300033) | 16 秒起 |
| Touching Moments Two - Higher | 约会与靠近 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100037) | 12 秒起 |
| Touching Moments Four - Melody | 和解与信任 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100040) | 12 秒起 |
| Heartbreaking | 关系分歧 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100208) | 7 秒起 |
| Darkest Child | 异闻与疑点 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100783) | 18 秒起 |
| Lightless Dawn | 恐怖调查 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100655) | 54 秒起 |
| The Dread | 恐怖升级 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100048) | 25 秒起 |
| Prelude and Action | 考核与转折 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100887) | 17 秒起 |
| Long Road Ahead | 毕业与离别 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100588) | 20 秒起 |
| Reunited | 重逢与结局 | [Incompetech](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1200068) | 14 秒起 |

游戏对白使用 [Sherpa-ONNX](https://github.com/k2-fsa/sherpa-onnx) 文档列出的 [AISHELL-3 多说话人 VITS 模型](https://k2-fsa.github.io/sherpa/onnx/tts/pretrained_models/vits.html) 合成。[AISHELL-3 普通话语料](https://www.openslr.org/93/)由 Beijing Shell Shell Technology Co., Ltd. 发布，采用 Apache License 2.0。游戏包附带合成台词音频和生成脚本。不同角色采用不同的模型说话人编号，各种情绪使用不同语速、音高与句内曲线。本版提供 16 套声线，涵盖十二位角色、两种主角、教师及旁白。配音为合成表演。运行时不需要模型或网络服务。未随包生成的动态文本可使用设备提供的本地普通话语音。

音源重建可用 `node scripts/voice-script.mjs` 导出台词清单，再调用 `scripts/render-voices.py`。四个参数依次为模型目录、台词清单、输出目录、音频索引路径。模型目录需要 Sherpa 文档的 vits-icefall-zh-aishell3 文件。
