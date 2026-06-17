# BÀI 3: Đọc hiểu & Dò lỗi qua Prompt

## AI Verification

### 1. Prompt mới do em thiết kế

```text
Em có đoạn code Java dùng để tính thuế VAT 10% cho hóa đơn sản phẩm. Hãy kiểm tra lỗi logic nghiệp vụ, đặc biệt trong trường hợp `amount` là số âm hoặc bằng 0, vì hóa đơn không hợp lệ thì không nên tính VAT. Hãy sửa lại code để chặn trường hợp `amount <= 0` và giải thích ngắn gọn cách sửa.

public class TaxCalculator {

    public static double calculateVAT(double amount) {

        return amount * 0.1;

    }

}
```

### 2. Đoạn code Java đã được AI sửa đổi

```java
public class TaxCalculator {

    public static double calculateVAT(double amount) {

        if (amount <= 0) {
            throw new IllegalArgumentException("Amount must be greater than 0");
        }

        return amount * 0.1;
    }
}
```
