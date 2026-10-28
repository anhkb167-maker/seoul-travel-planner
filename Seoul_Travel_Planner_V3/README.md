# Seoul Travel Planner — production-ready static build

Data imported from the current Google Sheets workbook.

- Places: 147
- Stops: 37
- Tasks: 13
- Existing expenses: 0
- Place photos currently available: 0

## Included
Mobile-first/PWA interface; Today; Discover; Food; Itinerary; Expenses; Checklist; Naver Map deep links; search and filters; local offline shell.

## Data model
`data.js` is generated from APP_Places, APP_Stops, APP_Tasks and APP_Expenses. It can later be replaced by a server/API that reads Google Sheets.

## Important
This build intentionally does not invent place photos. Missing photos use a neutral Seoul placeholder. Add licensed/user-owned URLs to APP_Places.Photo_URL and regenerate.

## Deployment
Upload the folder contents to any static host (Cloudflare Pages, Netlify, GitHub Pages, etc.). No credentials are required for this static build.


## V3: Lịch trình có thể chỉnh sửa
- Từ thẻ địa điểm chọn **+ Lịch trình**, chọn ngày/giờ.
- Từ timeline chọn **Sửa / sắp xếp** để đổi ngày, giờ, thứ tự hoặc xóa.
- **Ăn gần đây** chuyển sang danh sách quán theo khu vực; **Naver Map** mở bản đồ nếu có địa chỉ.
- Các thay đổi lịch trình được lưu trên trình duyệt bằng localStorage (seoulPlanV3), chưa đồng bộ Google Sheets và không tự chia sẻ giữa thiết bị.
- Dữ liệu gốc 37 điểm dừng vẫn giữ nguyên trong data.js.
