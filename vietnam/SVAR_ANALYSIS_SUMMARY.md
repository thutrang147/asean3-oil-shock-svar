Phân Tích SVAR Việt Nam – Báo Cáo Tóm Tắt
Ngày: 30/03/2026
Dữ liệu: macro_monthly_15y_vnm.csv
Thời gian: Tháng 01/2006 – Tháng 01/2024 (217 observations) 

DỮ LIỆU CHUNG
Observations: 217
Biến số: WTI, GDP, CPI, Interest rate, Exchange rate
Biến đổi: ln(WTI, GDP, CPI, Exchange rate); Interest rate giữ nguyên

QUYẾT ĐỊNH MÔ HÌNH

Bậc sai phân: d = 1
- Tất cả chuỗi log-level không dừng (I(1))
- Sai phân bậc 1 dừng (I(0))
- Dùng dữ liệu sai phân cho VAR

Lag selection: p = 1
- Tất cả tiêu chí (AIC, BIC, FPE, HQIC) chọn lag = 1
- AIC = −58.94 (lag=1) < −58.87 (lag=2)
- VAR(1) ổn định (inverse roots < 1)

Thứ tự Cholesky: WTI → GDP → CPI → Interest rate → Exchange rate
- WTI ngoại sinh (giá dầu thế giới)
- GDP phản ứng sau 1 tháng
- CPI hấp thụ shock chi phí
- Interest rate phản ứng lạm phát
- Exchange rate điều chỉnh cuối

Kiểm tra phần dư
- Ljung-Box (lag=1): p = 0.51 (ổn)
- Ljung-Box (lag=3): p = 0.004 (có tín hiệu)

THỐNG KÊ MÔ TẢ

Mức log:
- ln(WTI): trung bình 4.23, SD 0.33, khoảng [2.81 – 4.90]
- ln(GDP): trung bình 26.12, SD 0.54, khoảng [24.92 – 26.89]
- ln(CPI): trung bình 4.88, SD 0.30, khoảng [4.16 – 5.25]
- Interest rate: trung bình 9.94%, SD 2.82%, khoảng [6.96% – 16.95%]
- ln(Exchange rate): trung bình 9.94, SD 0.13, khoảng [9.68 – 10.09]

Sai phân bậc 1 (dùng trong VAR):
- Δln(WTI): 0.0006 ± 0.1108, khoảng [−0.57 – 0.55]
- Δln(GDP): 0.0091 ± 0.0062, khoảng [0.002 – 0.032]
- Δln(CPI): 0.0050 ± 0.0043, khoảng [0.0005 – 0.019]
- ΔInterest rate: -0.0086% ± 0.2034%, khoảng [−0.48% – 0.38%]
- Δln(Exchange rate): 0.0019 ± 0.0022, khoảng [−0.0002 – 0.0085]

Mức gốc (raw):
- WTI: trung bình 72.42 USD/bbl, SD 22.08, khoảng [16.55 – 133.88]
- GDP: trung bình 2.50e11 USD, SD 1.14e11, khoảng [6.64e10 – 4.76e11]
- CPI: trung bình 137.4 (index), SD 35.6, khoảng [64.33 – 189.7]
- Interest rate: trung bình 9.94%, SD 2.82%, khoảng [6.96% – 16.95%]
- FX: trung bình 20,922 VND/USD, SD 2,555, khoảng [15,994 – 24,165]


