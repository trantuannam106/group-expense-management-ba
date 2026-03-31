📝 User Stories – Group Expense Management System 
🔐 1. User & Authentication | Quản lý người dùng
🟢 US1: Social Login (Google OAuth) | Đăng nhập Google
Actor | Tác nhân: User (Người dùng)
Priority | Độ ưu tiên: High
Story Points: 5

Description | Mô tả:
As a user, I want to log in using my Google account so that I can quickly access the system without creating a new password.
Là một người dùng, tôi muốn đăng nhập bằng tài khoản Google để có thể truy cập hệ thống nhanh chóng mà không cần tạo mật khẩu mới.

Acceptance Criteria | Tiêu chí chấp nhận:

System displays “Login with Google” button.
Hệ thống hiển thị nút “Đăng nhập bằng Google”.
User is authenticated via Google OAuth.
Người dùng được xác thực thông qua Google OAuth.
On successful login, user is redirected to Main Dashboard.
Sau khi đăng nhập thành công, chuyển hướng đến trang chính.
If first-time login, system creates a new account automatically.
Nếu đăng nhập lần đầu, hệ thống tự động tạo tài khoản.

Edge Cases | Trường hợp đặc biệt:

Login fails due to network error → show error message.
Lỗi mạng → hiển thị thông báo lỗi.
User cancels login → stay on login page.
Người dùng hủy đăng nhập → ở lại trang đăng nhập.
👥 2. Group Management | Quản lý nhóm
🟢 US2: Create Group & Invite Members | Tạo nhóm & mời thành viên
Actor | Tác nhân: Group Admin (Trưởng nhóm)
Priority | Độ ưu tiên: High
Story Points: 8

Description | Mô tả:
As a group admin, I want to create a group and invite members via email so that we can manage shared expenses together.
Là một trưởng nhóm, tôi muốn tạo nhóm và mời thành viên qua email để cùng quản lý chi tiêu chung.

Acceptance Criteria | Tiêu chí chấp nhận:

Admin inputs Group Name.
Trưởng nhóm nhập tên nhóm.
Admin adds member emails.
Thêm email thành viên.
System sends invitations (real-time/email).
Hệ thống gửi lời mời.
Group appears in dashboard.
Nhóm hiển thị trên dashboard.

Edge Cases | Trường hợp đặc biệt:

Email không tồn tại → cảnh báo.
Email trùng → không cho mời trùng.
Tên nhóm rỗng → báo lỗi.
🟢 US3: Join Group | Tham gia nhóm
Actor | Tác nhân: Member (Thành viên)
Priority: High
Story Points: 5

Description | Mô tả:
As a member, I want to accept group invitations so that I can join and participate in group expenses.
Là một thành viên, tôi muốn chấp nhận lời mời để tham gia nhóm và bắt đầu chia sẻ chi tiêu.

Acceptance Criteria | Tiêu chí chấp nhận:

View pending invitations.
Xem danh sách lời mời.
Accept / Reject invitation.
Chấp nhận hoặc từ chối.
Member list updates in real-time.
Danh sách thành viên cập nhật ngay.

Edge Cases:

Lời mời hết hạn → không join được.
Đã ở trong nhóm → không cho join lại.
💰 3. Fund & Budget | Quỹ & Hạn mức
🟢 US4: Fund Contribution | Nạp tiền vào quỹ
Actor: Member (Thành viên)
Priority: High
Story Points: 8

Description | Mô tả:
As a member, I want to contribute money to the group fund so that the group has balance for activities.
Là một thành viên, tôi muốn nạp tiền vào quỹ nhóm để có ngân sách chi tiêu chung.

Acceptance Criteria:

Input amount.
Nhập số tiền.
Validate personal balance.
Kiểm tra số dư.
Update group fund.
Cập nhật quỹ nhóm.
Save transaction history.
Lưu lịch sử giao dịch.

Edge Cases:

Không đủ tiền → báo lỗi.
Số tiền âm → không hợp lệ.
🟢 US5: Budget Alerts | Cảnh báo hạn mức
Actor: Group Admin
Priority: Medium
Story Points: 5

Description | Mô tả:
As a group admin, I want to monitor budget status using colors so that I can control overspending.
Là trưởng nhóm, tôi muốn theo dõi ngân sách bằng màu sắc để kiểm soát chi tiêu.

Acceptance Criteria:

Green: < 80%
Yellow: 80–100%
Red: > 100%
Real-time update
Cập nhật theo thời gian thực.
🧾 4. Expenses & Communication | Chi tiêu & Giao tiếp
🟢 US6: Split Expenses | Chia tiền
Actor: Member
Priority: High
Story Points: 13

Description | Mô tả:
As a member, I want to add expenses and split them fairly.
Là một thành viên, tôi muốn thêm khoản chi và chia tiền công bằng.

Acceptance Criteria:

Add expense.
Thêm khoản chi.
Split methods:
Equal (Chia đều)
Percentage (Theo %)
Custom (Tùy chỉnh)
Auto calculate balances.
Tự động tính toán.

Edge Cases:

Tổng chia ≠ tổng tiền → lỗi.
Giá trị âm → không hợp lệ.
🟢 US7: Group Chat | Chat nhóm
Actor: Member
Priority: Medium
Story Points: 8

Description | Mô tả:
As a member, I want to chat in real-time so that we can discuss expenses.
Là thành viên, tôi muốn chat realtime để trao đổi.

Acceptance Criteria:

Real-time messaging (Socket).
Tin nhắn realtime.
Store chat history.
Lưu lịch sử.
Show timestamp + sender.
Hiển thị thời gian & người gửi.
⚙️ 5. Administration | Quản trị
🟢 US8: Account Security | Bảo mật tài khoản
Actor: System Admin
Priority: Medium
Story Points: 5

Description | Mô tả:
As an admin, I want to lock/unlock accounts to protect the system.
Là admin, tôi muốn khóa/mở tài khoản để bảo vệ hệ thống.

Acceptance Criteria:

Toggle account status.
Chuyển trạng thái.
Locked user cannot login.
Không đăng nhập được.
Show blocked message.
Hiển thị thông báo bị khóa.
