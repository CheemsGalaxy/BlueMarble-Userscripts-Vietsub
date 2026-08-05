## Hình ảnh xem trước của nhánh [**Custom-Improve**](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/tree/custom-improve) thuộc bản Fork này

| Template | Overlay |
|-|-|
| ![Template](assets/Template.png) | ![Overlay](assets/Overlay.png) |

| Thông tin Pixel | Xuất bản đồ (từ hộp thoại Chia sẻ) |
|-|-|
|Wplace 1.1.1 ~ Hiện tại:<br>![Pixel Info](assets/PixelInfo111.png)<br>Wplace 1.1.0:<br>![Pixel Info](assets/PixelInfo110.png)<br>Wplace 1.0.0:<br>![Pixel Info](assets/PixelInfo100.png) | ![Map Export](assets/ExportMap.png)

Đọc thêm về bản Fork này **[tại đây](#regarding-this-fork)**.

<strong>Cài đặt chỉ với một cú nhấp:</strong> Nhấn vào liên kết dưới đây để cài đặt Blue Marble trực tiếp:

<a href="https://raw.githubusercontent.com/t-wy/Wplace-BlueMarble-Userscripts/main/dist/BlueMarble.user.js" target="_blank" rel="noopener noreferrer"><strong>Phiên bản gốc (Hỗ trợ Userscript)</strong></a>
/
<a href="https://raw.githubusercontent.com/t-wy/Wplace-BlueMarble-Userscripts/custom-improve/dist/BlueMarble.user.js" target="_blank" rel="noopener noreferrer"><strong>Phiên bản Custom Mod</strong></a>

Ngoài ra còn có **[phiên bản Bookmarklet](/dist/BlueMarble.bookmarklet.min.js)** (bao gồm cả [phiên bản Custom Mod](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/custom-improve/dist/BlueMarble.bookmarklet.min.js)).

Để sử dụng, hãy sao chép toàn bộ nội dung và dán vào trường **URL** khi tạo một **Dấu trang (Bookmark)**.

<table>
  <tr>
    <td><a href="#blue-marble">Blue Marble</a></td>
    <td valign="top" rowspan="99"><a href="https://discord.gg/tpeBPy46hf"><img alt="Discord Banner" src="https://discord.com/api/guilds/796124137042608188/widget.png?style=banner4"></a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#regarding-this-fork">Về bản Fork này</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#quick-guide">Hướng dẫn nhanh</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#overview">Tổng quan</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#installation-instructions">Hướng dẫn cài đặt</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#script-settings">Cài đặt Script</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#template-settings">Cài đặt Template</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#how-versioning-works">Quy ước đánh số phiên bản</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#licenses">Giấy phép</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#faq">Câu hỏi thường gặp (FAQ)</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#is-blue-marble-malware">Blue Marble có phải phần mềm độc hại không?</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#how-can-blue-marble-place-pixels-for-me">Blue Marble có thể tự động đặt Pixel như thế nào?</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#how-do-i-hide-the-overlay">Làm thế nào để ẩn Overlay?</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#why-do-game-notifications-appear-on-top-of-the-overlay">Tại sao thông báo trong trò chơi lại hiển thị phía trên Overlay?</a></td>
  </tr>
</table>

<h1>Blue Marble</h1>

## Thông tin về bản phân nhánh này
Đối với người dùng không muốn mua ứng dụng TamperMonkey trên App Store (vì đây là ứng dụng trả phí, khác với các nền tảng trình duyệt khác), ứng dụng Userscripts là giải pháp thay thế miễn phí để quản lý Userscript.

Tuy nhiên, bộ API GM mà Userscripts hỗ trợ ít hơn nhiều so với TamperMonkey, đặc biệt là các API đồng bộ cũ mà Blue Marble đang sử dụng — những API này đã bị Greasemonkey loại bỏ từ phiên bản 4.0+, cần thay thế bằng các phương thức tương ứng:
- `GM_addStyle` → `GM.addStyle`
- `GM_getValue` → `GM.getValue`
- `GM_getResourceText` → Đã được thay thế hoàn toàn (Userscripts không hỗ trợ hàm này)

Xem nhánh **[Custom-Improve](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/tree/custom-improve)** để biết các tính năng và cải tiến mới chưa được hợp nhất vào kho mã gốc:
- Hiển thị số lượt tô màu còn lại bên ngoài nút bấm, tránh bị che bởi Cloudflare Turnstile *(phiên bản 0.85.3)*
- Hiển thị thời gian còn lại để đầy đủ lượt tô màu *(phiên bản 0.85.9)*
- Hiển thị gợi ý màu sắc dưới dạng dấu thập phân thay vì chấm tròn, dễ quan sát hơn *(phiên bản 0.85.2)*
  - Có thể quay lại chế độ chấm tròn từ phiên bản 0.85.46
  - Trên Safari di động, giới hạn kích thước Canvas chỉ cho phép phóng to tối đa 4 lần thay vì 5
- Ghi nhớ các ô bản đồ đã tải để giảm độ trễ và tính toán dư thừa khi nội dung không thay đổi *(phiên bản 0.85.4)*
- Khắc phục lỗi không lưu trạng thái bật/tắt màu sắc *(phiên bản 0.85.1)*
- Khắc phục lỗi hiển thị sai tổng số ô cần tô màu sau khi tải lại trang *(phiên bản 0.85.2)*
- Khắc phục lỗi nút "Bật tất cả" / "Tắt tất cả" không lưu trạng thái *(phiên bản 0.85.13)*
- Khắc phục lỗi chuyển đổi không gian màu trên Firefox *(phiên bản 0.85.16)*
- Hiển thị số ô đã tô màu tương ứng với mỗi màu *(phiên bản 0.85.10)*
- Nhấp vào màu chưa hoàn thành trong danh sách sẽ tự động di chuyển đến ô chưa tô màu của màu đó *(phiên bản 0.85.10)*
- Hỗ trợ di chuyển trực tiếp đến tọa độ ô bản đồ thông qua nút điều hướng bên cạnh ô nhập liệu *(phiên bản 0.85.9)*
- Hiển thị cả tọa độ địa lý bên cạnh tọa độ ô bản đồ *(phiên bản 0.85.5)*
- Tối ưu hóa vòng lặp để phản ứng nhanh hơn *(phiên bản 0.85.7)*
- Cho phép sử dụng nhiều Mẫu cùng lúc *(phiên bản 0.85.11)*
- Thêm nút di chuyển đến góc trên bên trái của Mẫu đang chọn *(phiên bản 0.85.12)*
- Tùy chọn ẩn các màu chưa mở khóa khỏi danh sách màu *(phiên bản 0.85.17)*
- Cung cấp phiên bản Bookmarklet *(phiên bản 0.85.22)*
- Cho phép ẩn các màu đã hoàn thành khỏi danh sách *(phiên bản 0.85.23)*
- Thêm các cách sắp xếp màu sắc khác nhau: theo số ô đã tô/chưa tô, theo sắc độ, theo độ sáng
  - Bổ sung tùy chọn sắp xếp theo mã màu *(phiên bản 0.87.16)*
- Thêm thanh tiến trình bên cạnh mỗi màu trong danh sách *(phiên bản 0.85.24)*
- Hỗ trợ dán các định dạng tọa độ khác nhau vào ô nhập liệu đầu tiên: `a, b, c, d` / `a b c d` / `Tl X: a, Tl Y: b, Px X: c, Px Y: d` *(phiên bản 0.85.28)*
- Cho phép tải tác phẩm về với kích thước chính xác từ bản đồ thông qua nút Chia sẻ, bằng cách chọn hai góc đối diện *(phiên bản 0.85.28)*
- Chế độ tiết kiệm bộ nhớ: chỉ tạo đối tượng hình ảnh khi xử lý Mẫu và giải phóng ngay sau khi hoàn thành *(phiên bản 0.85.33)*
- Cho phép đặt điểm neo cho tọa độ Mẫu (mặc định là góc trên bên trái) *(phiên bản 0.85.34)*
- Hỗ trợ hiển thị vị trí vật phẩm sự kiện (cần cung cấp nguồn dữ liệu JSON, ví dụ: [tệp pumpkin.json của Wplace Archive](https://wplace.samuelscheit.com/tiles/pumpkin.json)) *(phiên bản 0.85.35)*
- Tự động chỉ hiển thị các ô của màu đang được chọn trên Wplace *(phiên bản 0.85.37)*
- Cập nhật nội dung bản đồ ngay khi thay đổi màu hoặc Mẫu *(phiên bản 0.85.38)*
- Cập nhật nội dung bản đồ ngay sau khi gửi ô màu *(phiên bản 0.85.39)*
- Hỗ trợ chuyển đổi giữa các giao diện màu có sẵn của Wplace *(phiên bản 0.85.40)*
- Thử nghiệm tính năng bản đồ lỗi: Đỏ - sai màu, Vàng - chưa tô, Xanh lá - đúng màu *(phiên bản 0.85.46)*
- Tách riêng lớp phủ và lớp hiển thị lỗi khỏi lớp tác phẩm *(phiên bản 0.86.1)*
- Lớp phủ cập nhật ngay lập tức, không cần chờ tải lại dữ liệu *(phiên bản 0.86.1)*
- Cho phép đổi tên Mẫu bằng cách nhấp vào tên Mẫu *(phiên bản 0.86.1)*
- Hỗ trợ di chuyển bản đồ theo đường chéo bằng các phím `W` `A` `S` `D`
  - Được thực hiện bởi [@due2e](https://github.com/due2e) theo yêu cầu [PR #7](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/pull/7)
  - Lưu ý: Wplace có phím tắt mặc định để di chuyển theo chiều ngang/dọc bằng các phím mũi tên, kết hợp phím `Shift` để xoay/nghiêng bản đồ
- Hiển thị thời gian và lý do bị hạn chế tài khoản nếu có *(phiên bản 0.86.6)*
- Thêm các nút điều chỉnh mức phóng to để đảm bảo mỗi ô màu trên ảnh chụp có kích thước bằng nhau, hoặc phóng to ở mức tối thiểu trước khi tác phẩm bị mất
  - Được mở rộng bởi [@Commenter25](https://github.com/Commenter25) theo yêu cầu [PR #13](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/pull/13) *(phiên bản 0.86.15)*
- Cho phép tạo Mẫu đường thẳng/hình tròn từ màu đang chọn bằng cách chọn hai điểm đối diện trên bản đồ
  - Đối với hình tròn: tọa độ nhập vào là tâm, điểm chọn trên bản đồ là một điểm trên đường tròn *(phiên bản 0.86.16)*
- Thêm tùy chọn chỉ tính lỗi cho các màu đang được bật trong bản đồ lỗi *(phiên bản 0.86.14)*
- Khắc phục các lỗi giới hạn từ mã gốc và từ Wplace:
  - Blue Marble: Mẫu vượt qua giới hạn Tl X: 2047 → 0 không hiển thị đúng khi bắt đầu từ Tl X = 0
  - Blue Marble: Tọa độ không cập nhật khi chọn ô tại Tl X = 2047 với tâm bản đồ ở Tl X = 0
  - Blue Marble & Wplace: Nút gắn thẻ lấy tọa độ âm khi chọn ô tại Tl X = 2047 với tâm bản đồ ở Tl X = 0
  - Wplace: Không hiển thị thông tin ô khi chọn tại Tl X = 0 với tâm bản đồ ở Tl X = 2047
- Cho phép tắt tạo lớp phủ trên bản đồ để giảm tải xử lý, phù hợp khi sử dụng cùng các công cụ hiển thị khác *(phiên bản 0.87.15)*
  - Lưu ý: Khi bật tùy chọn này, màu sắc hiển thị trên lớp phủ sẽ do công cụ bên ngoài quản lý

---

## Hướng dẫn nhanh
Nhấp vào tiêu đề để xem nội dung chi tiết:
<details>
  <summary>
    <b>Tải Blue Marble về máy</b>
  </summary>
  <a href="#h%C6%B0%E1%BB%9Bng-d%E1%BA%ABn-c%C3%A0i-%C4%91%E1%BA%ADt">Xem hướng dẫn cài đặt</a>
</details>

<details>
  <summary>
    <b>Có câu hỏi về Blue Marble</b>
  </summary>
  <a href="https://discord.gg/tpeBPy46hf" target="_blank" rel="noopener noreferrer">Tham gia nhóm hỗ trợ trên Discord</a>
  <br>
  <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/discussions/categories/q-a">Đặt câu hỏi trên GitHub</a>
</details>

<details>
  <summary>
    <b>Báo cáo lỗi</b>
  </summary>
  <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/issues/new/choose">Tạo yêu cầu báo cáo lỗi và chọn mục "Báo cáo lỗi"</a>
</details>

<details>
  <summary>
    <b>Đề xuất tính năng mới</b>
  </summary>
  <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/issues/new/choose">Tạo yêu cầu và chọn mục "Đề xuất tính năng"</a>
</details>

<details>
  <summary>
    <b>Đóng góp vào dự án</b>
  </summary>
  <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/CONTRIBUTING.md">Xem quy định đóng góp</a>
</details>

<details>
  <summary>
    <b>Báo cáo lỗ hổng bảo mật</b>
  </summary>
  <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/security">Gửi báo cáo bảo mật</a>
</details>

<details>
  <summary>
    <b>Truy cập trang web chính thức</b>
  </summary>
  <a href="https://bluemarble.camilledaguin.fr/" target="_blank" rel="noopener noreferrer">Mở trang web Blue Marble</a>
</details>

---

## Tổng quan
Chào mừng bạn đến với Blue Marble! Đây là một Userscript dành cho trang web [wplace.live](https://wplace.live/), giúp bạn chồng hình ảnh tác phẩm lên bản đồ một cách dễ dàng — không cần chuyển qua lại giữa các tab hoặc màn hình. Ngoài ra, Blue Marble còn có nhiều tính năng hữu ích khác:
- Hiển thị số ô màu cần tô để lên cấp tiếp theo
- Cung cấp hệ thống tọa độ đầy đủ: tọa độ ô bản đồ và tọa độ ô màu
- Di chuyển bảng màu lên đầu màn hình để thao tác thuận tiện hơn
- Hỗ trợ dùng công cụ lấy màu trực tiếp từ Mẫu nếu màu sắc khớp với bảng màu của Wplace
- ...và nhiều tính năng khác!

Nếu bạn thích dự án này, hãy cho chúng tôi một ⭐ trên GitHub nhé! Để cập nhật thông tin mới nhất, truy cập [trang web chính thức](https://bluemarble.camilledaguin.fr/). Nếu muốn tham gia phát triển, xem chi tiết trong tệp [CONTRIBUTING.md](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/CONTRIBUTING.md).

![Hình ảnh minh họa giao diện Blue Marble](./assets/Showcase1.png)

### Hướng dẫn cài đặt
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Trình duyệt hỗ trợ" src="https://img.shields.io/badge/H%E1%BB%97_tr%E1%BB%A3-Chrome%20%7C%20Firefox%2A%20%7C%20Safari%20%7C%20Edge%20%7C%20Brave-orange?style=flat"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Trình duyệt không hỗ trợ" src="https://img.shields.io/badge/Kh%C3%B4ng_h%E1%BB%97_tr%E1%BB%A3-Firefox%2A%20%7C%20Kiwi%20%7C%20Vivaldi-red?style=flat"></a>

Blue Marble đã được kiểm tra và hoạt động ổn định trên các thiết bị di động. Dự án được phát triển chủ yếu trên Chrome, nhưng có thể hoạt động trên các trình duyệt khác không được liệt kê ở trên. Một số phiên bản hoặc bản phân nhánh của Firefox có thể tương thích hoặc không.

Nhấp vào các mục bên dưới để xem hướng dẫn chi tiết cho trình duyệt của bạn:
<details>
  <summary>
    <b>Cài đặt trên Chrome</b>
  </summary>
  <a href="https://www.youtube.com/watch?v=gg5oiJcftEc" target="_blank" rel="noopener noreferrer"><img alt="Video hướng dẫn cài đặt" src="https://img.shields.io/badge/Xem_video_h%C6%B0%E1%BB%9Bng_d%E1%BA%ABn-gray?style=flat&logo=YouTube&logoColor=white&logoSize=auto&labelColor=darkred"></a>
  <ol>
    <li>Cài đặt tiện ích [TamperMonkey](https://chromewebstore.google.com/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) cho Chrome.
    <br>
    <img alt="Nhấn nút 'Thêm tiện ích'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerChromeInstall1.png"></li>
    <li>Nhấp chuột phải vào biểu tượng TamperMonkey trên thanh tiện ích.
    <br>
    <img alt="Chọn 'Quản lý tiện ích'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerChromeInstall2.png"></li>
    <li>Chọn mục "Quản lý tiện ích".</li>
    <li>Bật chế độ "Chế độ dành cho nhà phát triển".
    <br>
    <img alt="Bật 'Chế độ dành cho nhà phát triển' và 'Cho phép Userscript'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerChromeInstall3.png"></li>
    <li>Bật tùy chọn "Cho phép Userscript".</li>
    <li><strong>Cài đặt nhanh:</strong> Nhấp vào liên kết này để cài đặt trực tiếp Blue Marble: <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/releases/download/pre/BlueMarble.user.js"><strong>Cài đặt Blue Marble</strong></a>
    <br>
    TamperMonkey sẽ tự động nhận diện và hiển thị cửa sổ xác nhận cài đặt.</li>
    <li>Tải lại trang [wplace.live](https://wplace.live/).</li>
  </ol>
</details>

<details>
  <summary>
    <b>Cài đặt trên Microsoft Edge</b>
  </summary>
  <ol>
    <li>Cài đặt tiện ích [TamperMonkey](https://microsoftedge.microsoft.com/addons/detail/iikmkjmpaadaobahmlepeloendndfphd) cho Edge.
    <br>
    <img alt="Nhấn nút 'Tải về'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerEdgeInstall1.png"></li>
    <li>Nhấp chuột phải vào biểu tượng TamperMonkey trên thanh tiện ích.
    <br>
    <img alt="Chọn 'Quản lý tiện ích'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerEdgeInstall2.png"></li>
    <li>Chọn mục "Quản lý tiện ích".</li>
    <li>Bật chế độ "Chế độ dành cho nhà phát triển".
    <br>
    <img alt="Bật 'Chế độ dành cho nhà phát triển'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerEdgeInstall3.png"></li>
    <li>Tải tệp [BlueMarble.user.js](https://github.com/t-wy/Wplace-BlueMarble-Userscripts/releases) trong phần "Tệp đính kèm" của bản phát hành mới nhất.</li>
    <li>Mở trang quản lý của TamperMonkey.
    <br>
    <img alt="Mở trang quản lý TamperMonkey" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerEdgeInstall4.png"></li>
    <li>Kéo thả tệp `BlueMarble.user.js` vào trang quản lý.
    <br>
    <img alt="Kéo thả tệp vào trang quản lý" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerChromeInstall5.png"></li>
    <li>Nhấn nút "Cài đặt" để xác nhận.
    <br>
    <img alt="Nhấn nút 'Cài đặt'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerChromeInstall6.png"></li>
    <li>Bật Blue Marble trong danh sách Userscript của TamperMonkey.
    <br>
    <img alt="Bật Blue Marble" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerChromeInstall7.png"></li>
    <li>Tải lại trang [wplace.live](https://wplace.live/).</li>
  </ol>
</details>

<details>
  <summary>
    <b>Cài đặt trên Firefox</b>
  </summary>
  <ol>
    <li>Cài đặt tiện ích [TamperMonkey](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/) cho Firefox.
    <br>
    <img alt="Nhấn nút 'Thêm vào Firefox'" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/ComputerFireFoxInstall1.png"></li>
    <li><strong>Cài đặt nhanh:</strong> Nhấp vào liên kết này để cài đặt trực tiếp Blue Marble: <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/releases/download/pre/BlueMarble.user.js"><strong>Cài đặt Blue Marble</strong></a>
    <br>
    TamperMonkey sẽ tự động nhận diện và hiển thị cửa sổ xác nhận cài đặt.</li>
    <li>Tải lại trang [wplace.live](https://wplace.live/).</li>
  </ol>
</details>

<details>
  <summary>
    <b>Cài đặt trên Safari bằng Userscripts thay vì TamperMonkey</b>
  </summary>
  <ol>
    <li>Tải ứng dụng [Userscripts](https://apps.apple.com/us/app/userscripts/id1463298887) từ App Store.
    <br>
    Đảm bảo đã cấp quyền đầy đủ cho ứng dụng và bật tiện ích trong cài đặt Safari.</li>
    <br>
    <li>Tải tệp Blue Marble và lưu vào thư mục được chỉ định trong ứng dụng: <a href="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/releases/download/pre/BlueMarble.user.js"><strong>Tải Blue Marble</strong></a>
    <br>
    Userscripts sẽ tự động nhận diện tệp Userscript.</li>
    <li>Tải lại trang [wplace.live](https://wplace.live/).</li>
    <li>Nếu gặp vấn đề trong quá trình cài đặt hoặc sử dụng, vui lòng xem tài liệu tại [kho mã của Userscripts](https://github.com/quoid/userscripts/).</li>
  </ol>
</details>

### Hướng dẫn sử dụng Mẫu
Blue Marble sẽ hiển thị Mẫu với kích thước chính xác như hình ảnh gốc. Ví dụ: hình ảnh cao 500 pixel, rộng 300 pixel sẽ tạo ra Mẫu có kích thước tương tự. Các bước để hiển thị Mẫu trên bản đồ:
<ol>
  <li>Chọn ô màu ở góc trên bên trái của khu vực cần vẽ, ghi lại các giá trị `Tl X`, `Tl Y`, `Px X`, `Px Y`. Bạn có thể nhấp vào biểu tượng gắn thẻ bên cạnh ô nhập liệu để tự động điền tọa độ sau khi chọn ô.
  <br>
  <img alt="Lấy tọa độ cho Mẫu" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/TemplateCoordinates1.png"></li>
  <li>Tải lên tệp hình ảnh định dạng PNG hoặc WEBP.</li>
  <li>Nhấn nút "Tạo Mẫu".</li>
  <li>Nếu Mẫu không hiển thị, hãy thử nhấn nút "Bật Mẫu".</li>
</ol>

### Cài đặt Script
Blue Marble có nhiều tùy chọn cài đặt chi tiết, giúp bạn điều chỉnh cách hoạt động của Script theo nhu cầu sử dụng.

### Cài đặt Mẫu
#### Ô trong suốt
Cách hoạt động của Mẫu trên Blue Marble có một điểm khác biệt so với thông thường: Wplace có màu "Trong suốt" riêng, nên các ô trong suốt trên hình ảnh gốc sẽ được xử lý như sau:
- Nếu muốn một ô có thể tô màu bất kỳ: để ô đó trong suốt trên hình ảnh gốc
- Nếu muốn một ô được tô màu "Trong suốt" của Wplace: tô ô đó bằng màu `#deface` trên hình ảnh gốc

#### Hệ thống tọa độ
##### Tọa độ ô bản đồ
Hệ thống tọa độ của Wplace không dùng tọa độ toàn cục mà tọa độ của mỗi ô sẽ phụ thuộc vào ô bản đồ chứa nó. Khi bạn nhấp vào một ô màu, Blue Marble sẽ hiển thị đầy đủ tọa độ ô bản đồ và tọa độ ô màu — đây là các giá trị bạn cần dùng để căn chỉnh Mẫu.
<br>
<img alt="Vị trí hiển thị tọa độ ô bản đồ" src="https://github.com/t-wy/Wplace-BlueMarble-Userscripts/blob/main/docs/assets/TemplateCoordinatesDisplay.png">

##### Tọa độ Mẫu
Mặc định, Mẫu sẽ được căn chỉnh dựa trên góc trên bên trái. Bạn có thể dùng biểu tượng gắn thẻ để tự động điền tọa độ vị trí cần đặt Mẫu.

---

## Quy tắc đánh số phiên bản
Blue Marble tuân thủ nghiêm ngặt quy tắc **[Đánh số phiên bản theo ngữ nghĩa](https://semver.org/)** với định dạng `X.Y.Z`:
- **X (phiên bản chính):** Tăng khi có thay đổi không tương thích ngược, hoặc khi Wplace cập nhật làm thay đổi cấu trúc khiến Script không hoạt động
- **Y (phiên bản phụ):** Tăng mỗi khi cập nhật tính năng mới hoặc sửa lỗi ổn định
- **Z (phiên bản sửa lỗi):** Tăng khi phát hành bản thử nghiệm hoặc sửa lỗi nhỏ chưa ảnh hưởng đến chức năng chung

---

## Giấy phép
Toàn bộ mã nguồn của Blue Marble được phát hành theo giấy phép **[MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/)**. Hình ảnh logo "Blue Marble" do NASA cung cấp và được bảo vệ theo giấy phép **[CC0 1.0 Quốc tế](https://creativecommons.org/publicdomain/zero/1.0/deed.vi)**.

---

## Câu hỏi thường gặp
### Blue Marble có phải là mã độc không?
**Trả lời:** Hoàn toàn không. Toàn bộ mã nguồn được công khai trong thư mục `src/`. Nếu bạn còn nghi ngờ, hoàn toàn có thể xem xét mã nguồn hoặc tự xây dựng tệp Script từ mã nguồn gốc.

### Blue Marble có thể tự động tô màu giúp tôi không?
**Trả lời:** Không. Việc tự động tô màu trái với quy định của Wplace, nên tính năng này sẽ không bao giờ được phát triển.

### Làm thế nào để ẩn lớp phủ Mẫu?
**Trả lời:** Tắt Blue Marble trong quản lý Userscript và tải lại trang Wplace.

### Làm thế nào để phân biệt các màu với nhau?
**Trả lời:** Tìm màu tương ứng trong danh sách lọc màu, dùng dấu chọn để bật/tắt màu đó. Để thuận tiện, bạn có thể nhấn "Tắt tất cả", sau đó chỉ bật màu cần tô — khi đó trên Mẫu sẽ chỉ hiển thị các ô của màu đang được chọn.

### Làm thế nào để lấy màu của một ô trên Mẫu?
**Trả lời:** Dùng công cụ lấy màu có sẵn của Wplace. Nếu màu sắc trên Mẫu khớp hoàn toàn với bảng màu của Wplace, bạn có thể nhấp trực tiếp vào ô màu trên Mẫu để lấy màu tương ứng.

### Tại sao thông báo của Wplace lại hiển thị phía trên lớp phủ?
**Trả lời:** Các thông báo hệ thống được ưu tiên hiển thị cao nhất để bạn không bỏ lỡ thông tin quan trọng.

---
