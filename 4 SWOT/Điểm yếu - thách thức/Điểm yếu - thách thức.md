# Những vấn đề có nhiều hệ quả nhất
```dataview
LIST WITHOUT ID K + ": " + length(rows)
WHERE lý-do
WHERE trạng-thái != "Đã giải quyết xong"
FLATTEN lý-do
GROUP BY lý-do AS K
SORT length(rows) DESC
Limit 10
```

## Những vấn đề bề mặt
```dataview 
table lý-do from "4 SWOT/Điểm yếu - thách thức" 
Where length(file.outlinks)!=0 and file.name != this.file.name
```
## Những vấn đề nguồn 2
```dataview 
table lý-do from "4 SWOT/Điểm yếu - thách thức" 
Where meta(lý-do).path and file.name != this.file.name
```

## Những vấn đề nguồn
```dataview 
list from "4 SWOT/Điểm yếu - thách thức" 
Where length(file.outlinks)=0 and file.name != this.file.name
```

## Những vấn đề đã được thảo luận
```dataview 
list from "4 Tài liệu/41 SWOT/Điểm yếu" 
Where row["Nội dung"]
```
