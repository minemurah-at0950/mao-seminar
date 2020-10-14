# SENKYO_JAPAN_MAP
EMAPで使用している選挙用の日本地図を管理するためのリポジトリです。  
  
**EMAPの地図種別 と 最新バージョン**  
- ```Prefecture``` : 県境 - YYYY.MM.DD
- ```City``` : 市区町村の境界 - YYYY.MM.DD
- ```SHSenkyoku``` : 衆院選 選挙区 - 2020.10.2 ( 2020.10.1 演出チェック済 )
- ```SHKaihyojo``` : 衆院選 開票所 - 2020.10.2 ( 2020.10.1 演出チェック済 )
- ```SASenkyoku``` : 参院選 選挙区 - YYYY.MM.DD
- ```SAKaihyojo``` : 参院選 開票所 - YYYY.MM.DD

  
## フォルダ構造
```
.
├── DOC                 # ドキュメント。仕様書や配布資料、開発者向け資料など
├── FBX                 # 3DCGファイル。EMAPで使用しているFBXファイルと、書き出し用のMayaシーン
├── SCRIPTS             # 各種スクリプト。ArcGIS、 Mayaでのshape > FBX 変換
├── SHAPE               # Shapeファイル。ドキュメント・FBX・SVGの元となるデータ
├── SVG                 # SVGファイル。EMAPで地図の境界描画に使用
└── README.md
```

**EMAP用のUnityアセット**  
EMAPで読み込む最終ファイルは、以下の２種類です。
- ```FBX```のFBXファイル
- ```SVG```のSGVファイル


## 更新履歴

### 2020.10. 2 &nbsp;　地図・属性情報の修正 
**衆院選**  
&nbsp;　・兵庫12区「姫路市12区４」を「姫路市12区３」へ統合  
&nbsp;　・広島6区「尾道市瀬尾道」を「尾道市尾道」へ修正 ：誤植   
&nbsp;　・宮崎2区「五ケ瀬町」を「五ヶ瀬町」へ修正 ：「ヶ」のサイズを変更    
**全国地図・参院選**  
&nbsp;　・宮崎県　「五ケ瀬町」を「五ヶ瀬町」へ修正  

**更新対象ファイル**
```
.
├── DOC                 報道局配布資料, 属性情報(Excel)
├── FBX                 SHSenkyoku, SHKaihyojo
├── SCRIPTS             Output_Python_Script.jsx, import_to_maya.py
├── SHAPE               全てのファイル
├── SVG                 SHSenkyoku, SHKaihyojo
└── README.md
```
