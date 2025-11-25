---
title: "UI-TARS-desktop by deepwiki"
source: "https://deepwiki.com/search/os_8af7664a-383e-4b07-af71-85272cfc361f"
author:
  - "[[DeepWiki]]"
published:
created: 2025-05-12
description: "DeepWiki provides up-to-date documentation you can talk to, for every repo in the world. Think Deep Research for GitHub - powered by Devin."
tags:
  - "clippings"
---
[Powered by Devin](https://devin.ai/)

[DeepWiki](https://deepwiki.com/)

[return to bytedance/UI-TARS-desktop](https://deepwiki.com/bytedance/UI-TARS-desktop)

利用できるOSは何ですか？

Fast

Searched across bytedance/UI-TARS-desktop

## Answer

UI-TARS Desktopは以下のオペレーティングシステムをサポートしています：

1. **Windows**
2. **macOS**
3. **ブラウザ** （ブラウザベースの実装としても利用可能） README.md:50

UI-TARS Desktopはクロスプラットフォームアプリケーションとして設計されており、Electronフレームワークを使用して構築されています。これにより、Windows、macOSなど複数のプラットフォームで動作することが可能になっています。

## プラットフォーム固有の情報

### Windows

- Windows x64アーキテクチャ向けのビルドがサポートされています
- Windows ARMアーキテクチャ向けのビルドもサポートされています CONTRIBUTING.md:140-143

### macOS

- macOS x64（Intel）アーキテクチャ向けのビルドがサポートされています
- macOS ARM（Apple Silicon）アーキテクチャ向けのビルドもサポートされています CONTRIBUTING.md:140-141

### ブラウザ

READMEには「Browser」もサポートされているプラットフォームとして記載されています。これはMidsceneという名前のブラウザベースの実装を通じて利用可能です。 README.md:26-27

## リリースワークフローでサポートされているプラットフォーム

現在のリリースワークフローでは、以下のプラットフォームが公式にサポートされています：

- MacOS x64
- MacOS arm64
- Windows x64 CONTRIBUTING.md:155-159

## インストール方法

### macOS

macOSでは、アプリケーションを「Applications」フォルダにドラッグしてインストールします。また、Homebrewを使用してインストールすることも可能です：

```
brew install --cask ui-tars
```

quick-start.md:13-16

### Windows

Windowsでは、インストーラーを実行してアプリケーションをインストールします。 quick-start.md:36-40

## Notes

UI-TARS Desktopは主にWindows（x64およびARM）とmacOS（Intel x64およびApple Silicon ARM）をサポートしています。また、ブラウザベースの実装（Midscene）も存在します。リリースワークフローでは現在、MacOS x64、MacOS arm64、Windows x64が公式にサポートされています。

Wiki pages you might want to explore:

- [Development Guide (bytedance/UI-TARS-desktop)](https://deepwiki.com/bytedance/UI-TARS-desktop/9-development-guide)

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [CONTRIBUTING.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/CONTRIBUTING.md)

```
137
Run \`pnpm run build\` in current system, it will output into \`out/*\` directory.
138

139
To build the products of other systems, run:
```

```
140
- Mac x64: \`pnpm run publish:mac-x64\`
141
- Mac ARM: \`pnpm run publish:mac-arm64\`
142
- Windows x64: \`pnpm run publish:win32\`
143
- Windows ARM: \`pnpm run publish:win32-arm64\`
```

```
144

145
### Release
146
```

```
152
2. Git commit and push to the \`release/${version}\` branch, create a PR targeting \`main\` branch, titled \`release(app): ${version}\`
153
3. Trigger the release [workflow](https://github.com/bytedance/UI-TARS-desktop/actions/workflows/release.yml) manually after the PR is merged
154
```

```
155
Currently, the release workflow supports the following platforms:
156

157
- MacOS x64
158
- MacOS arm64
159
- Windows x64
```

```
160

161
#### Packages
162
```

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [docs/quick-start.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/docs/quick-start.md)

```
10

11
You can download the [latest release](https://github.com/bytedance/UI-TARS-desktop/releases/latest) version of UI-TARS Desktop from our releases page.
12
```

```
13
> **Note**: If you have [Homebrew](https://brew.sh/) installed, you can install UI-TARS Desktop by running the following command:
14
> \`\`\`bash
15
> brew install --cask ui-tars
16
> \`\`\`
```

```
17

18
<br />
19
```

```
33
  <img src="../apps/ui-tars/images/mac_app.png" width="500px" />
34

35
```

```
36
### Windows
37

38
**Still to run** the application, you can see the following interface:
39

40
<img src="../apps/ui-tars/images/windows_install.png" width="400px" style="margin-left: 4em;" />
```

```
41

42
<br />
43
```

[return to bytedance/UI-TARS-desktop](https://deepwiki.com/bytedance/UI-TARS-desktop)

使われている生成AIのモデルは何ですか？自分で設定できますか？

Fast

Searched across bytedance/UI-TARS-desktop

## Answer

UI-TARS Desktopで使用されている生成AIモデルについてお答えします。

## 使用されている生成AIモデル

UI-TARS Desktopでは、主に以下の生成AIモデルがサポートされています：

1. **UI-TARS-1.0シリーズ**
	- UI-TARS-2B-SFT
	- UI-TARS-7B-SFT
	- UI-TARS-7B-DPO
	- UI-TARS-72B-SFT
	- UI-TARS-72B-DPO bug\_report\_ui\_tars\_desktop.yml:19-23
2. **UI-TARS-1.5シリーズ**
	- UI-TARS-1.5-7B（Hugging Faceで利用可能） quick-start.md:51-52
3. **Doubao-1.5-UI-TARS** （VolcEngine/火山引擎で利用可能） quick-start.md:87

## モデルの自分での設定方法

はい、UI-TARS Desktopでは使用するAIモデルを自分で設定することができます。設定方法は以下の通りです：

### 設定画面へのアクセス

アプリケーションの左下にある設定ボタンをクリックして設定画面を開きます。 quick-start.md:17-19

### モデル設定オプション

設定画面の「AI Models Settings」タブで以下の項目を設定できます： SettingsModal.tsx:152-155

1. **言語（Language）** ：
	- 英語（en）または中国語（zh）を選択できます setting.md:26-29
2. **VLMプロバイダー（VLM Provider）** ：
	- `OpenAI compatible for UI-TARS-1.0`
	- `OpenAI compatible for UI-TARS-1.5`
	- `VolcEngine Ark for Doubao-1.5-UI-TARS` setting.md:42-45
3. **VLM Base URL** ：
	- モデルのAPIエンドポイントURLを指定します setting.md:61-64
4. **VLM API KEY** ：
	- モデルのAPIキーを指定します setting.md:76-79
5. **VLM Model Name** ：
	- 使用するモデル名を指定します setting.md:89-92

### カスタムモデル名の使用

標準で提供されているモデル以外にも、カスタムモデル名を使用することができます。設定画面で「Use custom model name」スイッチをオンにすると、任意のモデル名を入力できるようになります。 ModelSettingsTab.tsx:215-222

### 設定例

#### Hugging Faceの例（UI-TARS-1.5）

```
Language: en  
VLM Provider: OpenAI compatible for UI-TARS-1.5  
VLM Base URL: https:xxx  
VLM API KEY: hf_xxx  
VLM Model Name: tgi
```

setting.md:101-107

#### VolcEngine（火山引擎）の例（Doubao-1.5-UI-TARS）

```
Language: cn  
VLM Provider: VolcEngine Ark for Doubao-1.5-UI-TARS  
VLM Base URL: ttps://ark.cn-beijing.volces.com/api/v3  
VLM API KEY: ARK_API_KEY  
VLM Model Name: doubao-1.5-ui-tars-250328
```

setting.md:113-119

## 重要な注意点

1. VLMプロバイダーの選択は、モデルのパフォーマンスと正確なGUIアクション実行に影響します。適切なプロバイダーを選択することが重要です。 setting.md:47-48
2. VLM Base URLはOpenAI互換のAPIエンドポイントである必要があります。 setting.md:66-67
3. UI-TARS-1.5を使用する場合は、VLMプロバイダーとして「OpenAI compatible for UI-TARS-1.5」を選択してください。 quick-start.md:66-67
4. Doubao-1.5-UI-TARSを使用する場合は、VLMプロバイダーとして「VolcEngine Ark for Doubao-1.5-UI-TARS」を選択してください。 quick-start.md:112-113

## Notes

UI-TARS Desktopでは、UI-TARS-1.0シリーズ、UI-TARS-1.5シリーズ、およびDoubao-1.5-UI-TARSなどの生成AIモデルをサポートしています。これらのモデルは設定画面から自分で設定することができ、言語、プロバイダー、Base URL、APIキー、モデル名などの項目を指定できます。適切なモデルとプロバイダーを選択することで、最適なパフォーマンスを得ることができます。

Wiki pages you might want to explore:

- [Architecture (bytedance/UI-TARS-desktop)](https://deepwiki.com/bytedance/UI-TARS-desktop/2-architecture)

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop)[.github/ISSUE\_TEMPLATE/bug\_report\_ui\_tars\_desktop.yml](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/.github/ISSUE_TEMPLATE/bug_report_ui_tars_desktop.yml)

```
16
    label: Model
17
    description: "Select the VLM being used when this issue occurred."
18
    options:
```

```
19
      - UI-TARS-2B-SFT
20
      - UI-TARS-7B-SFT
21
      - UI-TARS-7B-DPO
22
      - UI-TARS-72B-SFT
23
      - UI-TARS-72B-DPO
```

```
24
  validations:
25
    required: true
26
- type: dropdown
```

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [docs/quick-start.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/docs/quick-start.md)

```
48
1. Click the button \`Deploy from Hugging Face\` on the top right corner of the page
49
  <img src="../apps/ui-tars/images/quick_start/huggingface_deploy.png" width="500px" />
50
```

```
51
2. Select the model UI-TARS-1.5-7B
52
  <img src="../apps/ui-tars/images/quick_start/huggingface_uitars_1.5.png" width="500px" />
```

```
53

54
3. Refer to [README_deploy.md](https://github.com/bytedance/UI-TARS/blob/main/README_deploy.md) for detailed deployment instructions to obtain the **Base URL**, **API Key**, and **Model Name**.
55
```

```
63
VLM Model Name: xxx
64
\`\`\`
65
```

```
66
> [!NOTE]
67
> For VLM Provider, make sure to select "**OpenAI compatible for UI-TARS-1.5**" to ensure proper VLM Action parsing.
```

```
68

69
  <img src="../apps/ui-tars/images/quick_start/huggingface_setting.png" width="500px" />
70
```

```
84
### Doubao-1.5-UI-TARS on [VolcEngine](https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-1-5-ui-tars)
85

86
```

```
87
1. Visit the [VolcEngine Doubao-1.5-UI-TARS page](https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-1-5-ui-tars)
```

```
88

89

90
2. Click the button \`Try (立即体验)\` on the top right corner of the page
```

```
109
VLM Model Name: doubao-1.5-ui-tars-250328
110
\`\`\`
111
```

```
112
> [!NOTE]
113
> For VLM Provider, make sure to select "**VolcEngine Ark for Doubao-1.5-UI-TARS**" to ensure proper VLM Action parsing.
```

```
114

115
  <img src="../apps/ui-tars/images/quick_start/volcengine_settings.png" width="500px" />
116
```

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [apps/agent-tars/docs/quick-start.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/apps/agent-tars/docs/quick-start.md)

```
14
![accessibility-permission.png](https://github.com/user-attachments/assets/77e171d2-dffb-4905-98c0-92c5ab00e333)
15

16
```

```
17
You can click the left-bottom button to open the configuration page:
18

19
![setting-icon.png](https://lf3-static.bytednsdoc.com/obj/eden-cn/uhbfnupenuhf/agent-tars/setting-icon.jpeg)
```

```
20

21
Then you can set the model config and the search config.
22
```

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [docs/setting.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/docs/setting.md)

```
23
Controls localization settings for VLM.
24

25
| Property    | Details                        |
```

```
26
| ----------- | ------------------------------ |
27
| **Type**    | \`string\`                       |
28
| **Options** | \`en\` (English), \`zh\` (Chinese) |
29
| **Default** | \`en\`                           |
```

```
30

31
> [!NOTE]
32
> Changing the settings will **only** affect the output of VLM, not the language of the desktop app itself. Regarding the i18n of the App itself, welcome to contribute PR.
```

```
39
Select the backend VLM provider to ensure more accurate execution of GUI actions. This option can improve the performance of the model.
40

41
| Property    | Details                |
```

```
42
| ----------- | ---------------------- |
43
| **Type**    | \`string\`               |
44
| **Options** | - \`OpenAI compatible for UI-TARS-1.0\`<br /> - \`OpenAI compatible for UI-TARS-1.5\`<br /> - \`VolcEngine Ark for Doubao-1.5-UI-TARS\` |
45
| **Required** | \`true\`         |
```

```
46
```

```
47
> [!NOTE]
48
> This is an interface reserved for different VLM providers.
```

```
49

50

51
<br>
```

```
58

59
For UI TARS deployment, please check out [Deployment](./deployment.md).
60
```

```
61
| Property     | Details  |
62
|
 
------------
 
|
 
--------
 
|

63

| **Type**     | \`string\` |
64
| **Required** | \`true\`   |
```

```
65
```

```
66
> [!NOTE]
67
> VLM Base URL should be OpenAI compatible API endpoints (see [OpenAI API protocol document](https://platform.openai.com/docs/guides/vision/uploading-base-64-encoded-images) for more details).
```

```
68

69

70
<br>
```

```
73

74
Specify the vlm api key.
75
```

```
76
| Property     | Details  |
77
|
 
------------
 
|
 
--------
 
|

78

| **Type**     | \`string\` |
79
| **Required** | \`true\`   |
```

```
80

81

82
<br>
```

```
86

87
Specify the requested module name.
88
```

```
89
| Property     | Details  |
90
|
 
------------
 
|
 
--------
 
|

91

| **Type**     | \`string\` |
92
| **Required** | \`true\`   |
```

```
93

94

95
<br>
```

```
98

99
In the HuggingFace example in [UI-TARS/README_deploy.md](https://github.com/bytedance/UI-TARS/blob/main/README_deploy.md#python-test-code), the VLM parameters are as follows:
100
```

```
101
\`\`\`yaml
102
Language: en
103
VLM Provider: OpenAI compatible for UI-TARS-1.5
104
VLM Base URL: https:xxx
105
VLM API KEY: hf_xxx
106
VLM Model Name: tgi
107
\`\`\`
```

```
108

109
<br>
110

111
In the VolcEngine(火山引擎) example in [Doubao-1.5-UI-TARS](https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-1-5-ui-tars), the VLM parameters are as follows:
112
```

```
113
\`\`\`yaml
114
Language: cn
115
VLM Provider: VolcEngine Ark for Doubao-1.5-UI-TARS
116
VLM Base URL: ttps://ark.cn-beijing.volces.com/api/v3
117
VLM API KEY: ARK_API_KEY
118
VLM Model Name: doubao-1.5-ui-tars-250328
119
\`\`\`
```

```
120

121
<br>
122
```

[return to bytedance/UI-TARS-desktop](https://deepwiki.com/bytedance/UI-TARS-desktop)

VLMを使うということは、利用できるマシンのスペックの条件は厳しいですか？GPU搭載したハイスペックマシンじゃないとダメ？

Fast

Searched across bytedance/UI-TARS-desktop

## Answer

UI-TARS Desktopを使用するためのマシンスペック要件についてお答えします。

## マシンスペック要件

UI-TARS Desktopは、 **ローカルマシン上でGPUを必要としません** 。これは、VLM（Vision Language Model）の処理がクラウド上で行われるためです。

UI-TARS Desktopアプリケーション自体はElectronベースのデスクトップアプリケーションであり、一般的なデスクトップコンピュータやラップトップで動作するように設計されています。アプリケーションは以下の2つの主要な展開方法をサポートしています：

1. **クラウド展開** ：
	- この方法では、VLMモデルはHugging FaceやVolcEngine（火山引擎）などのクラウドサービス上で実行されます
	- ローカルマシンはAPIリクエストを送信し、結果を受け取るだけです bug\_report\_ui\_tars\_desktop.yml:27-32
2. **ローカル展開** ：
	- この方法も選択肢としてありますが、実際にはローカルでVLMを実行するわけではなく、ローカルネットワーク内のサーバーやAPIエンドポイントを指すことを意味します bug\_report\_ui\_tars\_desktop.yml:27-32

## 設定方法

UI-TARS Desktopでは、VLMプロバイダーの設定を通じて、クラウド上のモデルに接続します：

```
VLM Provider: OpenAI compatible for UI-TARS-1.5  
VLM Base URL: https:xxx  
VLM API KEY: hf_xxx  
VLM Model Name: tgi
```

setting.md:101-107

または、VolcEngine（火山引擎）を使用する場合：

```
VLM Provider: VolcEngine Ark for Doubao-1.5-UI-TARS  
VLM Base URL: ttps://ark.cn-beijing.volces.com/api/v3  
VLM API KEY: ARK_API_KEY  
VLM Model Name: doubao-1.5-ui-tars-250328
```

setting.md:113-119

これらの設定は、クラウド上のVLMサービスへの接続情報を指定するものであり、ローカルマシンでモデルを実行するための設定ではありません。

## アプリケーションの動作

UI-TARS Desktopアプリケーションは以下のように動作します：

1. スクリーンショットを撮影
2. そのスクリーンショットをクラウド上のVLMに送信
3. VLMからの応答を解析してアクションに変換
4. そのアクションをローカルマシン上で実行

この処理フローでは、計算負荷の高いVLMの処理はすべてクラウド上で行われるため、ローカルマシンには特別な高性能ハードウェア（GPUなど）は必要ありません。

## 必要なシステム権限

UI-TARS Desktopを実行するために必要なのは、以下のようなシステム権限です：

### macOS

- **スクリーンレコーディング権限** ：スクリーンショットを撮影するために必要
- **アクセシビリティ権限** ：マウスとキーボード入力をシミュレートするために必要 quick-start.md:27-30

### Windows

特別な権限設定は明示されていませんが、アプリケーションを実行するための標準的な権限が必要です。 quick-start.md:36-39

## まとめ

UI-TARS Desktopは、GPUを搭載したハイスペックマシンを必要としません。アプリケーション自体は標準的なデスクトップコンピュータやラップトップで動作し、VLMの処理負荷はクラウドサービス（Hugging FaceやVolcEngine）に委託されます。

ローカルマシンに必要なのは、スクリーンショットの撮影、APIリクエストの送信、受信したアクションの実行ができる程度の一般的なスペックです。特別なハードウェア要件はドキュメントに記載されていません。

## Notes

UI-TARS Desktopは、VLM（Vision Language Model）を使用していますが、そのモデルはクラウド上で実行されるため、ローカルマシンにGPUは必要ありません。アプリケーションはElectronベースで、標準的なデスクトップコンピュータやラップトップで動作します。設定画面でクラウドサービス（HuggingFaceやVolcEngine）への接続情報を指定することで、VLMの機能を利用できます。

Wiki pages you might want to explore:

- [UI-TARS Desktop (bytedance/UI-TARS-desktop)](https://deepwiki.com/bytedance/UI-TARS-desktop/4-ui-tars-desktop)
- [Contributing Guidelines (bytedance/UI-TARS-desktop)](https://deepwiki.com/bytedance/UI-TARS-desktop/9.2-contributing-guidelines)

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop)[.github/ISSUE\_TEMPLATE/bug\_report\_ui\_tars\_desktop.yml](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/.github/ISSUE_TEMPLATE/bug_report_ui_tars_desktop.yml)

```
24
  validations:
25
    required: true
26
- type: dropdown
```

```
27
  attributes:
28
    label: Deployment Method
29
    description: "Select the deployment method for UI TARS Desktop."
30
    options:
31
      - Cloud
32
      - Local
```

```
33
  validations:
34
    required: true
35
- type: textarea
```

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [docs/setting.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/docs/setting.md)

```
98

99
In the HuggingFace example in [UI-TARS/README_deploy.md](https://github.com/bytedance/UI-TARS/blob/main/README_deploy.md#python-test-code), the VLM parameters are as follows:
100
```

```
101
\`\`\`yaml
102
Language: en
103
VLM Provider: OpenAI compatible for UI-TARS-1.5
104
VLM Base URL: https:xxx
105
VLM API KEY: hf_xxx
106
VLM Model Name: tgi
107
\`\`\`
```

```
108

109
<br>
110

111
In the VolcEngine(火山引擎) example in [Doubao-1.5-UI-TARS](https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-1-5-ui-tars), the VLM parameters are as follows:
112
```

```
113
\`\`\`yaml
114
Language: cn
115
VLM Provider: VolcEngine Ark for Doubao-1.5-UI-TARS
116
VLM Base URL: ttps://ark.cn-beijing.volces.com/api/v3
117
VLM API KEY: ARK_API_KEY
118
VLM Model Name: doubao-1.5-ui-tars-250328
119
\`\`\`
```

```
120

121
<br>
122
```

[return to bytedance/UI-TARS-desktop](https://deepwiki.com/bytedance/UI-TARS-desktop)

クラウド上のモデルを利用するということですが、利用した際の情報はバイトダンス側に学習データとして利用されますか？セキュリティ面について詳しく教えてください

Fast

Searched across bytedance/UI-TARS-desktop

## Answer

UI-TARS Desktopのセキュリティとデータプライバシーについてお答えします。

## クラウドモデルの利用とデータプライバシー

UI-TARS Desktopでは、クラウド上のVLM（Vision Language Model）を利用していますが、コードベースを確認した限りでは、バイトダンス側がユーザーデータを学習データとして利用するかどうかについての明示的な記述は見つかりませんでした。

ただし、アプリケーションの設計から以下のことが分かります：

1. **データの送信先** ：  
	UI-TARS Desktopは、設定に応じて異なるVLMプロバイダー（Hugging FaceやVolcEngine/火山引擎など）にデータを送信します。これらのプロバイダーはそれぞれ独自のプライバシーポリシーを持っています。
2. **送信されるデータ** ：  
	アプリケーションはスクリーンショットを撮影し、それをクラウド上のVLMに送信します。これには画面上の情報が含まれます。

## UTIOデータ収集メカニズム

UI-TARS Desktopには「UTIO」（UI-TARS Insights and Observation）と呼ばれるデータ収集メカニズムが存在します。これは以下のようなイベントを収集する可能性があります： setting.md:216-222

UTIOは以下の3種類のイベントを収集します：

1. **アプリケーション起動情報** ：
	- プラットフォームタイプ
	- OSバージョン
	- 画面解像度
2. **送信された指示内容** ：
	- ユーザーが送信した指示内容
3. **共有レポート** ：
	- 最後のスクリーンショット（オプション）
	- レポートURL（オプション） setting.md:238-269

## セキュリティ面での考慮事項

1. **APIキーの管理** ：  
	VLMプロバイダーに接続するためのAPIキーはローカルに保存されます。これらのキーの安全な管理はユーザー自身の責任となります。
	```
	VLM Provider: OpenAI compatible for UI-TARS-1.5  
	VLM Base URL: https:xxx  
	VLM API KEY: hf_xxx  
	VLM Model Name: tgi
	```

setting.md:101-107

1. **スクリーンショットのプライバシー** ：  
	アプリケーションはスクリーンショットを撮影してクラウドに送信するため、画面上に機密情報がある場合は注意が必要です。
2. **プロバイダーの選択** ：  
	異なるVLMプロバイダーを選択できるため、プライバシーポリシーが自分のニーズに合ったプロバイダーを選ぶことができます。
	```
	VLM Provider: VolcEngine Ark for Doubao-1.5-UI-TARS  
	VLM Base URL: ttps://ark.cn-beijing.volces.com/api/v3  
	VLM API KEY: ARK_API_KEY  
	VLM Model Name: doubao-1.5-ui-tars-250328
	```

setting.md:113-119

## プライバシーに関する推奨事項

1. **機密情報の取り扱い** ：  
	スクリーンショットに機密情報が含まれる可能性がある場合は、UI-TARS Desktopの使用を避けるか、その情報が表示されていない状態で使用することをお勧めします。
2. **プロバイダーのプライバシーポリシーの確認** ：  
	選択したVLMプロバイダー（Hugging FaceやVolcEngine/火山引擎など）のプライバシーポリシーを確認し、データの取り扱いについて理解しておくことが重要です。
3. **UTIOの設定確認** ：  
	UTIOデータ収集メカニズムの設定を確認し、必要に応じて無効化または制限することを検討してください。

## まとめ

UI-TARS Desktopはクラウド上のVLMを利用するため、スクリーンショットや指示内容などのデータがクラウドに送信されます。バイトダンス側がこれらのデータを学習データとして利用するかどうかについての明示的な情報はコードベースには見つかりませんでしたが、UTIOデータ収集メカニズムが存在し、一部のデータが収集される可能性があります。

セキュリティとプライバシーを重視する場合は、使用するVLMプロバイダーのプライバシーポリシーを確認し、機密情報の取り扱いに注意することをお勧めします。

## Notes

UI-TARS Desktopのセキュリティとプライバシーに関する情報は限られています。コードベースからは、UTIOというデータ収集メカニズムの存在と、クラウドVLMプロバイダーへのデータ送信の仕組みは確認できましたが、バイトダンス側でのデータ利用ポリシーについての明確な記述は見つかりませんでした。実際の利用にあたっては、選択するVLMプロバイダーのプライバシーポリシーを確認することが重要です。

Wiki pages you might want to explore:

- [Overview (bytedance/UI-TARS-desktop)](https://deepwiki.com/bytedance/UI-TARS-desktop/1-overview)

[bytedance/UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop) [docs/setting.md](https://github.com/bytedance/UI-TARS-desktop/blob/16cc5eaa/docs/setting.md)

```
98

99
In the HuggingFace example in [UI-TARS/README_deploy.md](https://github.com/bytedance/UI-TARS/blob/main/README_deploy.md#python-test-code), the VLM parameters are as follows:
100
```

```
101
\`\`\`yaml
102
Language: en
103
VLM Provider: OpenAI compatible for UI-TARS-1.5
104
VLM Base URL: https:xxx
105
VLM API KEY: hf_xxx
106
VLM Model Name: tgi
107
\`\`\`
```

```
108

109
<br>
110

111
In the VolcEngine(火山引擎) example in [Doubao-1.5-UI-TARS](https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-1-5-ui-tars), the VLM parameters are as follows:
112
```

```
113
\`\`\`yaml
114
Language: cn
115
VLM Provider: VolcEngine Ark for Doubao-1.5-UI-TARS
116
VLM Base URL: ttps://ark.cn-beijing.volces.com/api/v3
117
VLM API KEY: ARK_API_KEY
118
VLM Model Name: doubao-1.5-ui-tars-250328
119
\`\`\`
```

```
120

121
<br>
122
```

```
213

214
#### UTIO Base URL
215
```

```
223

224
This option defines the base URL for the **UTIO** server that handles application events and instructions.
225
```

```
235

236
##### Event Types
237
```

```
238
The server handles three types of events:
239

240
###### **Application Launch**
241
\`\`\`typescript
242
interface AppLaunchedEvent {
243
  type: 'appLaunched';
244
  /** Platform type */
245
  platform: string;
246
  /** OS version, e.g. "major.minor.patch" format */
247
  osVersion: string;
248
  /** Screen width in pixels */
249
  screenWidth: number;
250
  /** Screen height in pixels */
251
  screenHeight: number;
252
}
253
\`\`\`
254

255
###### **Send Instruction**
256
\`\`\`typescript
257
interface SendInstructionEvent {
258
  type: 'sendInstruction';
259
  /** User-submitted instruction content */
260
  instruction: string;
261
}
262
\`\`\`
263

264
###### **Share Report**
265
\`\`\`typescript
266
interface ShareReportEvent {
267
  type: 'shareReport';
268
  /** Optional last screenshot url or base64 content */
269
  lastScreenshot?: string;
```

```
270
  /** Optional report url */
271
  report?: string;
272
  /** Related instruction */
```