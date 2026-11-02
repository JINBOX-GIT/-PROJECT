# 天姫_MIXXIA_多方向基準画制作仕様書_Ver0.1

## 1. 制作概要

天姫上半身8方向・試験制作Ver0.1。既存正面1枚＋新規7方向。生成とQA合格と正式採用は別段階。

## 2. 制作目的

Reels・動画・漫画の人物参照候補を作成する。完全な3D再構成や正確な角度の保証ではない。

## 3. 参照資料と優先順位

指定7資料は提供ファイルの本文・関連箇所を参照可能。全文の整合性監査やGitHub最新版の照合は行っていない。画像内に埋め込まれた他姫の人物画像は開かず、人物入力には添付の天姫1枚だけを使用した。他姫の外見プロンプトを生成へ流用していない。

|依頼資料|提供ファイル|確認範囲|
|---|---|---|
|00_運用規約_Ver1.9|11-00_-_Ver1.9-1-.docx|0.1、0.4、0.10、正本・差分・優先順位|
|正式設定Ⅰ章_Ver2.8|13-01_-_-_-_Ver2.8_-Word-1-.docx|天姫の関連記述、7.7.2等|
|世界設定_Ver1.83|12-02_-_-_Ver1.83.docx|天姫の役割に関する関連箇所|
|創世カノン_Ver1.2|10-04_-_-_Ver1.2.docx|天姫関連・作品思想の箇所。本文表題は「創生カノン」で表記差あり|
|作風定義と執筆憲章_Ver1.8|09-_Ver.1.8.docx|作風・人物描写の関連箇所|
|MIXXIA仕様_Ver0.5|16-_MIXXIA_-_Ver0.5.docx|Identity/Geometry、Pencil/COPIC/Lighting、正面、多方向、海姫の方法記述のみ|
|絵画的リアリズム_ver2.2|14-MarkDown-_ver2.2.md|Geometry非補正、Rendering、85mm F1.4、Loop Lighting|

運用規約は最上位。チャット確定正本→正本保存媒体→参考資料の扱いを継承する。本成果は新規試験候補で、既存正本を更新しない。運用規約内の02/03の文書体系名と提供資料の「02 世界設定」には表記体系差があるため、独断で改称・統合しない。

共通規則：元人物の癖も補正しない／Identity・GeometryとRenderingを分離／正面をGeometry Referenceとする／頭部と胴体を同じY軸角度で回す／視線だけカメラへ戻さない／装飾の遮蔽を許し再デザインしない／角度間で比較する。Pencilは構造線、COPICは彩色、Lightingは光と質感の層である。今回は完成済みの添付から多方向へ進む応用条件であり、Pencil・COPICを新規実行していない。背面180°は今回の追加条件。海姫10.5.6と重複番号10.5.7の記述は制作依頼例として参照し、他姫の造形を用いていない。

## 4. 天姫正面基準画の定義

唯一の人物入力は今回の添付PNG。1024×1536。TEN_00_Front.pngは原本のバイト列をコピーし、補正・トリミング・再保存なし。原本には頭の傾きと肩線の傾斜があるため、その姿勢を基準とした。「0°」は登録名であり厳密な正投影を実測した意味ではない。

## 5. Identity Lock仕様

添付の顔・年齢印象・微笑み・肌・ショートボブ・花羽根飾り・衣装のみを固定基準とする。生成された候補を正面に代わるIdentity Sourceにしない。

## 6. Facial Geometry仕様

輪郭、頬、顎、額、目眉鼻口の相対配置を保持する指示。横顔の鼻・顎・額の奥行きは正面のみから確定不能。数値的な同一性測定は実施していない。

## 7. Hair Geometry仕様

ブラウンの短いボブ、透ける前髪、左右非対称の羽根花飾りと花・クリスタルの下がりを継承。全方向で微細な花弁数や金具形状に揺れがある。

## 8. Costume Geometry仕様

淡いピンク・アイボリー、花刺繍・レース・シアー袖、首元の小ハートと胸元の大ハートを固定。側面は遮蔽を許す。背面の開口・留め具・腰のレースは未承認推定。

## 9. Body Geometry仕様

首長・肩幅・胸郭・腕の比率を変更しない指示。元の腕を前へ下ろす姿勢を継承する。側面の厚みは正面から検証不能。

## 10. Rotation Geometry仕様

