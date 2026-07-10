---
title: "Worklog Tuần 9"
date: 2026-06-15
weight: 9
chapter: false
pre: "<b>1.9.</b>"
---

# Worklog Tuần 9

## Mục tiêu tuần 9

- Hoàn thiện nền tảng gameplay top-down cho dự án game 2D co-op boss fight.
- Chuyển đổi các hệ thống cũ từ platformer sang top-down, đặc biệt là movement, aim, combat và weapon.
- Xây dựng cơ chế boss Minotaur nhiều trạng thái, nhiều kỹ năng và tương tác với knockback, block, parry.
- Kiểm thử multiplayer ban đầu bằng Unity Netcode for GameObjects.

## Các công việc cần triển khai trong tuần này

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Phân tích lại project Unity hiện tại, xác định hướng chuyển game từ platformer sang top-down co-op boss fight, thiết lập Player top-down movement và cấu hình điều khiển theo owner trong môi trường online. | 15/06/2026 | 15/06/2026 | Unity Documentation, Netcode for GameObjects |
| Thứ 3 | Xây dựng nền tảng Boss Minotaur, thiết kế state machine gồm Move, ChooseSkill, Attack và Stun, bổ sung dữ liệu boss như phase, movement speed, cooldown và damage multiplier. | 16/06/2026 | 16/06/2026 | Unity Documentation, Project source code |
| Thứ 4 | Tích hợp Core combat system cho Boss và Player, kết nối Stats, Health, Poise, DamageReceiver và KnockBackReceiver, test boss knockback lên Player và xử lý stun khi Poise về 0. | 17/06/2026 | 17/06/2026 | Project source code |
| Thứ 5 | Chuyển Weapon system từ platformer sang top-down, thiết kế một vũ khí chính với hai kỹ năng chuột trái và chuột phải, setup Sword với normal attack, Block và Parry, sửa hướng Block/Parry theo top-down aim. | 18/06/2026 | 18/06/2026 | Unity Documentation, Project source code |
| Thứ 6 | Debug cơ chế Block và Parry, sửa lỗi null reference liên quan đến TopDownAim, DamageReceiver và KnockBackReceiver, test cửa sổ Block/Parry bằng animation events và đảm bảo Player không bị knockback liên tục. | 19/06/2026 | 19/06/2026 | Project source code |
| Thứ 7 | Hoàn thiện bước đầu các vũ khí test như Sword, Bow và Staff, kiểm tra input chuột trái/chuột phải, tinh chỉnh animation events cho AttackAction, EnterAttackPhase và AnimationFinished. | 20/06/2026 | 20/06/2026 | Unity Documentation, Project source code |
| Chủ nhật | Kiểm thử tổng hợp gameplay offline và local online, kiểm tra Player movement, aim direction, animation sync và combat interactions, ghi nhận lỗi cần xử lý trong tuần tiếp theo. | 21/06/2026 | 21/06/2026 | Netcode for GameObjects, Project source code |

## Kết quả đạt được tuần 9

- Hoàn thiện nền tảng Player top-down movement gồm di chuyển 4 hướng bằng Rigidbody2D và aim theo chuột.
- Đồng bộ movement direction và aim direction trong môi trường online, đảm bảo chỉ owner mới điều khiển Player của mình.
- Xây dựng state machine cho Boss Minotaur gồm Move, ChooseSkill, Attack, Stun và phase transition.
- Triển khai nền tảng Boss Minotaur 2 phase với các kỹ năng Melee Attack, AOE Attack, Range Attack, Dash Attack và Defend.
- Tích hợp Boss với Core combat system gồm Health, Poise, DamageReceiver, KnockBackReceiver, ParryReceiver và Death handling.
- Chuyển Weapon system sang top-down với kỹ năng chính chuột trái và kỹ năng phụ chuột phải.

## Nguồn tham khảo

- Unity Documentation
- Netcode for GameObjects
- Project source code
