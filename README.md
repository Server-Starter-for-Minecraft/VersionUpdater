# VersionUpdater
package.jsonのversionを次のバージョンに更新する。

### inputs

##### update-type:
'major' | 'minor' | 'patch'
次のバージョンの種類
現在が1.2.3の場合、次のバージョンは以下のようになる。
- patch : 1.2.4
- minor : 1.3.0
- major : 2.0.0

##### json-path
string
プロジェクトルートからpackage.jsonまでのパス。
規定値 'package.json'

##### update-json
boolean
json内のバージョンを更新するかどうか (コミットはしない)
規定値 true

### outputs

##### current-version
string
現在のバージョン

##### next-version
string
次のバージョン