人物自身の右＝鼻が画面左、人物自身の左＝鼻が画面右。頭部・胴体・肩・腕を剛体的に回転する。左右反転処理は未使用。指定角度はプロンプト条件で、実測値ではない。45°は不適合が残る。

## 11. Rendering仕様

絵画的リアリズムLighting Rendering、85mm F1.4、Loop Lighting、白背景、原本と同じ淡色・素材感。これは生成指示であり実在レンズや撮影EXIFの証明ではない。目視では近い質感だが厳密な照明一致は未検証。

## 12. Composition仕様

全PNG1024×1536、2:3縦長。正面の画角を優先し、腰下を入れるための再トリミングや身体引き伸ばしは行わない。全方向で頭部サイズ・人物位置は近似で、完全一致ではない。新しく見える側面・後頭部・背中は推定生成。

## 13. 8方向基準画一覧

### 00_Front

![[images/TEN_00_Front.png]]

### R15

![[images/TEN_R15.png]]

### L15

![[images/TEN_L15.png]]

### R45

![[images/TEN_R45.png]]

### L45

![[images/TEN_L45.png]]

### R90

![[images/TEN_R90.png]]

### L90

![[images/TEN_L90.png]]

### 180_Back

![[images/TEN_180_Back.png]]

## 14. 画像生成プロンプト

以下は実際に送信した指示（原文）。全呼出しの人物入力はTEN_00_Frontと同一の添付原本1枚のみ。内蔵image_genを使用し、内部モデルの正式識別名は取得不可。Seed/CFG/Stepsは取得不可。

### TEN_R15

- 生成日時UTC：2026-11-01T10:54:20.210Z
- サイズ：(1024, 1536)
- 再生成回数：0
- 結果：PNG生成成功／未承認
- 品質：要確認
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction R15: rotate her own right, nose points slightly toward SCREEN LEFT exactly 15 degrees from supplied front. Slight three-dimensional yaw, NOT 45 degrees. Both eyes visible with subtle foreshortening.
```

### TEN_L15

- 生成日時UTC：2026-11-01T10:54:49.725Z
- サイズ：(1024, 1536)
- 再生成回数：0
- 結果：PNG生成成功／未承認
- 品質：要確認
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction L15: rotate her own left, nose points slightly toward SCREEN RIGHT exactly 15 degrees from supplied front. Slight three-dimensional yaw, NOT 45 degrees. Both eyes visible with subtle foreshortening.
```

### TEN_R45

- 生成日時UTC：2026-11-01T11:00:00.029Z
- サイズ：(1024, 1536)
- 再生成回数：2
- 結果：PNG生成成功／未承認
- 品質：NG
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. CRITICAL DIRECTION: NOSE MUST POINT TOWARD THE LEFT EDGE OF THE IMAGE, viewer's LEFT. Show the woman's LEFT cheek and LEFT ear near camera. This is her own RIGHT turn of 45 degrees, TEN_R45. Turn BOTH shoulders and entire torso 45 degrees toward viewer's LEFT; front heart gems point diagonal LEFT. True three-quarter view, far eye smaller, far shoulder behind near shoulder. DO NOT FACE SCREEN RIGHT. Same original person and costume.
```

### TEN_L45

- 生成日時UTC：2026-11-01T10:58:30.684Z
- サイズ：(1024, 1536)
- 再生成回数：1
- 結果：PNG生成成功／未承認
- 品質：NG
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction L45, corrective generation: Whole person rotated a clear 45 degrees own left toward SCREEN RIGHT. Critical: camera sees BOTH her front and side equally, shoulders and ribcage at 45 degrees, front heart gem visibly foreshortened, far breast and far shoulder partially hidden behind near side. Face yaw 45, distant eye noticeably narrowed by perspective, nose overlaps distant cheek. NOT a nearly frontal portrait. Do not increase rotation of head relative to torso; rotate whole body together. Preserve original tilt, proportions and front costume.
```

### TEN_R90

