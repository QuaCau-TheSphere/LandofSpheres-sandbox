Mô tả::
# Đầu vào
- [ ] Tìm hiểu những tài nguyên hỗ trợ: 
	- [ ] [Obsidian Hub](https://publish.obsidian.md/hub/00+-+Start+here "00 - Start here - Obsidian Hub - Obsidian Publish")
	- [ ] Các web publish
- [ ] Tham gia [Discord Tiếng Việt cho Obsidian](https://discord.gg/obsidianmd)
# Đầu ra
# Tài liệu

# Người chơi
```dataview
list
From "6 Tổ chức/62 Thành viên (Người chơi)" 
where contains(kỹ-năng, [[]])
```

# Thử thách
```dataview
table 
	trạng-thái as "Trạng thái", 
	filter(file.inlinks, (i) => i.hoạt-động) as "Mục tiêu",
	người-chơi as "Người chơi"
from "1 Công việc"
Where contains(kỹ-năng, [[]])
```
```dataview 
List
from "1 Công việc"
Where contains(kỹ-năng, [[]])
```
