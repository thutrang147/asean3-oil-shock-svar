Phân Tích SVAR Việt Nam – Báo Cáo Tóm Tắt
Ngày: 31/03/2026
Dữ liệu: macro_monthly_15y_vnm.csv
Thời gian: Tháng 01/2006 – Tháng 01/2024 (217 observations) 

DỮ LIỆU CHUNG
Observations: 217
Biến số: WTI, GDP, CPI, Interest rate, Exchange rate
Biến đổi: ln(WTI, GDP, CPI, Exchange rate); Interest rate giữ nguyên

QUYẾT ĐỊNH MÔ HÌNH

Bậc sai phân: d = 1, D = 1
- Dùng sai phân bậc 1 + sai phân mùa vụ (lag 12)

Lag selection: p = 2
- Tiêu chí thông tin cho kết quả chia đôi: AIC = 12, FPE = 12; BIC = 1, HQIC = 1
- Theo rule majority vote dựa trên diagnostics (Ljung-Box + stability + normality proxy), lag đầu tiên đạt 3/3 là p = 2
- VAR(2) ổn định (inverse roots < 1)

Thứ tự Cholesky: WTI → GDP → CPI → Interest rate → Exchange rate
- WTI ngoại sinh (giá dầu thế giới)
- GDP phản ứng sau 1 tháng
- CPI hấp thụ shock chi phí
- Interest rate phản ứng lạm phát
- Exchange rate điều chỉnh cuối

THỐNG KÊ MÔ TẢ

Mức log:
- ln(WTI): trung bình 4.23, SD 0.33, khoảng [2.81 – 4.90]
- ln(GDP): trung bình 26.12, SD 0.54, khoảng [24.92 – 26.89]
- ln(CPI): trung bình 4.88, SD 0.30, khoảng [4.16 – 5.25]
- Interest rate: trung bình 9.94%, SD 2.82%, khoảng [6.96% – 16.95%]
- ln(Exchange rate): trung bình 9.94, SD 0.13, khoảng [9.68 – 10.09]

Sai phân bậc 1 (bảng mô tả Part 2.2):
- Δln(WTI): 0.0006 ± 0.1108, khoảng [−0.5682 – 0.5459]
- Δln(GDP): 0.0091 ± 0.0062, khoảng [0.0020 – 0.0319]
- Δln(CPI): 0.0050 ± 0.0043, khoảng [0.0005 – 0.0191]
- ΔInterest rate: -0.0086% ± 0.2034%, khoảng [−0.4762% – 0.3836%]
- Δln(Exchange rate): 0.0019 ± 0.0022, khoảng [−0.0002 – 0.0085]

Mức gốc (raw):
- WTI: trung bình 72.42 USD/bbl, SD 22.08, khoảng [16.55 – 133.88]
- GDP: trung bình 2.50e11 USD, SD 1.14e11, khoảng [6.64e10 – 4.76e11]
- CPI: trung bình 137.40 (index), SD 35.60, khoảng [64.33 – 189.70]
- Interest rate: trung bình 9.94%, SD 2.82%, khoảng [6.96% – 16.95%]
- FX: trung bình 20,921.97 VND/USD, SD 2,555.41, khoảng [15,994.25 – 24,164.89]


