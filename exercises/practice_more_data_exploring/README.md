🧪 Bài tập khám phá dữ liệu (Data Exploration) – Dùng adult-census.csv hoặc penguins.csv
📌 PHẦN 1: Tổng quan dữ liệu
1. Tải dữ liệu với pandas.
2. In ra 5 dòng đầu và 5 dòng cuối.
3. Sử dụng .info() và .describe() để mô tả sơ lược về dữ liệu.
4. Có bao nhiêu giá trị bị thiếu? (dùng .isnull().sum())

📌 PHẦN 2: Phân tích từng cột
1. Cột nào là dạng số? Cột nào là dạng phân loại?
2. Với các cột phân loại (như Species, Gender, Workclass, v.v):

Có bao nhiêu giá trị khác nhau? Dùng .unique() và .value_counts()

3. Với các cột số:

Tính trung bình, min, max, độ lệch chuẩn (.mean(), .min(), .std())

📌 PHẦN 3: Trực quan hóa đơn giản (sử dụng seaborn hoặc matplotlib)
1. Vẽ histogram cho cột số Age, Culmen Length, Hours per week, v.v
2. Vẽ biểu đồ cột (countplot) cho các cột phân loại
3. Vẽ boxplot để xem sự phân phối theo Species hoặc Income
4. Vẽ biểu đồ scatter plot giữa 2 cột số và tô màu theo nhãn (target)

📌 PHẦN 4: Tìm hiểu mối quan hệ giữa các cột
1. Có mối tương quan nào giữa các cột số không?
→ Dùng .corr() và heatmap (seaborn.heatmap)
2. Tìm mối liên hệ giữa Age và thu nhập (Income hoặc target)
→ Dùng groupby() kết hợp mean() hoặc count()

📌 PHẦN 5: Thực hành mở rộng
1. Đếm số lượng người có tuổi > 40 và thu nhập > 50K
2. Với mỗi ngành nghề (occupation), tính tỉ lệ người thu nhập >50K
3. Tạo bảng thống kê tổng hợp bằng groupby() theo giới tính và thu nhập

