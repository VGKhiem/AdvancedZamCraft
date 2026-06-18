# ✨ ADVANCED ZAMCRAFT - HỆ THỐNG RPG TOÀN DIỆN

AdvancedZamCraft là một plugin RPG nâng cao dành cho server Minecraft (**Paper 1.21.8 - 1.21.11**). Plugin này tích hợp toàn bộ các tính năng nhập vai từ hệ thống nhân vật, hệ phái, kỹ năng, cường hóa, khảm ngọc, cho đến tính năng độc đáo hệ thống **tự tạo vật phẩm** (AI).

---

## 🚀 Các Tính Năng Cốt Lõi

### 🎭 1. Hệ Thống Hệ Phái (Classes) & Thiên Phú (Talents)
Plugin hỗ trợ 4 lớp nhân vật cơ bản, mỗi phái có hệ số nhận chỉ số gốc khác nhau và bảng thiên phú riêng biệt:
- 🗡️ **SÁT THỦ (Assassin)**: Tốc độ cao, sát thương vật lý và chí mạng cực mạnh, nội tại tăng tỉ lệ hút máu và đòn đánh thứ 3 gây thêm sát thương.
- 🛡️ **HIỆP SĨ (Knight)**: Lượng máu và giáp vượt trội, khả năng phản sát thương, đỡ đòn tốt, nội tại tăng % máu tối đa.
- 🏹 **CUNG THỦ (Archer)**: Chiến đấu tầm xa với lượng sát thương cung lớn, tốc độ di chuyển nhanh, nội tại tăng tỉ lệ bắn ra chùm tên.
- 🔮 **PHÁP SƯ (Mage)**: Tầm đánh phép xa, lượng mana và hồi mana dồi dào, tăng sát thương phép thuật và sát thương kỹ năng, nội tại tăng % kháng sát thương.

<div style="border-left: 4px solid #2b9fe3; padding: 6px 12px; margin: 15px 0;">
  <span style="color: #2b9fe3; font-weight: bold; font-size: 1.1em;">ℹ️ THÔNG TIN THIÊN PHÚ:</span><br>
  Người chơi khi thăng cấp sẽ nhận được điểm thiên phú để tăng cấp các kỹ năng thiên phú (Talent 1 đến Talent 5) của phái mình chọn trong menu <strong>/nhanvat</strong> (hoặc <strong>/nv</strong>, <strong>/stats</strong>).
</div>

---

### ⚔️ 2. Hệ Thống Chỉ Số RPG Đa Dạng
AdvancedZamCraft sở hữu hơn 22 thuộc tính chỉ số RPG chia làm các nhóm chính:
- **Tấn công**:<br>
  &nbsp;&nbsp;&nbsp;&nbsp;Sát thương vật lý (<span style="color: #e74c3c;">PHYSICAL_DAMAGE</span>), Sát thương cung (<span style="color: #2ecc71;">BOW_DAMAGE</span>), Sát thương phép (<span style="color: #9b59b6;">MAGIC_DAMAGE</span>), Tỉ lệ chí mạng (<span style="color: #e67e22;">CRIT_CHANCE</span>), Sát thương chí mạng (<span style="color: #e67e22;">CRIT_DAMAGE</span>), Xuyên giáp (<span style="color: #e67e22;">PENETRATION</span>), Chính xác (<span style="color: #e67e22;">ACCURACY</span>), Sát thương kỹ năng (<span style="color: #e67e22;">SKILL_DAMAGE</span>).
- **Phòng thủ**:<br>
  &nbsp;&nbsp;&nbsp;&nbsp;Máu tối đa (<span style="color: #e74c3c;">HEALTH</span>), Giáp/Phòng thủ (<span style="color: #3498db;">DEFENSE</span>), Né tránh (<span style="color: #2ecc71;">DODGE_RATE</span>), Kháng chí mạng (<span style="color: #3498db;">CRIT_DEFENSE</span>), Tỉ lệ đỡ đòn (<span style="color: #3498db;">BLOCK_RATE</span>), Lượng sát thương chặn (<span style="color: #3498db;">BLOCK_AMOUNT</span>).
