# 📖 HƯỚNG DẪN CẤU HÌNH ADVANCED ZAMCRAFT

## 📂 Danh sách các file Cấu hình

### ⚙️ 1. <span style="color: #2b9fe3; font-weight: bold;">`others.yml`</span> (Cài đặt chung & API)
Nơi chứa các cấu hình chung như tiền thưởng, kinh nghiệm, và kết nối với AI (Gemini).

- **`RankExpBonus`**: Cấu hình tỉ lệ cộng thêm phần trăm (%) Kinh Nghiệm (EXP) khi người chơi có permission rank (ví dụ: `group.vip1`).
- **`RankMoneyBonus`**: Cấu hình tỉ lệ cộng thêm phần trăm (%) Tiền (Money) rớt ra khi giết quái vật nếu người chơi có permission tương ứng. *(Yêu cầu có plugin Vault)*.
- **`GeminiAPIKey & GeminiModel`**: Khóa kết nối API và tên model AI dùng cho lệnh `/zc ai`.

---

### 📊 2. <span style="color: #e2c027; font-weight: bold;">`stats.yml`</span> (Hệ số quy đổi tiềm năng)
Điều chỉnh cách điểm tiềm năng cộng vào nhân vật của bạn sẽ được chuyển đổi ra sát thương hoặc các chỉ số ẩn khác.

- **`StatScales`**:
  - Ví dụ: `STRENGTH_TO_PVE_DAMAGE: 1.5` ➡️ Mỗi 1 điểm **Sức mạnh (Strength)** người chơi sẽ nhận được thêm `1.5` Sát thương PVE.
  - Các hệ số cho: **Sức mạnh** (STRENGTH), **Nhanh nhẹn** (AGILITY), **Thể lực** (VITALITY), **Trí tuệ** (ENERGY), **Khéo léo** (DEXTERITY).

---

### 🛡️ 3. <span style="color: #27ae60; font-weight: bold;">`classes.yml`</span> (Cấu hình Hệ Phái)
Thiết lập chi tiết về các lớp nhân vật (Class), các nhánh kĩ năng và thiên phú.

- **`Classes`**: Mỗi hệ phái (ví dụ: `KNIGHT`, `ARCHER`) có những mục:
  - `BaseStats`: Chỉ số tiềm năng gốc khởi điểm.
  - `BaseRates`: Chỉ số tỉ lệ % khởi điểm (Máu cơ bản, Mana cơ bản...).
  - `Talent1 -> Talent5`: Tên Thiên phú, mô tả và tỉ lệ thưởng (`BonusPerLevel`) khi người chơi tăng 1 cấp điểm thiên phú.
- **`SkillFarm`**: Tầm đánh và sát thương của tính năng đánh lan.
- **`Skills`**: Yêu cầu về năng lượng (Mana) hoặc chỉ số sát thương của từng chiêu thức `Skill1` ➡️ `Skill4`.

---

### ⚔️ 4. <span style="color: #e74c3c; font-weight: bold;">`abilities.yml`</span> (Kỹ năng vũ khí / Chủ động)
Điều chỉnh Sát thương cơ bản và Sát thương tăng tiến mỗi khi vũ khí được nâng cấp.

- **`Abilities`**: Liệt kê các chiêu thức (ví dụ: `CLEAVE`, `FLAME_STRIKE`).
  - `BaseDamage`: Sát thương gốc mặc định.
  - `Base`: Giá trị phụ (nếu có tùy chiêu).
  - `Growth`: Mức sát thương hoặc chỉ số cộng thêm mỗi khi chiêu này được lên 1 cấp độ.

---

### 🌟 5. <span style="color: #9b59b6; font-weight: bold;">`ultimates.yml`</span> (Chiêu Cuối / Kỹ năng tối thượng)
Tương tự như `abilities.yml`, nhưng dùng cho bộ kĩ năng tối thượng (Ultimates).