- 生成日時UTC：2026-11-01T10:58:10.784Z
- サイズ：(1024, 1536)
- 再生成回数：0
- 結果：PNG生成成功／未承認
- 品質：要確認
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction R90: STRICT TRUE SIDE PROFILE, 90 degrees her own right, nose pointing horizontally to SCREEN LEFT, see her left side. Entire ribcage, shoulder line and arms are viewed EDGE-ON IN SIDE ELEVATION, not frontal torso. Only ONE eye visible; far eye fully occluded. Far shoulder behind near shoulder. No three-quarter face. Heart gems on front of neck/chest seen only edge-on, never moved onto side. Preserve original pose relative to body.
```

### TEN_L90

- 生成日時UTC：2026-11-01T10:57:38.069Z
- サイズ：(1024, 1536)
- 再生成回数：0
- 結果：PNG生成成功／未承認
- 品質：要確認
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction L90: STRICT TRUE SIDE PROFILE, 90 degrees her own left, nose pointing horizontally to SCREEN RIGHT, see her right side. Entire ribcage, shoulder line and arms are viewed EDGE-ON IN SIDE ELEVATION, not frontal torso. Only ONE eye visible; far eye fully occluded. Far shoulder behind near shoulder. No three-quarter face. Heart gems on front of neck/chest seen only edge-on, never moved onto side. Preserve original pose relative to body.
```

### TEN_180_Back

- 生成日時UTC：2026-11-01T11:00:24.568Z
- サイズ：(1024, 1536)
- 再生成回数：1
- 結果：PNG生成成功／未承認
- 品質：要確認
- ネガティブ指定：下記Avoid、No、Do not節に含む。

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction BACK 180 degrees: EXACT REAR ELEVATION, head and torso both fully facing away. No face or eye visible. Preserve brown short bob volume and nape length, hair ornaments attached to their original anatomical sides (now screen sides reverse due to rotation, NOT mirroring). Show only backs and side edges of existing ornaments, not new ornaments. Back of lace choker, shoulder straps and sheer embroidered pale pink ivory dress consistent with front. Front heart gems are hidden on chest, DO NOT duplicate heart gems on back. Unseen back design is a conservative provisional continuation of existing floral lace and shawl, no invented bow, zipper feature, wings or back gem. Preserve original shoulder/head tilt and arms in front of body, mostly occluded from rear. Plain white background. Corrective instruction: arms are IN FRONT OF HER ABDOMEN exactly as source pose. From rear camera, forearms and hands must be OCCLUDED BY TORSO; do NOT show forearms crossing over her lower back and do NOT clasp hands behind her back. Upper arms fall along sides, lower arms go away from camera in front. Keep shoulders and head tilt from source. Minimal rear lace continuation, back aperture shape is provisional.
```

## 15. 品質検査結果

|画像|Identity|Facial Geometry|Hair|Costume|Body|Rotation|Rendering|Composition|総合|
|---|---|---|---|---|---|---|---|---|---|
|TEN_00_Front|OK|OK|OK|OK|OK|要確認|要確認|OK|原本・無変更|
|TEN_R15|要確認|要確認|要確認|要確認|要確認|要確認|OK|要確認|要確認|
|TEN_L15|要確認|要確認|要確認|要確認|要確認|要確認|OK|要確認|要確認|
|TEN_R45|要確認|要確認|要確認|要確認|要確認|NG|OK|要確認|NG|
|TEN_L45|要確認|要確認|要確認|要確認|要確認|NG|OK|要確認|NG|
|TEN_R90|要確認|要確認|要確認|要確認|要確認|要確認|OK|要確認|要確認|
|TEN_L90|要確認|要確認|要確認|要確認|要確認|要確認|OK|要確認|要確認|
|TEN_180_Back|要確認|要確認|要確認|要確認|要確認|要確認|OK|要確認|要確認|

**R15**：顔の方向は画面左。胴体の回転が顔より弱く見える。15°の厳密値、首元の下がり金具と花の配列は要確認。

**L15**：顔の方向は画面右。髪飾りの花・羽根・下がり飾りの配列、胸元刺繍が原本と完全一致しない。厳密角度は未測定。

**R45**：NG：方向の誤りは解消したが、胴体が正面寄りで顔との回転差が残る。45°剛体回転基準として不適合。

**L45**：NG：胴体は斜めだが顔がカメラ側へ戻る傾向があり、頭部と胴体の45°一致を満たさない。

**R90**：画面左向きの側面。鼻・顎・後頭部・胸郭の厚みは単一正面からの推定。厳密な90°と元ポーズの継承は要確認。

**L90**：画面右向きの側面。遠側眼付近の描写が残り、厳密90°か要確認。鼻・顎の突出と衣装側面は推定。

**180_Back**：前面ハートの背面複製なし。腕を背中へ回す誤りは改善。背中の大きな開口、腰の花レース、留め具、後頭部と装飾背面は未確認の推定であり正式設定ではない。

原本のRotationは正面登録に傾きがある点、Renderingは撮影条件の実証不能のため要確認。他の原本OKは原本との自己一致の意味。

## 16. 制作履歴・再生成履歴

順序：左右15°→左右45°初回→左右90°→45°修正→背面→右45°方向修正→背面腕修正。再生成4回、総生成11画像、最終比較用7画像。左右45°初回は浅い回転、右45°2回目は逆向き、背面初回は腕が背中側へ回ったため除外。NG履歴画像はhistory/に隔離し、最終候補と混同しない。

### R45_attempt1（除外）

日時UTC：2026-11-01T10:55:50.986Z

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction R45: rotate her own right, nose toward SCREEN LEFT exactly 45 degrees. Clear THREE QUARTER VIEW of whole torso AND head, shoulder on far side foreshortened. Not just face rotation. Nose and sternum face same yaw direction. Preserve attached original head tilt relative to torso.
```

