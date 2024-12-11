# saveSEG 插件
此插件將複寫原本產生 SEG XML 檔案的功能

## 功能
- 儲存的是 dicom 檔案而非 XML

## 使用方法
- 更改 `bluelight/data/plugin.config`
- 加入 dcmjs 的檔案
- 加入此 repo 的 segSaver.js
```json
{
    "plugin": [
        {"path": "https://unpkg.com/dcmjs", "name": "dcmjs"},
        {"path": "../scripts/plugin/segSaver.js", "name": "segSaver"}
    ]
}
```