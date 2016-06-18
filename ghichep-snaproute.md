##Chưa đến lúc chúng ta có mạng lưới mở? Có thật sự như vậy?

Đã có 1 sự bùng nổ trong cách đổi mới của trung tâm dữ liệu mạng trong những năm gàn đây bao gồm các SDN software controller như :
White-box switches, các công cụ cho việc ghép chung các mạng doanh nghiệp thuộc sở hữu với những dịch vụ public cloud từ Amazon và những nơi 
khác. Nhưng theo Gartner Group, chỉ mới vài trăm công ty bắt đầu thay đổi một cách thực sự trong phương thức họ xây dựng và vận hành mạng.

Tại SnapRoute, chúng tôi nghĩ một nguyên nhân chính đó là sự thiếu hụt của một trong những thành phần cơ bản còn thiếu : một phần mềm mở tiêu 
chuẩn thực sự cho các switch và router cơ bản ( layer 2 và layer 3). Mặc dù có nhiều nỗ lực trong những năm qua, nhưng các kỹ sư vẫn phải dựa 
vào phần mềm được cung cấp bởi OEMs để vận hành và khắc phục sự cố các sản phẩm của họ. Nếu bạn muốn giám sát các mẫu lưu lượng network theo cách
mà công cụ không hỗ trợ, bạn có thể yêu cầu một tính năng mới, và chờ đợi trong một vài tháng, một vài năm hoặc có thể không bao giờ. Khi các bug
xuất hiện, bạn chỉ có thể gọi điện phàn nàn và cầu mong là sẽ việc sửa chữa sẽ tới sớm. 
Có 1 cách tốt hơn, và tất cả chung ta đều biết nó là gì : mã nguồn mở. Trong khoảng 20 năm gần đây, các shop IT của công ty đã sử dụng Linux để 
xây dựng, giám sát và khắc phục sự cố các server. Rất nhiều trong số họ sử dụng các database mã nguồn mở như MYSQL và MongDB thay thế Oracle. 
Big Data trở thành một từ thường dùng bởi vì các công ty đã có lựa chọn về các công cụ được xây từ công nghệ nguồn mở Hadoop. Gần đây hơn, một số
 công ty thay thế thiết bị lưu trữ độc quyền với hệ thống dựa vào các tiêu chuẩn mở.
Tất nhiên, các công ty nay đang nỗ lực để trì hoãn tới ngày phán xét của mình. Tất cả tranh luận rằng những việc mà các sản phẩm của họ làm được
còn chưa đủ quan trọng và phức tạp để tạo sự tin tưởng tới các cộng đồng mã nguồn mở. Bằng một cách nào đó, các công ty mạng vẫn có thể duy trì 
sự kìm kẹp của họ. Và ai có thể đổ lỗi cho họ đây? Họ kiểm soát khả năng vận hành hệ thống mạng của bạn quá lâu rồi, họ có thể yêu cầu những
mức giá cao hơn nữa. Không có gì ngạc nhiên khi các công ty hàng đầu thế vẫn còn tạo ra 60% lợi nhuận trên các thiết bị mạng của họ, nhiều gấp 
đôi các server Linux kia.

Chúng tôi không tạo ra SnapRoute để làm tổn hại đến lợi ích của bất kỳ ai cả. Thay vào đó, mục tiêu của chúng tôi chính là giải phóng các kỹ sư
 mạng tài năng để họ làm việc bằng hết khả năng của mình, không phải chịu bất kỳ giới hạn bởi nhà cung cấp lock-in. Chúng tôi nghĩ rằng, 
 không, đúng hơn là chúng tôi biết rằng, điều này có thể thúc đẩy sự đổi mới và giảm chi phí cho hàng ngàn công ty.
 
