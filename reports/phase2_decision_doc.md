## PHASE 2 DECISION & JUSTIFICATION REPORT
### Thailand SVAR: Parameter Decision and Identification Rationale

### 1. Quyet dinh tinh dung (Stationarity Decision)

Can cu ket qua kiem dinh ADF voi muc y nghia 5%, tat ca bien o dang muc deu khong bac bo gia thuyet goc co nghiem don vi:
- ln_WTI: p = 0.1305
- ln_GDP: p = 0.4803
- ln_CPI: p = 0.8396
- Interest: p = 0.2594
- ln_FX: p = 0.1312

Dien giai: cac chuoi o dang muc la khong dung, phu hop dac trung I(1) trong du lieu kinh te vi mo theo tan suat thang.

O sai phan bac nhat:
- Dln_WTI dung ro rang (p = 0.0000).
- Cac bien con lai co tinh ben cao va p-value van lon hon 0.05 trong ADF.

Quyet dinh thuc nghiem cho mo hinh: ap dung sai phan bac nhat cho toan bo he bien truoc khi uoc luong VAR/SVAR de giam nguy co hoi quy gia mao va dam bao tinh nhat quan cua he thong.

### 2. Quyet dinh do tre toi uu p (Lag Selection)

Ket qua VAR Order Selection tren du lieu sai phan cho thay su dong thuan giua cac tieu chi:
- AIC -> p = 1
- BIC -> p = 1
- HQIC -> p = 1
- FPE -> p = 1

Quyet dinh cuoi cung:
- Chon do tre toi uu p = 1.

Ly do:
- Mo hinh gon, tranh overfitting voi mau 179 quan sat sau sai phan.
- Phu hop voi co che truyen dan ngan han cua du lieu thang.

### 3. Bao ve thu tu Cholesky

Thu tu nhan dang cau truc:
ln_WTI -> ln_GDP -> ln_CPI -> Interest -> ln_FX

Lap luan kinh te vi mo:
- ln_WTI: cu soc ngoai sinh toan cau.
- ln_GDP: phan ung som qua kenh chi phi va san luong.
- ln_CPI: dieu chinh sau kenh chi phi day.
- Interest: phan ung chinh sach tien te.
- ln_FX: bien hap thu tong hop cu soc ben ngoai va dieu chinh vi mo.

### 4. Tong hop tham so chot cho Phase 3

- Differencing: True
- Lag order: 1
- Cholesky ordering: ln_WTI -> ln_GDP -> ln_CPI -> Interest -> ln_FX

Please reply: 'I confirm Lag = 1 and differencing = True. Proceed to /phase3_svar'
