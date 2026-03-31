📝 User Stories: Group Expense Management System
1. User & Authentication | Quản lý người dùng
US1: Social Login | Đăng nhập mạng xã hội
As a user, I want to log in using my Google account, so that I can access the system quickly.
Là một người dùng, tôi muốn đăng nhập bằng tài khoản Google, để truy cập hệ thống nhanh chóng mà không cần nhớ mật khẩu mới.
Acceptance Criteria (AC):
System displays "Login with Google" button.
Successful login redirects to the Main Dashboard.

2. Group Management | Quản lý nhóm
US2: Create & Invite | Tạo nhóm & Mời thành viên
As a group admin, I want to create a group and invite members via email, so that we can manage shared costs.
Là một trưởng nhóm, tôi muốn tạo nhóm và mời thành viên qua email, để cùng nhau quản lý các khoản chi chung.
AC:
Admin can input Group Name and member emails.
System sends real-time invitations to invited users.

US3: Join Group | Tham gia nhóm
As a member, I want to accept group invitations from my notification center, so that I can join the team.
Là một thành viên, tôi muốn chấp nhận lời mời vào nhóm từ trung tâm thông báo, để bắt đầu tham gia chi tiêu cùng nhóm.
AC:
Pending invitations are listed clearly.
Joining a group updates the member list in real-time.

3. Fund & Budget | Quản lý Quỹ & Hạn mức
US4: Fund Contribution | Nạp tiền vào quỹ nhóm
As a member, I want to contribute money from my personal wallet to the group fund, so that the group has a balance for activities.
Là một thành viên, tôi muốn nạp tiền từ ví cá nhân vào quỹ nhóm (Hũ chi tiêu), để nhóm có số dư thực hiện các hoạt động chung.
AC:
System validates personal balance before contribution.
Group balance increases and transaction history is recorded.

US5: Budget Alerts | Cảnh báo hạn mức chi tiêu
As a group admin, I want to see color-coded status based on the budget limit, so that I can control overspending.
Là một trưởng nhóm, tôi muốn thấy trạng thái bằng màu sắc dựa trên hạn mức chi tiêu, để kiểm soát việc chi tiêu quá độ.
AC:
Green (Xanh): Spending < 80% budget.
Yellow (Vàng): Spending 80% - 100% budget.
Red (Đỏ): Spending > 100% (Over budget).

4. Expenses & Communication | Chi tiêu & Giao tiếp
US6: Split Expenses | Chia sẻ hóa đơn
As a member, I want to add expenses and choose a split method, so that costs are shared fairly.
Là một thành viên, tôi muốn thêm khoản chi và chọn cách chia tiền, để chi phí được phân bổ công bằng.
AC:
Support split by: Equal, Percentage, or Custom amount.
Automated balance calculation for all involved members.

US7: Group Chat | Nhắn tin nội bộ
As a member, I want to chat with others in the group room, so that we can discuss financial matters instantly.
Là một thành viên, tôi muốn chat với mọi người ngay trong phòng, để thảo luận về các khoản chi tiêu hoặc kế hoạch trả nợ.
AC:
Messages are sent and received in real-time via Socket.

5. Administration | Quản trị hệ thống
US8: Account Security | Bảo mật tài khoản
As a system admin, I want to lock or unlock user accounts, so that I can protect the system from suspicious users.
Là một quản trị viên hệ thống, tôi muốn khóa hoặc mở khóa tài khoản người dùng, để bảo vệ hệ thống khỏi các hành vi nghi ngờ.
AC:
Admin can toggle "Locked" status in Admin Dashboard.
Locked users cannot log in and receive a "Blocked" notification.
