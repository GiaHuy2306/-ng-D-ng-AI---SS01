# BÀI 2: Tối ưu Prompt

## Tối ưu Prompt: Giải nghĩa logic code Java

### 1. Nội dung Prompt sau khi tối ưu

```text
Hãy giải thích ngắn gọn hàm Java dưới đây cho một người mới học lập trình. Tập trung vào điều kiện rẽ nhánh `points >= 1000` và ý nghĩa của hai kết quả trả về `"VIP"` và `"Standard"`.

public class MemberCheck {

    public static String checkLevel(int points) {

        if (points >= 1000) {

            return "VIP";

        }

        return "Standard";

    }

}
```

### 2. Đoạn phản hồi nhận được từ AI sau khi chạy thử prompt

```text
Hàm `checkLevel(int points)` dùng để kiểm tra hạng thành viên của khách hàng dựa trên số điểm tích lũy.

Nếu biến `points` có giá trị lớn hơn hoặc bằng 1000, điều kiện `points >= 1000` đúng, chương trình sẽ trả về kết quả `"VIP"`. Điều này có nghĩa là khách hàng có đủ điểm để được xếp hạng VIP.

Nếu `points` nhỏ hơn 1000, điều kiện trong câu lệnh `if` sai, chương trình sẽ bỏ qua phần trả về `"VIP"` và đi xuống dòng `return "Standard";`. Khi đó, khách hàng được xếp hạng `"Standard"`.

Tóm lại:
- Từ 1000 điểm trở lên: trả về `"VIP"`.
- Dưới 1000 điểm: trả về `"Standard"`.
```