- **Tiện ích & Khác**:<br>
  &nbsp;&nbsp;&nbsp;&nbsp;Tốc độ chạy (<span style="color: #1abc9c;">SPEED</span>), Tăng PvP (<span style="color: #e74c3c;">PVP_DAMAGE</span>) / Giảm PvP (<span style="color: #3498db;">PVP_DEFENSE</span>), Tăng PvE (<span style="color: #e74c3c;">PVE_DAMAGE</span>) / Giảm PvE (<span style="color: #3498db;">PVE_DEFENSE</span>), Tăng EXP (<span style="color: #1abc9c;">EXP_BONUS</span>), Tăng Tiền (<span style="color: #1abc9c;">MONEY_BONUS</span>), Tốc độ hồi phục (<span style="color: #2ecc71;">REGENERATION</span>), Hiệu ứng ma pháp (<span style="color: #9b59b6;">MAGIC_EFFECT</span>).

---

### 🔮 3. Kỹ Năng Vũ Khí, Chiêu Cuối & Nội Tại
- **Kỹ năng chủ động <span style="color: #2980b9;">(Abilities)</span>**:<br>
  &nbsp;&nbsp;&nbsp;&nbsp;Sấm sét (<span style="color: #e74c3c;">SAM_SET</span>), Độc diện rộng (<span style="color: #e74c3c;">DOC_DIEN_RONG</span>), Tia Laser (<span style="color: #e74c3c;">TIA_LASER</span>), Hút máu (<span style="color: #e74c3c;">HUT_MAU</span>), Ăn mòn (<span style="color: #e74c3c;">AN_MON</span>), Lốc xoáy (<span style="color: #e74c3c;">LOC_XOAY</span>), Phát nổ (<span style="color: #e74c3c;">PHAT_NO</span>), Đóng băng (<span style="color: #e74c3c;">DONG_BANG</span>), Cực quang (<span style="color: #e74c3c;">CUC_QUANG</span>), và Đảo hướng (<span style="color: #e74c3c;">DAO_HUONG</span>).
- **Chiêu tối thượng <span style="color: #9b59b6;">(Ultimates)</span>**:<br>
  &nbsp;&nbsp;&nbsp;&nbsp;Lôi phạt (<span style="color: #9b59b6;">LOI_PHAT</span>), Công lý (<span style="color: #9b59b6;">CONG_LY</span>), Sóng thần (<span style="color: #9b59b6;">SONG_THAN</span>), Lãnh địa (<span style="color: #9b59b6;">LANH_DIA</span>), Băng hàn (<span style="color: #9b59b6;">BANG_HAN</span>), Dịch chuyển (<span style="color: #9b59b6;">DICH_CHUYEN</span>)...
- **Nội tại <span style="color: #27ae60;">(Passives)</span>**:<br>
  &nbsp;&nbsp;&nbsp;&nbsp;Thức tỉnh (<span style="color: #27ae60;">THUC_TINH</span>), Quỷ vương (<span style="color: #27ae60;">QUY_VUONG</span>), Kinh địa (<span style="color: #27ae60;">KINH_DIA</span>), Thiên quang (<span style="color: #27ae60;">THIEN_QUANG</span>), Đối ma (<span style="color: #27ae60;">DOI_MA</span>), và Cường hóa (<span style="color: #27ae60;">CUONG_HOA</span>).

---

### ⚒️ 4. Lò Rèn Cường Hóa & Bàn Chuyển Hóa
Hệ thống rèn trang bị nâng cao qua GUI trực quan:
- **Cường Hóa (<span style="color: #e2c027; font-weight: bold;">/zc upgradegui</span>)**: Đặt vũ khí/trang bị, đặt **Đá Cường Hóa** và **Bùa Bảo Vệ** (tùy chọn).
  - Thành công: Vật phẩm được tăng cấp (tối đa tùy cấu hình, mặc định +15).
  - Thất bại: Vật phẩm bị tụt đi 1 cấp cường hóa. Nếu có sử dụng **Bùa Bảo Vệ**, vật phẩm sẽ được giữ nguyên cấp độ khi thất bại.
