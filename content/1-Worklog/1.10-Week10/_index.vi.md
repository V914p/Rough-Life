---
title: "Worklog Tuần 10"
date: 2026-06-22
weight: 10
chapter: false
pre: "<b>1.10.</b>"
---

# Worklog Tuần 10

## Mục tiêu tuần 10

- Hoàn thiện hệ thống vũ khí top-down với nhiều loại weapon.
- Bổ sung hiệu ứng hình ảnh cho attack, Block, Parry và projectile.
- Tạo công cụ debug để dễ xem và chỉnh hitbox, block direction và parry direction.
- Kiểm thử đầy đủ cơ chế online trong Unity.
- Chuẩn bị bước đầu để build game và đưa server online lên AWS.

## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Hoàn thiện flow Lobby và Map Lobby, thiết kế flow vào Boss Room, test spawn Player online/offline và chuẩn bị scene BossRoom_Minotaur. | 22/06/2026 | 22/06/2026 | Unity Documentation, Netcode for GameObjects |
| Thứ 3 | Setup Cinemachine camera cho top-down gameplay, cấu hình camera follow local player, setup CameraBounds, sửa lỗi Player bị đẩy ra ngoài map và kiểm tra camera ở offline/online. | 23/06/2026 | 23/06/2026 | Unity Cinemachine Documentation |
| Thứ 4 | Hoàn thiện gameplay UI system, liên kết Stats với Health, Mana và Poise UI, kiểm tra Weapon Pickup offline/online, sửa lỗi weapon pickup và đồng bộ WeaponData sai. | 24/06/2026 | 24/06/2026 | Unity Documentation, Project source code |
| Thứ 5 | Tối ưu NetworkPlayer và PlayerMove, test nhiều client trong cùng LobbyScene, sửa lỗi NetworkManager và UnityTransport, test Player online di chuyển, aim, đổi weapon và vào map. | 25/06/2026 | 25/06/2026 | Netcode for GameObjects |
| Thứ 6 | Hoàn thiện nhiều loại weapon: Sword, Spear, Bow và Staff. Setup Spear combo và quick Parry, Bow Rapid Fire/Burst Rapid Fire, Staff homing magic bolt và heal aura, thêm icon kỹ năng vào WeaponData. | 26/06/2026 | 26/06/2026 | Unity Documentation, Project source code |
| Thứ 7 | Thiết kế Slash Effect Prefab, setup Shield Wave khi Block, Hold Pulse khi giữ Block, Spark effect khi Block/Parry thành công và projectile trail cho Arrow/Magic Bolt. | 27/06/2026 | 27/06/2026 | Unity Documentation, Project source code |
| Chủ nhật | Tạo hitbox debug tool cho ActionHitBox, vẽ preview hướng Block và Parry trong Scene View, tinh chỉnh vùng đánh cho Sword, Spear và Shield, chuẩn bị kiến trúc AWS gồm EC2, Lambda Function URL và DynamoDB, bắt đầu xử lý Linux Dedicated Server build và SSH tới EC2. | 28/06/2026 | 28/06/2026 | AWS Documentation, Unity Dedicated Server Documentation |

## Kết quả đạt được tuần 10

- Hoàn thiện hệ thống vũ khí top-down với nhiều loại weapon: Sword, Spear, Bow và Staff.
- Sword hỗ trợ combo, Block và Parry; Spear hỗ trợ combo chuột trái và quick Parry chuột phải.
- Bow hỗ trợ Rapid Fire và Burst Rapid Fire; Staff hỗ trợ homing magic bolt và kỹ năng heal/buff.
- Bổ sung hệ thống icon kỹ năng cho WeaponData gồm icon kỹ năng chính, icon kỹ năng phụ, tên kỹ năng chính và tên kỹ năng phụ.
- Hoàn thiện visual feedback cho combat như Slash Effect, Stab Effect, Shield Wave, Hold Pulse, Spark Effect và projectile trails.
- Tạo công cụ debug giúp hiển thị ActionHitBox, Block Direction, Parry Direction và vùng đánh thật khi animation event được gọi.
- Kiểm thử online trong Unity hoạt động tốt: Host/Client có thể vào Lobby, Player online có thể di chuyển, aim và dùng weapon.
- Chuẩn bị hướng triển khai AWS ban đầu với EC2, Lambda Function URL, DynamoDB, Unity Linux Dedicated Server và SSH connection tới EC2.

## Nguồn tham khảo

- AWS Documentation
- Unity Dedicated Server Documentation
- Netcode for GameObjects
- Project source code
