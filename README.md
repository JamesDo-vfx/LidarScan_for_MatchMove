
# 🛸 JamesDo's Scan Aligner — LiDAR Prep Tool

*Công cụ tối ưu hóa và căn chỉnh dữ liệu LiDAR Scan dành cho quy trình Matchmove chuyên nghiệp.*

> "Cách nhanh nhất để đưa dữ liệu quét thực tế vào không gian 3D chuẩn xác — Căn chỉnh, Reset Transform và sẵn sàng cho Tracking chỉ trong vài cú click."

**Tác giả:** JamesDo | **Lĩnh vực:** VFX & Matchmove | 🌷✨

---

*Giao diện đơn giản, trực quan giúp bạn xử lý hàng loạt file scan một cách nhanh chóng.*

---

## 🤔 Đây là công cụ gì?

**JamesDo's Scan Aligner** là một addon dành cho Blender, giúp các nghệ sĩ Matchmove xử lý thô các bản quét LiDAR (thường từ iPhone hoặc máy quét chuyên dụng). Thay vì phải di chuyển và đặt lại trục tọa độ thủ công một cách mệt mỏi, công cụ này tự động hóa quy trình để đảm bảo mô hình của bạn luôn nằm ở **Gốc tọa độ (World Origin)** với tỉ lệ chuẩn xác trước khi đưa vào các phần mềm như 3DEqualizer, PFTrack hay Syntheyes. 💛

---

## ✨ Tính năng nổi bật

| Tính năng | Chi tiết |
| --- | --- |
| 📂 **Batch Import** | Nhập nhiều file `.fbx` cùng lúc với cấu trúc tên Shot/Sequence. |
| 📍 **Smart Registration** | Công cụ đưa tâm vật thể (Origin) về 3D Cursor cực nhanh. |
| 📐 **Apply Transforms** | Tự động đưa Location/Rotation về 0 và Scale về 1 để tránh lỗi tracking. |
| 📏 **Matchmove Scale** | Tùy chọn xuất file với tỉ lệ x100 đặc thù cho các phần mềm Matchmove. |
| 🚀 **Export Ready** | Xuất mesh sạch, đã căn chỉnh trục tọa độ đúng chuẩn công nghiệp. |

---

## 🚀 Hướng dẫn cài đặt

1. Tải file `.zip` của addon từ mục [Releases](https://github.com/).
2. Mở Blender, đi tới **Edit > Preferences > Add-ons**.
3. Nhấn **Install...** và chọn file `.zip` vừa tải.
4. Tích chọn **JamesDo's Scan Aligner** để kích hoạt. 🌷✨

---

## 🕹️ Quy trình sử dụng (Workflow)

Công cụ được thiết kế để sử dụng từ trên xuống dưới theo 3 bước:

### Bước 1: Import Raw Lidar Scan

* Nhấn **Batch Import Scan** để chọn các file scan thô.
* Addon sẽ tự động tổ chức chúng vào Scene cho bạn.

### Bước 2: Scene Registration (Quan trọng nhất)

Để phần mềm Matchmove hiểu được không gian, bạn cần làm sạch dữ liệu:

1. Find a matching feature on both scans.
2. **Set Origin to Cursor** at that point for the source object.
3. Place the **3D Cursor** on the same point of the target object.
4. Use **Selection to Cursor** to snap them together perfectly. ✨

### Bước 3: Export Aligned Model

1. Tích vào ô **Scale 100 (For MatchMove Software)** nếu bạn định đưa vào 3DEqualizer hoặc PFTrack.
2. Nhấn **Export Mesh**.

---

## 🛠️ Xử lý sự cố thường gặp

| Vấn đề | Nguyên nhân | Giải pháp |
| --- | --- | --- |
| Mô hình bị quá nhỏ khi vào 3DE | Quên tích chọn Scale 100 | Xuất lại và nhớ tích vào ô Scale 100. |
| File scan quá nặng, Blender bị treo | Số lượng đa giác (Polygon) quá lớn | Sử dụng modifier Decimate để giảm lưới trước khi Export. |
| Trục tọa độ bị ngược | Quy chuẩn trục khác nhau | Đảm bảo mặt đất nằm trên trục XY trước khi Apply Transforms. |

---

## 📄 Bản quyền (License)

Phát hành dưới giấy phép MIT — Xem file [LICENSE](https://www.google.com/search?q=LICENSE) để biết thêm chi tiết.

---

**Được tạo ra với ❤️ bởi JamesDo**

⭐ Hãy tặng mình 1 sao trên GitHub nếu bạn thấy công cụ này hữu ích nhé! 🌷✨

---

Hy vọng cấu trúc này đúng ý bạn! Nếu bạn cần mình thay đổi màu sắc của các nút badge hay thêm bớt mục nào, cứ bảo mình nha. 💛 Trông nó sẽ rất xịn sò trên GitHub đấy!
