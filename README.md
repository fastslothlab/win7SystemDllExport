system dll name to export function name database in windows 7
=============
This repo have four json files. seen `data type` to get how to decode those json files.
* i386 mean intel 32 bit cpu.
* amd64 mean intel 64 bit cpu.

data type
=============
i386_DllNameToExportNameListMap.json
amd64_DllNameToExportNameListMap.json
```
type DllNameToExportNameListMap struct{
	IsAmd64 bool `json:",omitempty"`
	IsI386 bool `json:",omitempty"`
	DllNameToExportNameListMap map[string][]string `json:",omitempty"`
}
```

i386_ExportNameToDllNameMap.json
amd64_ExportNameToDllNameMap.json
```
type ExportNameToDllNameMap struct{
	IsAmd64                bool                `json:",omitempty"`
	IsI386                 bool                `json:",omitempty"`
	ExportNameToDllNameMap map[string][]string `json:",omitempty"`
}
```