### L45_attempt1（除外）

日時UTC：2026-11-01T10:56:17.731Z

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction L45: rotate her own left, nose toward SCREEN RIGHT exactly 45 degrees. Clear THREE QUARTER VIEW of whole torso AND head, shoulder on far side foreshortened. Not just face rotation. Nose and sternum face same yaw direction. Preserve attached original head tilt relative to torso.
```

### R45_attempt2（除外）

日時UTC：2026-11-01T10:57:52.344Z

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction R45, corrective generation: Whole person rotated a clear 45 degrees own right toward SCREEN LEFT. Critical: camera sees BOTH her front and side equally, shoulders and ribcage at 45 degrees, front heart gem visibly foreshortened, far breast and far shoulder partially hidden behind near side. Face yaw 45, distant eye noticeably narrowed by perspective, nose overlaps distant cheek. NOT a nearly frontal portrait. Do not increase rotation of head relative to torso; rotate whole body together. Preserve original tilt, proportions and front costume.
```

### 180_Back_attempt1（除外）

日時UTC：2026-11-01T10:59:21.796Z

```text
Use case: identity-preserve. Create ONE portrait reference image of the exact same adult woman Tenhime in the sole attached reference. Only rotate the entire existing person rigidly about vertical Y axis; head, torso, shoulders, neck and arms rotate together. Preserve original head tilt relative to shoulders and original arms held down inward in front. Do not straighten her pose. Preserve exact face bone structure, gray-brown eyes, lips, age, warm brown short bob and wispy bangs, nonidentical bilateral pink ivory feather-flower hair ornaments and dangling crystals, flower earrings. Preserve pale pink ivory floral lace dress, sheer embroidered shawl/sleeves, floral straps, small heart gem at lace choker and larger lower-chest heart gem, gold filigree and crystal drops. No redesign, beautifying, slimming or bust changes. Attached image is the ONLY person and costume reference. Painterly realism Lighting Rendering matching attached delicate textures, 85mm F1.4, soft Loop Lighting, plain white background. Same vertical 2:3 canvas preferably 1024x1536, same head size and centered head-to-lower-waist framing as original, no stretching. Gaze rotates with head, do not look back at camera. No text, labels, collage, extra accessories, anime or plastic skin. Occlude details naturally. Direction BACK 180 degrees: EXACT REAR ELEVATION, head and torso both fully facing away. No face or eye visible. Preserve brown short bob volume and nape length, hair ornaments attached to their original anatomical sides (now screen sides reverse due to rotation, NOT mirroring). Show only backs and side edges of existing ornaments, not new ornaments. Back of lace choker, shoulder straps and sheer embroidered pale pink ivory dress consistent with front. Front heart gems are hidden on chest, DO NOT duplicate heart gems on back. Unseen back design is a conservative provisional continuation of existing floral lace and shawl, no invented bow, zipper feature, wings or back gem. Preserve original shoulder/head tilt and arms in front of body, mostly occluded from rear. Plain white background.
```

## 17. 未確定事項・承認管理

最終7方向の総合判定はNG2枚、要確認5枚、無条件OK0枚。正式採用0枚。45°は顔と胴体の回転を修正してから再審査する。背面の開口・後頭部・髪飾り裏・背面レース・留め具はユーザー承認必須。正面のみでは検証不能な厚みは、承認済み立体資料が得られるまで確定しない。今後は角度を制御できる3D代理形状で投影を固定し、原本のIdentityを照合する方法が改善候補。既存設定・GitHub資料は変更していない。