Đội ngũ sáng lập của chúng tôi có một kết hợp của 30 năm kinh nghiệm xây dựng và chạy một số các mạng doanh nghiệp phức tạp nhất trên thế giới, 
trong đó hơn một thập kỷ tại IBM, giúp 20 công ty xây dựng mạng lưới của họ.
Ở cương vị của người sáng lập SnapRoute, tôi không hề xấu hổ khi thừa nhận một bí mật hơi không trong sáng, mà nó sẽ không gây bất ngờ với 
nhiều nhà điều hành mạng hoạt động. Việc tăng lên theo bậc thang của chúng tôi có vẻ ít ý nghĩa với những thành tựu kỹ thuật của riêng tôi và 
nhiều hơn với các khả năng của mình để có được nhà cung cấp. Tôi xây dựng một đại diện như một khẩu súng thuê để giải quyết nhiều thứ khi những
 kỹ năng thực sự và lớn nhất của tôi đã biết gọi cho ai và nói điều gì để có được sự hỗ trợ của Cisco hay nhà cung cấp khác. Đó là một buổi biểu 
 diễn tuyệt vời. Tôi thậm chí không cần phải viết một trường hợp kinh doanh. Chắc chắn, các nhà cung cấp thì cũng có lỗi của mình, nhưng vào cuối 
 ngày, họ đã có sự tin tưởng của tôi.
Nhưng điều không kéo dài. dịch vụ Internet và lượng traffic tăng lên nhanh chóng, tạo ra hàng lớp phức tạp không thể tưởng tượng nổi. Thay vì 
ngừng cấp hoặc hai lần mỗi năm, công ty đã bắt đầu phải nhận tổn thất mỗi quý, và sau đó là mỗi tháng. Tôi bắt đầu nhận được gọi đến trụ sở chính bởi 
higher-ups và bi trừng phạt đối với các vấn đề mạng mà tôi thiếu các công cụ để giải quyết. Các bug, các nâng cấp, và các vấn đề khác đã đến quá 
nhanh, và sự chậm trễ quá lớn. Sau một thời gian, uy tín cá nhân của tôi đã bắt đầu bị nghi ngờ.

Sau đó, tôi đã chọn một công việc tại Apple, nơi mà tôi đã có một vị trí ringside về một trong những bùng nổ hệ thống mạng đầy thử thách trong lịch
 sử. Khi tôi đến vào năm 2011, Apple đã có hai trung tâm dữ liệu, chủ yếu là xử lý traffic nội bộ và sự nhỏ giọt bài hát và các ứng dụng từ cửa 
 hàng âm nhạc iTunes. Vào lúc chúng tôi rời đi, Apple đã có một số trung tâm bị nhồi với một số lượng đáng kinh ngạc của các thiết bị mạng để xử
 lý hàng tỷ Siri và truy vấn Bản đồ, iMessages và các dịch vụ điện toán đám mây.
Thật ly kỳ và đáng sợ. Khi ngay cả một phần trăm traffic của Apple bị đình trệ, đó lập tức là tin tức trên trang nhất. Và tất cả các quá thường
 xuyên, chúng tôi đang đối phó với vấn đề các nhà cung cấp của chúng tôi đã không bao giờ dự tính, ít nhiều đã tìm ra. Chúng tôi bắt đầu khám 
 phá các cách tiếp cận hoàn toàn mới, bao gồm một số các giải pháp được cho là mã nguồn mở nên chúng tôi có thể sử dụng mạng của riêng chúng 
 tôi, có thể nói là nhìn trực tiếp vào các dữ liệu cái mà sắp tắt bộ xử lý mạng. Chúng ta muốn những công nghệ đó để làm việc, còn họ 
 thì không, Vì vậy, chúng tôi phát triển một số của riêng của chúng tôi, bao gồm một công cụ dự phòng cho việc nâng cấp các phần mềm trên hàng 
 ngàn switch mà không cần dùng mạng offline. Nếu bạn chưa từng nghe nói, Apple thích giữ những thành tích bên trong cho chính bản thân 
 họ, vì vậy tôi không thể chia sẻ các kết quả. Hãy chỉ nói rằng chúng tôi có thể thực hiện trong vài phút những thứ nếu làm có thể mất hàng giờ,
 ngày hoặc thậm chí cả tuần.
 
Dần dần, mong muốn của chúng tôi để chia sẻ ý tưởng của chúng tôi với thế giới và bắt đầu làm lu mờ sự hồi hộp và niềm tự hào của việc làm việc 
cho Apple. Nhóm của tôi và tôi rời đi trong năm 2015. Thật lòng mà nói, tôi đã dành một vài ngày khóc trên chiếc ghế dài. Tâm trạng của tôi chỉ
 được cải thiện khi chúng tôi bắt đầu thử nghiệm những ý tưởng của chúng tôi với khách hàng tiềm năng. Rất nhanh chóng, chúng tôi biết chúng tôi 
 có thể làm một cái gì đó, giả sử chúng ta có thể thực hiện. Các nhà cung cấp điện toán đám mây lớn và các công ty bán lẻ, dịch vụ tài chính và 
 các lĩnh vực khác cho biết họ đã phải vật lộn với rất nhiều trở ngại mà chúng tôi đã bắt đầu giải quyết.
 
