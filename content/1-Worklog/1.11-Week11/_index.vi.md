---
title: "Worklog Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " 1.11. "
---

# Worklog Tuần 11

## Mục tiêu tuần 11:

- Hoàn thiện các bước cuối của project game RoughLife trước giai đoạn báo cáo.
- Sửa và đồng bộ các hiệu ứng quan trọng trong gameplay online như death particle và trạng thái nhân vật.
- Hoàn thiện cơ chế revive cho chế độ chơi online, đảm bảo người chơi có thể hỗ trợ nhau khi bị hạ gục.
- Kiểm thử lại gameplay offline/online, boss room, combat, weapon và UI.
- Bắt đầu áp dụng server AWS vào project, tập trung vào mô hình dedicated server và Amazon GameLift.
- Chuẩn bị minh chứng triển khai AWS để bổ sung vào báo cáo thực tập và project.

## Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
|---|---|---:|---:|---|
| 2 | - Rà soát lại toàn bộ project RoughLife sau khi hoàn thiện gameplay chính.<br>- Kiểm tra các hệ thống quan trọng gồm Player, Boss, Weapon, UI, Lobby và Boss Room.<br>- Xác định các lỗi còn tồn tại trước khi bước vào giai đoạn hoàn thiện cuối. | 29/06/2026 | 29/06/2026 | Project source code, Unity Documentation |
| 3 | - Hoàn thiện và đồng bộ **death particle** trong môi trường online.<br>- Kiểm tra hiệu ứng khi Player bị hạ gục ở Host và Client.<br>- Đảm bảo hiệu ứng chết không chỉ hiển thị local mà được sync đúng cho các người chơi khác.<br>- Sửa lỗi particle không xuất hiện hoặc xuất hiện sai vị trí khi nhân vật chết. | 30/06/2026 | 30/06/2026 | Unity Netcode for GameObjects, Project source code |
| 4 | - Hoàn thiện cơ chế **revive** cho Player online.<br>- Xây dựng logic khi Player bị hạ gục sẽ chuyển sang trạng thái chờ revive.<br>- Cho phép Player khác tiếp cận và thực hiện revive.<br>- Kiểm tra hồi máu sau khi revive thành công.<br>- Đảm bảo trạng thái revive được đồng bộ giữa Host và Client. | 01/07/2026 | 01/07/2026 | Unity Documentation, Netcode for GameObjects |
| 5 | - Kiểm thử cơ chế chết, revive và quay lại Lobby trong Boss Room.<br>- Kiểm tra trường hợp tất cả Player bị hạ gục.<br>- Sửa lỗi Player offline/online bị kẹt trong Boss Room.<br>- Đảm bảo gameplay vẫn hoạt động ổn định sau khi revive hoặc sau khi boss fight kết thúc. | 02/07/2026 | 02/07/2026 | Project source code |
| 6 | - Bắt đầu áp dụng server AWS vào project.<br>- Tìm hiểu mô hình dedicated server cho Unity game online.<br>- Chuẩn bị Linux Dedicated Server Build từ Unity.<br>- Tìm hiểu Amazon GameLift, Fleet, Anywhere Fleet, Alias và Game Session Queue.<br>- Xác định hướng triển khai phù hợp với giới hạn AWS Free Tier và quota hiện tại. | 03/07/2026 | 03/07/2026 | AWS Documentation, Amazon GameLift Documentation, Unity Dedicated Server Documentation |
| 7 | - Thử nghiệm các bước cấu hình AWS cho server game.<br>- Chuẩn bị các minh chứng liên quan đến GameLift, Fleet/Alias/Queue hoặc phương án thay thế khi bị giới hạn quota.<br>- Kiểm tra khả năng kết nối giữa Unity Client và server build.<br>- Ghi nhận các lỗi phát sinh trong quá trình setup AWS server. | 04/07/2026 | 04/07/2026 | AWS Console, Amazon GameLift Documentation |
| CN | - Kiểm thử tổng hợp project sau khi hoàn thiện death particle, revive và bước đầu AWS server.<br>- Tổng hợp các hình ảnh minh chứng đã thực hiện.<br>- Ghi chú các phần cần bổ sung vào báo cáo gồm gameplay, online co-op, revive, server architecture và AWS deployment. | 05/07/2026 | 05/07/2026 | Project source code, AWS Console |

## Kết quả đạt được tuần 11:

- Hoàn thiện thêm các chức năng cuối của project RoughLife trước giai đoạn báo cáo.
- Đồng bộ được hiệu ứng **death particle** trong môi trường online, giúp trạng thái Player bị hạ gục hiển thị rõ ràng hơn giữa Host và Client.
- Hoàn thiện cơ chế **revive** cho Player online, cho phép người chơi hỗ trợ nhau trong quá trình đánh boss.
- Kiểm thử và sửa lỗi liên quan đến trạng thái chết, hồi sinh, quay lại Lobby và xử lý tình huống tất cả Player bị hạ gục.
- Gameplay offline/online ổn định hơn, đặc biệt ở các phần Boss Room, combat, weapon và UI.
- Bắt đầu áp dụng AWS server vào project theo hướng dedicated server.
- Tìm hiểu và thử nghiệm các thành phần AWS liên quan như Amazon GameLift, Fleet, Anywhere Fleet, Alias và Game Session Queue.
- Chuẩn bị được các minh chứng ban đầu cho phần triển khai server game trên AWS.
- Xác định được các giới hạn cần lưu ý khi triển khai GameLift, đặc biệt là quota và phạm vi sử dụng AWS Free Tier.

## Nguồn tham khảo:

- https://cloudjourney.awsstudygroup.com
- https://unity.com
- AWS Documentation
- Amazon GameLift Documentation
- Unity Netcode for GameObjects Documentation