- **Chuyển Hóa (<span style="color: #e2c027; font-weight: bold;">/zc transfergui</span>)**: Cho phép chuyển cấp độ cường hóa từ vũ khí cũ sang vũ khí mới.
  - Yêu cầu bắt buộc **Đá Chuyển Hóa**.
  - Nếu thất bại mà không có **Bùa Bảo Vệ**, vũ khí gốc sẽ bị tụt đi 1 cấp. Nếu có bùa bảo vệ, vũ khí gốc sẽ được an toàn.

---

### 💎 5. Hệ Thống Khảm Ngọc (Socket System)
Người chơi có thể cá nhân hóa trang bị bằng các viên ngọc tăng chỉ số:
- **Đục lỗ khảm**: Sử dụng lệnh <span style="color: #e2c027; font-weight: bold;">/zc addsocket</span> để thêm ô ngọc trống vào lore trang bị.
- **Khảm ngọc (<span style="color: #e2c027; font-weight: bold;">/zc gemgui</span>)**: Kéo thả **Ngọc thuộc tính** vào ô ngọc trống. Mỗi viên ngọc có tỉ lệ thành công nhất định. Nếu thất bại, viên ngọc sẽ bị vỡ.
- **Tháo ngọc**: Để lấy lại ngọc đã khảm, người chơi phải cầm **Thanh Xoá Ngọc** (`Gem Remover`) và kéo thả vào ô ngọc đã gắn trong menu khảm ngọc. *Chú ý: Thanh Xoá Ngọc sẽ bị tiêu hao 1 đơn vị sau mỗi lần tháo ngọc thành công.*

---

### 🤖 6. Sinh Tạo Vật Phẩm Bằng AI (Gemini)
Tính năng độc quyền cho phép Admin tạo ra các trang bị độc nhất vô nhị chỉ bằng mô tả văn bản tiếng Việt hoặc tiếng Anh:
- Sử dụng lệnh: <span style="color: #e2c027; font-weight: bold;">/zc ai</span> &lt;Mô tả vũ khí bạn muốn&gt;
- Ví dụ: <span style="color: #e2c027; font-weight: bold;">/zc ai</span> kiếm rồng đỏ có sát thương chí mạng cao và hiệu ứng thiêu đốt
- Gemini AI sẽ tự động phân tích prompt, tạo ra tên vật phẩm có dải màu gradient cực đẹp, tự động phân phối các chỉ số RPG hợp lý, thêm dòng mô tả (Lore) cốt truyện sâu sắc và gán các kỹ năng/hiệu ứng phù hợp nhất với mô tả của bạn.

---

## 📜 Danh Sách Lệnh (Commands)

### 🎮 Lệnh dành cho Người Chơi
- <span style="color: #2b9fe3; font-weight: bold;">/nhanvat</span> (hoặc <span style="color: #2b9fe3; font-weight: bold;">/nv</span>, <span style="color: #2b9fe3; font-weight: bold;">/stats</span>): Mở giao diện thông tin nhân vật, nâng điểm tiềm năng, học thiên phú.
- <span style="color: #2b9fe3; font-weight: bold;">/zc bal</span>: Xem số dư **Linh Hồn** hiện có.
- <span style="color: #2b9fe3; font-weight: bold;">/zc help</span>: Xem menu hướng dẫn các lệnh trong game.
- <span style="color: #2b9fe3; font-weight: bold;">/zc about</span>: Xem thông tin phiên bản plugin.