Có một bối cảnh rộng lớn hơn đằng sau sự quan tâm dồn nén này. Sau nhiều năm quan tâm đến the public cloud, nhiều công ty lớn đang nhận ra họ 
cần phải tiếp tục xây dựng một số cơ sở hạ tầng riêng của mình nếu họ muốn tiếp tục là người đi đầu của sự đổi mới. Sau tất cả, ngay cả các công
 ty đáng kinh ngạc như Amazon, Google và Microsoft không thể đưa ra yêu cầu cụ thể của mọi khách hàng trên vào to-do list của họ. Họ cũng không 
 nên nếu họ muốn tối đa hóa lợi nhuận. Chúng tôi tin rằng khi cơ sở hạ tầng public cloud trở nên phổ biến, các công ty sẽ nhận ra họ cần để 
 phát triển công thức bí mật của họ nếu họ muốn có một lợi thế IT hơn đối thủ cạnh tranh. Nếu không, họ sẽ bị  hạn chế bởi nhà cung cấp 
 điện toán đám mây bởi các nhà cung cấp thiết bị độc quyền của họ. Như Roger Daltrey nói, “Tránh vỏ dưa gặp vỏ dừa”
 
May mắn hay không, tôi chọn tin vào những người đi trước, chúng tôi không phải là công ty duy nhất để nhận ra nhu cầu này. Năm ngoái, Dell đã 
công bố sáng kiến một hệ điều hành mạng mở và hợp tác với các phần khởi động như Cumulus Networks cung cấp một số thứ chúng tôi hướng đến. 
Trong vài tháng qua, HP và Microsoft cũng đã thông báo tương tự.

Chúng tôi tin rằng cách tiếp cận của chúng tôi sẽ nổi bật vì một vài lý do. Với những người mới bắt đầu, nhiều nỗ lực gần đây đã cố gắng để 
xây dựng hệ thống mạng theo kiểu stack tới Linux. Chúng tôi không tin rằng điều này sẽ hiệu quả với các cơ sở hạ tầng phức tạp mà công ty lớn cần. 
Mạng của switch và router đơn giản không phải là các server. Tại Apple, chúng tôi đã hoạt động với một số nhà cung cấp được giả mạo như là công ty 
mã nguồn mở. Nhưng trong khi họ có thể đã được sử dụng (và đóng góp) mã nguồn mở, các sản phẩm của họ lại là độc quyền và đóng.

Thách thức ngắn hạn lớn nhất là để bắt đầu xây dựng một hệ sinh thái của các đối tác, khách hàng và nhà phân phối cho FlexSwitch. 
Chúng tôi đang có một khởi đầu tốt. Dự án OPS vừa công bố rằng nó sẽ cung cấp FlexSwitch như một lựa chọn cho các hệ điều hành mạng OpenSwitch,
 được tạo ra vào năm ngoái. Hãy theo dõi các thông báo nhiều hơn với các nhà cung cấp chip mạng và các thành phần khác, các nhà cung cấp điện
 toán đám mây và khách hàng đầu tiên. Chúng tôi cũng có kế hoạch đóng góp mã nguồn của chúng tôi để chương trình Facebook’s Open Compute Program,
 để khách hàng có thể sử dụng nó trong phần cứng white box được xây dựng với những thông số kỹ thuật.
 
Chúng tôi không có bất kỳ ảo tưởng rằng chúng tôi sẽ tạo ra một cơn bão trong thị trường, chúng tôi cũng không tuyên bố mình sẽ là "Cisco killer"
 Thực tế, chúng tôi tin rằng hầu hết các công ty, chắc chắn những người không có nhiều nhân viên kỹ thuật làm việc tại nhà, hoặc có liên quan tới những nhu cầu của mạng tĩnh,
 đều sẽ tốt hơn các nhà cung cấp thành lập với công nghệ độc quyền chiến đấu thử nghiệm. Thay vào đó, chúng tôi dự định tiến hành với sự khiêm nhường và một 
 chủ nghĩa thực dụng hoạt động có đầu óc để xây dựng một hệ sinh thái để giúp những công ty muốn sử dụng cơ sở hạ tầng Internet như một một lợi thế cạnh tranh
