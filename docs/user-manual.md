---
sidebar_position: 2
title: XroidVerse 操作マニュアル
description: XroidVerse ソフトウェアの使用方法ガイド
keywords: [XroidVerse, 操作マニュアル, 録画, シナリオ再生, Firebase]
---

# XroidVerse 操作マニュアル

## 📖 概要
**XroidVerse**は、Unreal Engine 5で開発されたAI録画システムです。Xroid Studioで作成したシナリオを再生し、その様子を録画することができます。

:::tip このマニュアルについて
このマニュアルは、XroidVerseソフトウェアの使用方法を説明するユーザー向けガイドです。
:::

## 🚀 使用方法

### 1. 📝 Xroid Studio でシナリオを準備する
まず、Xroid Studioでシナリオを作成・準備してください。

### 2. ▶️ XroidVerse を起動する
XroidVerseアプリケーションを起動します。

### 3. 🎬 録画方法の選択
録画方法は以下の2つから選択できます：

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="external" label="外部録画（OBS）" default>
    #### 外部録画（OBS使用）の場合
    - OBSを起動し、XroidVerseの画面を録画できるように設定してください
    - OBSでの録画設定を完了させてください
  </TabItem>
  <TabItem value="internal" label="内部録画機能">
    #### 内部録画機能を使用する場合
    - XroidVerseの「録画する（マイク入力は録音されません）」にチェックを入れます
    - 「保存先」フィールドで録画ファイルの保存場所を設定します
    
    **例**: `D:/Users/Udon-Tobira/Downloads/`
  </TabItem>
</Tabs>

### 4. 🔐 Firebase認証情報の入力
- 「メールアドレス」フィールドにFirebaseのメールアドレスを入力します
- 「パスワード」フィールドにFirebaseのパスワードを入力します

### 5. 🔴 録画開始（OBS使用の場合）
OBSを使用している場合は、OBSの録画開始ボタンを押してください。

### 6. ▶️ シナリオ再生の開始
1. XroidVerseの「ログイン」ボタンを押します
2. ログイン後、シナリオ内の画像・音声・動画のダウンロードが始まります

:::warning 重要
**ダウンロードの間はアプリケーションがフリーズ状態となり、画面は何も変化せず、操作もできません**
:::

3. ダウンロード完了後、シナリオ再生が自動的に始まります
4. 内部録画機能をONにしている場合は、録画も同時に自動でスタートします

### 7. 🎮 シナリオの進行
基本的には眺めるだけで進行します。

AIから返答を求められた場合は以下の操作を行ってください：

<Tabs>
  <TabItem value="text-input" label="テキスト入力" default>
    #### テキスト入力の場合
    - 画面にテキストボックスが表示されます
    - 音声で入力するか、キーボードから入力してください
  </TabItem>
  <TabItem value="choice" label="選択肢">
    #### 選択肢の場合
    - 選択肢のボタンが表示されます
    - 適切なボタンを押してください
  </TabItem>
</Tabs>

### 8. ⏹️ シナリオの終了
- シナリオが全て終了しても自動では終了しません
- **「Esc」キーまたは「Enter」キーを押して手動で終了**させてください
- 内部録画機能をONにしている場合は、この操作によって`video.mp4`という名前で動画ファイルが書き出されます

## 📁 録画ファイルについて

### 内部録画機能使用時
録画終了後、指定した保存先フォルダに以下のファイルが生成されます：

| ファイル名 | 内容 |
|-----------|------|
| `video.mp4` | 録画された映像・音声データ |

### 外部録画（OBS）使用時
OBSの設定に従って録画ファイルが保存されます。

## ⚠️ 注意事項

:::caution 重要な注意点
- **シナリオのダウンロード中はアプリケーションが応答しなくなりますが、これは正常な動作です**
- **内部録画機能では「マイク入力は録音されません」のでご注意ください**
- **シナリオ終了時は必ず手動で終了操作を行ってください**
:::

## 🔧 トラブルシューティング

### よくある問題と解決方法

| 問題 | 原因 | 解決方法 |
|------|------|----------|
| アプリケーションがフリーズしたように見える | シナリオのダウンロード中 | しばらくお待ちください（正常な動作です） |
| 録画ファイルが生成されない | 保存先のパス設定が不正 | 保存先のパスが正しく設定されているか確認してください |
| Firebase認証に失敗する | 認証情報が不正 | メールアドレスとパスワードが正しいか確認してください |

---

:::info サポート
その他の問題については、開発チームまでお問い合わせください。
::: 