### 👑 Lệnh dành cho Quản Trị Viên (Yêu cầu quyền `zamcraft.admin`)
- <span style="color: #e2c027; font-weight: bold;">/zc upgradegui</span>: Mở Lò Rèn Cường Hóa.
- <span style="color: #e2c027; font-weight: bold;">/zc transfergui</span>: Mở Bàn Chuyển Hóa thuộc tính.
- <span style="color: #e2c027; font-weight: bold;">/zc gemgui</span>: Mở bàn gắn/tháo ngọc.
- <span style="color: #e2c027; font-weight: bold;">/zc addsocket</span> [Dòng]: Thêm một ô ngọc trống vào dòng lore chỉ định trên vật phẩm cầm tay.
- <span style="color: #e2c027; font-weight: bold;">/zc getitem</span> &lt;UpgradeStone&#124;ProtectCharm&#124;TransferStone&#124;Gem&#124;GemRemover&gt; [Cấp/ID]: Nhận các nguyên liệu rèn/khảm ngọc.
- <span style="color: #e2c027; font-weight: bold;">/zc generate</span> &lt;SWORD&#124;BOW&#124;WAND&#124;ARMOR&gt;: Tự sinh ngẫu nhiên một trang bị RPG theo phân lớp.
- <span style="color: #e2c027; font-weight: bold;">/zc setstats</span> &lt;Chỉ_số&gt; &lt;Giá_trị&gt; [Dòng]: Gán chỉ số RPG trực tiếp vào vật phẩm.
- <span style="color: #e2c027; font-weight: bold;">/zc setability</span> &lt;Kỹ_năng&gt; &lt;Cấp&gt; &lt;Tỉ_lệ&gt;: Gán kỹ năng vũ khí.
- <span style="color: #e2c027; font-weight: bold;">/zc setultimate</span> &lt;Tổ_hợp_phím&gt; &lt;Chiêu_cuối&gt; &lt;Cấp&gt; &lt;Hồi_chiêu&gt;: Gán chiêu cuối kích hoạt bằng nhấp chuột.
- <span style="color: #e2c027; font-weight: bold;">/zc setpassive</span> &lt;Nội_tại&gt; &lt;Cấp&gt;: Gán kỹ năng nội tại hệ phái.
- <span style="color: #e2c027; font-weight: bold;">/zc setreq</span> &lt;HỆ_PHÁI&gt;: Yêu cầu hệ phái để sử dụng trang bị này.
- <span style="color: #e2c027; font-weight: bold;">/zc setset</span> &lt;ID_Bộ&gt;: Thiết lập bộ trang bị kích hoạt thuộc tính.
- <span style="color: #e2c027; font-weight: bold;">/zc soul</span> &lt;give&#124;set&#124;take&gt; &lt;Tên_Người_Chơi&gt; &lt;Số_Lượng&gt;: Quản lý số dư Linh Hồn của người chơi.
- <span style="color: #e2c027; font-weight: bold;">/zc ai</span> &lt;Yêu cầu&gt;: Gửi yêu cầu tới Gemini để tạo vật phẩm bằng AI (Yêu cầu quyền `zamcraft.ai`).
- <span style="color: #e2c027; font-weight: bold;">/zc reload</span>: Tải lại tất cả cấu hình yml mà không cần khởi động lại Server.

---

## 🔑 Hệ Thống Quyền Hạn (Permissions)

- `zamcraft.*`: Cấp toàn bộ quyền hạn của plugin.
- `zamcraft.admin`: Quyền sử dụng tất cả lệnh quản trị, chế tạo và chỉnh sửa lore/nbt vật phẩm.
- `zamcraft.ai`: Quyền sử dụng tính năng sinh đồ bằng AI `/zc ai`.

---

## 🔗 Tích Hợp Tiền Tệ & Plugin Khác

- **Tiền tệ Linh Hồn**: Đây là hệ thống tiền tệ nội bộ của plugin, được lưu độc lập theo UUID người chơi. Sử dụng cho các hoạt động rèn, khảm ngọc và nâng cấp.
- **Vault (Soft-Depend)**: Nếu server có cài Vault, plugin sẽ hỗ trợ tính năng cộng thêm vàng khi tiêu diệt quái vật dựa trên chỉ số `MONEY_BONUS`.
- **MythicMobs**: Bạn có thể thiết lập các chỉ số phần thưởng rơi ra từ quái vật trong tệp cấu hình quái vật:
  - <span style="color: #1abc9c; font-weight: bold;">Exp</span>: Đây là thuộc tính tự định nghĩa riêng (Custom) của AdvancedZamCraft. Bạn cấu hình thêm khoá <code><span style="color: #1abc9c;">Exp: &lt;số_lượng&gt;</span></code> vào tệp cấu hình quái vật để cộng kinh nghiệm khi người chơi hạ quái.
  - <span style="color: #e2c027; font-weight: bold;">Money</span>: Đây là thuộc tính tự định nghĩa riêng (Custom) của AdvancedZamCraft. Bạn cấu hình thêm khoá <code><span style="color: #e2c027;">Money: &lt;số_lượng&gt;</span></code> vào tệp cấu hình quái vật để thưởng tiền vàng khi người chơi hạ quái.
  - <span style="color: #8e44ad; font-weight: bold;">Soul</span>: Đây là thuộc tính tự định nghĩa riêng (Custom) của AdvancedZamCraft. Bạn cấu hình thêm khoá <code><span style="color: #8e44ad;">Soul: &lt;số_lượng&gt;</span></code> vào tệp cấu hình quái vật để cộng Linh Hồn nội bộ khi người chơi hạ quái.
  - *Ví dụ cấu hình:*
    ```yaml
    SkeletionChuaTe:
      Type: SKELETON
      Display: '&c&lKhung Xương Chúa Tể'
      Health: 500
      Damage: 20
      Exp: 80       # Biến của AdvancedZamCraft 
      Money: 200    # Biến của AdvancedZamCraft 
      Soul: 3       # Biến của AdvancedZamCraft
    ```