- Bổ sung thêm thuộc tính **`Range`**: Tầm ảnh hưởng hoặc bán kính tác dụng của chiêu cuối.

---

### 🌌 6. <span style="color: #34495e; font-weight: bold;">`passives.yml`</span> (Nội Tại Hệ Phái)
Cấu hình các sức mạnh ẩn, kích hoạt tự động theo hệ phái.

- Cấu hình tương tự các file kỹ năng khác với `BaseDamage` và `Growth`.
- Riêng hệ thống **Cường Hóa (CuongHoa)**: Cấu hình `PotentialBonusPerLevel` là số điểm tiềm năng (Mọi chỉ số) được cộng thêm ứng với mỗi cấp Cường Hóa người chơi sở hữu.

---

### ⚒️ 7. <span style="color: #d35400; font-weight: bold;">`upgradesmith.yml`</span> (Lò Rèn Cường Hóa)
Cấu hình tỉ lệ đập đồ, loại đá yêu cầu, sát thương cộng thêm.

- **`Materials`**:
  - `DaCuongHoa`: Tên và Lore hiển thị của Đá Cường Hóa.
  - `BuaBaoVe`: Tên và Lore của Bùa Bảo Vệ (giữ không bị rớt cấp khi xịt).
- **`Upgrades`**:
  - `MaxLevel`: Cấp độ cường hóa tối đa (ví dụ: `+15`).
  - `BonusPerLevel`: % Sát thương hoặc thuộc tính tăng lên tương ứng ở mỗi cấp (ví dụ: `0.10` tức là +10%).
  - Bảng `Levels`: Tỉ lệ thành công (`SuccessRate`), số đá yêu cầu (`MaterialCost`), và có tụt cấp khi thất bại hay không (`DowngradeOnFail`).

---

### 🔮 8. <span style="color: #1abc9c; font-weight: bold;">`sets.yml`</span> (Bộ Trang Bị)
Thiết lập sức mạnh kích hoạt khi người chơi mặc theo bộ (Set đồ).

- Mỗi một **`ID_BO`** có:
  - `DisplayName`: Tên bộ (hiển thị trên Item).
  - `Bonuses`:
    - `2` (Mặc 2 món): `Description` (Dòng mô tả), `Stats` (Các chỉ số được kích hoạt ẩn, ví dụ: `MAX_HEALTH: 500`).
    - `4` (Mặc 4 món): ...
    - `5` (Mặc full bộ): ...

---

## 👾 Tính năng kết hợp với MythicMobs

- **Kinh nghiệm từ Mobs (Exp)**: Plugin sử dụng thuộc tính `Exp` mặc định của MythicMobs.
- **Tiền rớt từ Mobs (Vault)**: Sử dụng thuộc tính `Money: <số_lượng>` trong file quái vật.
- **Linh Hồn (ZamSouls)**: Cấu hình thêm thuộc tính `Souls: <số_lượng>` trong file quái vật để khi giết quái, người chơi nhận được Linh Hồn nội bộ.

<div style="border-left: 4px solid #e74c3c; padding: 6px 12px; margin: 15px 0;">
  <span style="color: #e74c3c; font-weight: bold; font-size: 1.1em;">⚠️ LƯU Ý QUAN TRỌNG:</span><br>
  Hãy thêm dòng <code>Souls: &lt;số_lượng&gt;</code> trực tiếp vào file cấu hình quái vật của MythicMobs để kích hoạt tính năng rơi Linh Hồn.
</div>

### 📝 Ví dụ cấu hình quái vật:
```yaml
TestBoss:
  Type: ZOMBIE
  Display: '&cTest Boss'
  Health: 1000
  Damage: 50
  Exp: 100
  Money: 500
  Souls: 5
```

---

## 💾 Quản lý Data Người Chơi

