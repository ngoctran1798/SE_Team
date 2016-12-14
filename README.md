##TÌM HIỂU GITHUB  
  
  ___  
    
###1.Github là gì?   
- Github được gọi là social network dành cho developer đi vào hoạt động tháng 2 năm 2008.  
- Là một dịch vụ sử dụng hệ thống quản lý phân tán GIT giúp người dùng lưu trữ source code cho các dự án.  
- Tính năng của GIT như bài trước mình đã nói, nó có mọi tính năng của một source control như SVN và hơn thế nữa.
- Github được viết bằng Ruby on Rails.  
- GitHub cung cấp dịch vụ thương mại và cả tài khoản miễn phí cho các dự án nguồn mở.  
- Theo khảo sát của người sử dụng Git vào năm 2009, Github hiện đang là server Git lưu trữ source code phổ biến nhất hiện nay .  

###2.Cách thức làm việc với github    
- Làm việc với repository ở local: với 2 command thường dùng là git add và git commit    
`git add`: add file đã thay đổi vào stage git commit: commit các file đã add vào stage lên repository ở local Ngoài ra bạn xem một số command khác.  
- Làm việc với repository ở server github:  
  - Sau khi đã quậy tè le ở local , cuối cùng khi có một bản ổn định và hoàn tất (có thông qua test) ta sẽ quyết định cập nhật nó lên repository server với: -push: push thay đổi từ repository local lên repository server -fetch: cập nhật thay đổi từ repository server về repository local -pull/rebase: sao chép source code từ server về local workspace (tương đương checkout của SVN)    
    
###3.Các khái niệm  
-**ADD**:Bạn có thể đề xuất thay đổi (thêm nó vào chỉ mục Index) bằng cách sử dụng lệnh:
```git add <tên tập tin>   
   git add *```   
-**Remove**: Xoá file đã tồn tại trong git và cập nhật gitignore giữa chừng dự án.  
-**Commit**: ghi lại việc thêm/thay đổi file hay thư mục vào repository.  
Khi thực hiện commit, trong repository sẽ tạo ra commit (hoặc revision) đã ghi lại sự khác biệt từ trạng thái đã commit lần trước với trạng thái hiện tại.  
Commit này đang được chứa tại repository, các commit nối tiếp với nhau theo thứ tự thời gian. Bằng việc lần theo commit này từ trạng thái mới nhất thì có thể biết được lịch sử thay đổi trong quá khứ hoặc nội dung thay đổi đó.  
```Git commit```  
-**Push**: đẩy những thay đổi từ máy trạm vào máy chủ.  
-**Pull**: Lấy tệp mã nguồn từ máy chủ về máy trạm  
-**Fetch**: hủy tất cả thay đổi và commit cục bộ, lấy về (fetch) lịch sử gần nhất từ máy chủ và trỏ nhánh master cục bộ vào nó **-Clone:** sao chép 1 repository có sẵn ở trên máy cục bộ hoặc trên máy chủ khác.  
```git clone /đường-dẫn-đến/repository/```  
Nếu repository đó ở máy chủ khác  
```git clone tênusername@địachỉmáychủ:/đường-dẫn-đến/repository```  

Fork: copy project có sẵn thành project cá nhân, rồi sau đó ta có thể tự do chỉnh sửa project đó