- **ProtocolLib (Dependency)**: Bắt buộc cài đặt để ẩn các bộ hiển thị sát thương mặc định của Minecraft, giúp plugin tự thiết kế cơ chế hiển thị sát thương dạng Hologram mượt mà và trực quan hơn.

---

## 📊 Biến PlaceholderAPI (PAPI)

Bạn có thể sử dụng các biến này trong Hologram, Scoreboard, Chat, TAB,... để hiển thị thông tin nhân vật:

| Biến Placeholder | Mô tả |
| :--- | :--- |
| <span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_class%</span> | Hệ Phái hiện tại (kèm màu sắc phân biệt) |
| <span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_current_level%</span> | Cấp độ hiện tại của người chơi |
| <span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_next_level%</span> | Cấp độ yêu cầu để có thể Chuyển Sinh lần kế tiếp |
| <span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_rebirth%</span> | Số lần Chuyển Sinh đã thực hiện |
| <span style="color: #8e44ad; font-weight: bold;">%advancedzamcraft_soul%</span> | Số dư **Linh Hồn** hiện tại |
| <span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_statpoints%</span> | Số điểm tiềm năng chưa cộng |
| <span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_strength%</span> | Chỉ số Sức mạnh |
| <span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_agility%</span> | Chỉ số Nhanh nhẹn |
| <span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_vitality%</span> | Chỉ số Thể lực |
| <span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_energy%</span> | Chỉ số Trí tuệ / Năng lượng |
| <span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_dexterity%</span> | Chỉ số Khéo léo |
| <span style="color: #e74c3c; font-weight: bold;">%advancedzamcraft_hp%</span> / <span style="color: #e74c3c; font-weight: bold;">%advancedzamcraft_max_hp%</span> | Lượng máu (HP) hiện tại / tối đa |
| <span style="color: #3498db; font-weight: bold;">%advancedzamcraft_mana%</span> / <span style="color: #3498db; font-weight: bold;">%advancedzamcraft_max_mana%</span> | Lượng năng lượng (Mana) hiện tại / tối đa |
| <span style="color: #2ecc71; font-weight: bold;">%advancedzamcraft_stamina%</span> / <span style="color: #2ecc71; font-weight: bold;">%advancedzamcraft_max_stamina%</span> | Lượng thể lực (Stamina) hiện tại / tối đa |
| <span style="color: #1abc9c; font-weight: bold;">%advancedzamcraft_exp_current%</span> / <span style="color: #1abc9c; font-weight: bold;">%advancedzamcraft_exp_max%</span> | EXP hiện tại ở cấp này / EXP cần để thăng cấp |
| <span style="color: #1abc9c; font-weight: bold;">%advancedzamcraft_exp_percent%</span> | Tỉ lệ % tiến độ thăng cấp (Ví dụ: `72.5%`) |

---

<div style="border-left: 4px solid #27ae60; padding: 6px 12px; margin: 15px 0;">
  <span style="color: #27ae60; font-weight: bold; font-size: 1.1em;">💡 HƯỚNG DẪN CẤU HÌNH:</span><br>
  Để tìm hiểu chi tiết về cách cấu hình tỷ lệ cường hóa, ngọc thuộc tính, hệ phái và các chỉ số RPG, vui lòng truy cập tài liệu <a href="config_guide.md"><strong>config_guide.md</strong></a> ở thư mục gốc của plugin.
</div>