<div style="border-left: 4px solid #2980b9; padding: 6px 12px; margin: 15px 0;">
  <span style="color: #2980b9; font-weight: bold; font-size: 1.1em;">ℹ️ LƯU Ý / THÔNG TIN:</span><br>
  Toàn bộ dữ liệu của người chơi (hệ phái, tiềm năng, số lần chuyển sinh, linh hồn...) được lưu dưới dạng <strong>UUID</strong> tại thư mục: <code>plugins/AdvancedZamCraft/playerdata/&lt;tên người chơi&gt;.yml</code>
</div>

---

## 📜 Danh Sách PlaceholderAPI (Biến)

Bạn có thể dùng các biến này ở mọi plugin hỗ trợ <span style="color: #fcad00ff;">**PAPI** (hologram, scoreboard, chat...).

### 👑 1. Thông tin chung
- <code><span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_class%</span></code>: Hiển thị Hệ Phái (Ví dụ: <span style="color: #e74c3c;">ASSASSIN</span>, <span style="color: #fcad00ff;">KNIGHT</span>...) kèm theo mã màu.
- <code><span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_current_level%</span></code>: Cấp độ hiện tại của người chơi.
- <code><span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_next_level%</span></code>: Cấp độ yêu cầu để Chuyển Sinh (Rebirth) lần kế tiếp.
- <code><span style="color: #9b59b6; font-weight: bold;">%advancedzamcraft_rebirth%</span></code>: Số lần đã chuyển sinh.
- <code><span style="color: #8e44ad; font-weight: bold;">%advancedzamcraft_soul%</span></code>: Số dư <span style="color: #7f8c8d; font-weight: bold;">Linh Hồn</span> hiện có.

### ⚡ 2. Tiềm Năng (Stats)
- <code><span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_statpoints%</span></code>: Điểm tiềm năng chưa cộng.
- <code><span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_strength%</span></code>: Sức mạnh.
- <code><span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_agility%</span></code>: Nhanh nhẹn.
- <code><span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_vitality%</span></code>: Thể lực.
- <code><span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_energy%</span></code>: Trí tuệ / Năng lượng.
- <code><span style="color: #e67e22; font-weight: bold;">%advancedzamcraft_dexterity%</span></code>: Khéo léo.

### 🩸 3. HP / MANA / STAMINA
- <code><span style="color: #e74c3c; font-weight: bold;">%advancedzamcraft_hp%</span></code> & <code><span style="color: #e74c3c; font-weight: bold;">%advancedzamcraft_max_hp%</span></code>: Lượng HP hiện tại / tối đa.
- <code><span style="color: #3498db; font-weight: bold;">%advancedzamcraft_mana%</span></code> & <code><span style="color: #3498db; font-weight: bold;">%advancedzamcraft_max_mana%</span></code>: Lượng Mana hiện tại / tối đa.
- <code><span style="color: #2ecc71; font-weight: bold;">%advancedzamcraft_stamina%</span></code> & <code><span style="color: #2ecc71; font-weight: bold;">%advancedzamcraft_max_stamina%</span></code>: Lượng thể lực hiện tại / tối đa.

### 📈 4. Kinh nghiệm (EXP)
- <code><span style="color: #1abc9c; font-weight: bold;">%advancedzamcraft_exp_current%</span></code>: Số EXP hiện tại ở level này.
- <code><span style="color: #1abc9c; font-weight: bold;">%advancedzamcraft_exp_max%</span></code>: Số EXP cần để lên level tiếp theo.
- <code><span style="color: #1abc9c; font-weight: bold;">%advancedzamcraft_exp_percent%</span></code>: % EXP hiện tại (ví dụ: `85%`).

---

<div style="border-left: 4px solid #27ae60; padding: 6px 12px; margin: 15px 0;">
  <span style="color: #27ae60; font-weight: bold; font-size: 1.1em;">💡 MẸO NHANH:</span><br>
  Bạn có thể tùy ý sửa các file cấu hình. Sau khi lưu, chỉ cần vào game gõ lệnh <strong>/zc reload</strong> (Yêu cầu quyền OP) để cập nhật ngay lập tức cấu hình!
</div>
