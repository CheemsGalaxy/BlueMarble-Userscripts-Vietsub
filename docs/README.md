Hình ảnh xem trước của [Nhánh Tùy chỉnh-Cải tiến](https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/tree/custom-improve) của Fork này:

| Bản mẫu | Lớp phủ |
|-|-|
| ![Bản mẫu](assets/Template.png) | ![Lớp phủ](assets/Overlay.png) |

| Thông tin Pixel | Xuất Bản đồ (Từ Hộp thoại Chia sẻ) |
|-|-|
|Wplace 1.1.1 ~ Hiện tại:<br>![Thông tin Pixel](assets/PixelInfo111.png)<br>Wplace 1.1.0:<br>![Thông tin Pixel](assets/PixelInfo110.png)<br>Wplace 1.0.0:<br>![Thông tin Pixel](assets/PixelInfo100.png) | ![Xuất Bản đồ](assets/ExportMap.png)

Thêm thông tin về Fork này **[Tại đây](#regarding-this-fork)**.

<strong>Cài đặt một lần:</strong> Nhấp vào liên kết này để cài đặt Blue Marble trực tiếp: <a href="https://raw.githubusercontent.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/main/dist/BlueMarble.user.js" target="_blank" rel="noopener noreferrer"><strong>Phiên bản Gốc với Hỗ trợ Userscripts</strong></a> / <a href="https://raw.githubusercontent.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/main/dist/BlueMarbleVietsub.user.js" target="_blank" rel="noopener noreferrer"><strong>Phiên bản Mod Tùy chỉnh</strong></a>

**📥 Cài đặt một lần:**

| Phiên bản | Tải xuống |
|-----------|-----------|
| 📦 Bản Gốc(SwingTheVine/) | [Tải về](https://raw.githubusercontent.com/SwingTheVine/Wplace-BlueMarble/main/dist/BlueMarble.user.js) |
| 🔧 Bản mod(T-wy) | [Tải về](https://raw.githubusercontent.com/t-wy/Wplace-BlueMarble-Userscripts/main/dist/BlueMarble.user.js) |
| 🇻🇳 Bản Vietsub từ bản mod bởi T-wy(CheemsGalaxy) | [Tải về](https://raw.githubusercontent.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/main/dist/BlueMarbleVietsub.user.js) |
| 📑 Bookmarklet | [Tải về](/dist/BlueMarble.bookmarklet.min.js) |

<table>
  <tr>
    <td><a href="#blue-marble">Blue Marble</a></td>
    <td valign="top" rowspan="99"><a href="https://discord.gg/tpeBPy46hf"><img alt="Discord Banner" src="https://discord.com/api/guilds/796124137042608188/widget.png?style=banner4"></a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#regarding-this-fork">Về fork này</a></td>
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
    <td>&emsp;&emsp;<a href="#script-settings">Cài đặt tập lệnh</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#template-settings">Cài đặt bản mẫu</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#how-versioning-works">Cách thức hoạt động của phiên bản</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#licenses">Giấy phép</a></td>
  </tr>
  <tr>
    <td>&emsp;<a href="#faq">Câu hỏi thường gặp</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#is-blue-marble-malware">Blue Marble có phải là phần mềm độc hại không?</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#how-can-blue-marble-place-pixels-for-me">Blue Marble có thể đặt pixel cho tôi bằng cách nào?</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#how-do-i-hide-the-overlay">Làm thế nào để ẩn lớp phủ?</a></td>
  </tr>
  <tr>
    <td>&emsp;&emsp;<a href="#why-do-game-notifications-appear-on-top-of-the-overlay">Tại sao thông báo trò chơi xuất hiện trên lớp phủ?</a></td>
  </tr>
</table>

<h1>Blue Marble</h1>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Phiên bản mới nhất" src="https://img.shields.io/badge/Latest_Version-0.92.0-lightblue?style=flat"></a>
<a href="https://github.com/SwingTheVine/Wplace-BlueMarble/releases" target="_blank" rel="noopener noreferrer"><img alt="Bản phát hành mới nhất" src="https://img.shields.io/github/v/release/SwingTheVine/Wplace-BlueMarble?sort=semver&style=flat&label=Latest%20Release&color=blue"></a>
<a href="https://github.com/SwingTheVine/Wplace-BlueMarble/blob/main/LICENSE.txt" target="_blank" rel="noopener noreferrer"><img alt="Giấy phép phần mềm: MPL-2.0" src="https://img.shields.io/badge/Software_License-MPL--2.0-slateblue?style=flat"></a>
<a href="https://discord.gg/tpeBPy46hf" target="_blank" rel="noopener noreferrer"><img alt="Liên hệ với tôi" src="https://img.shields.io/badge/Contact_Me-gray?style=flat&logo=Discord&logoColor=white&logoSize=auto&labelColor=cornflowerblue"></a>
<a href="https://bluemarble.lol/" target="_blank" rel="noopener noreferrer"><img alt="Trang web Blue Marble" src="https://img.shields.io/badge/Blue_Marble_Website-crqch-blue?style=flat&logo=globe&logoColor=white"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Thời gian lập trình" src="https://img.shields.io/badge/Coding_Time-212hrs_17mins-blue?style=flat&logo=wakatime&logoColor=black&logoSize=auto&labelColor=white"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Tổng số bản vá" src="https://img.shields.io/badge/Total_Patches-1231-black?style=flat"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Tổng số dòng mã" src="https://img.shields.io/badge/Lines_Of_Code-7540-blue?style=flat"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Tổng số dòng bình luận" src="https://img.shields.io/badge/Lines_Of_Comments-5918-blue?style=flat"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Tỷ lệ nén" src="https://img.shields.io/badge/Compression-72.57%25-blue"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Kích thước kho lưu trữ" src="https://img.shields.io/github/repo-size/SwingTheVine/Wplace-BlueMarble"></a>
<a href="https://hits.sh/github.com/SwingTheVine/Wplace-BlueMarble/" target="_blank" rel="noopener"><img alt="Lượt xem" src="https://hits.sh/github.com/SwingTheVine/Wplace-BlueMarble.svg?label=Views&extraCount=664359&color=ffffff"/></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Lượt tải xuống" src="https://img.shields.io/github/downloads/SwingTheVine/Wplace-BlueMarble/total.svg"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Xây dựng" src="https://github.com/SwingTheVine/Wplace-BlueMarble/actions/workflows/build.yml/badge.svg"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="Trang" src="https://github.com/SwingTheVine/Wplace-BlueMarble/actions/workflows/pages/pages-build-deployment/badge.svg?branch=wiki"></a>
<a href="" target="_blank" rel="noopener noreferrer"><img alt="CodeQL" src="https://github.com/SwingTheVine/Wplace-BlueMarble/actions/workflows/github-code-scanning/codeql/badge.svg"></a>
<a href="https://www.bestpractices.dev/projects/11067" target="_blank" rel="noopener noreferrer"><img alt="Thực hành tốt nhất OpenSSF" src="https://www.bestpractices.dev/projects/11067/badge"></a>
<h2 id="regarding-this-fork">Về fork này</h2>
<p>
  Đối với những người dùng không muốn mua ứng dụng TamperMonkey từ App Store, vốn là ứng dụng trả phí không giống như các nền tảng trình duyệt khác, ứng dụng Userscripts dường như là một lựa chọn thay thế miễn phí làm trình quản lý userscript.
</p>
<p>
  Tuy nhiên, GM API được Userscripts hỗ trợ ít hơn nhiều so với những gì TamperMonkey hỗ trợ, đặc biệt là đối với các API đồng bộ cũ mà Blue Marble sử dụng đã bị Greasemonkey loại bỏ trong Greasemonkey 4.0+ và phải được thay thế bằng các lựa chọn thay thế:
</p>

<ul>
  <li>GM_addStyle → GM.addStyle</li>
  <li>GM_getValue → GM.getValue</li>
  <li>GM_getResourceText → Đã thay thế (GM.getResourceText không tồn tại)</li>
</ul>

<p>
  Kiểm tra <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/tree/custom-improve">Nhánh Tùy chỉnh-Cải tiến</a> để biết các tính năng và cải tiến bổ sung được triển khai chưa có trong kho lưu trữ gốc:
</p>

<ul>
  <li>Hiển thị số lượng Charge bên ngoài nút có thể bị Cloudflare Turnstile che khuất. (v0.85.3)</li>
  <li>Hiển thị thời gian còn lại để đầy Charge. (v0.85.9)</li>
  <li>Hiển thị gợi ý bảng màu dưới dạng hình chữ thập thay vì dấu chấm để dễ nhìn hơn. (v0.85.2)</li>
  <li>(Có thể khôi phục về chế độ dấu chấm kể từ v0.85.46)</li>
  <li>(Do giới hạn kích thước Canvas của Safari trên thiết bị di động (4096x4096), mức thu phóng tối đa chỉ có thể là 4 thay vì 5)</li>
  <li>Ghi nhớ các ô đã tải để tránh độ trễ / tính toán dư thừa (bất cứ khi nào tiêu đề Last-Modified không thay đổi) (v0.85.4)</li>
  <li>Đã sửa lỗi chuyển đổi bảng màu không lưu trữ được. (v0.85.1)</li>
  <li>Đã sửa lỗi số lượng tổng số khối cần đếm là 1 hoặc 2 sau khi làm mới. (v0.85.2)</li>
  <li>Đã sửa lỗi các nút "Bật tất cả" và "Tắt tất cả" không lưu trữ được. (v0.85.13)</li>
  <li>Đã sửa lỗi chuyển đổi không gian màu trên Firefox. (v0.85.16)</li>
  <li>Hiển thị số lượng đã lấp đầy của từng màu. (v0.85.10)</li>
  <li>Dịch chuyển trực tiếp đến một trong các pixel chưa được lấp đầy khi nhấp vào khối màu chưa hoàn thành trong bộ lọc. (v0.85.10)</li>
  <li>Cho phép dịch chuyển đến tọa độ ô đã cho qua nút máy bay bên cạnh các hộp nhập liệu. (v0.85.9)</li>
  <li>Hiển thị cả tọa độ địa lý cùng với tọa độ ô. (v0.85.5)</li>
  <li>Tối ưu hóa vòng lặp for để phản hồi nhanh hơn. (v0.85.7)</li>
  <li>Cho phép sử dụng nhiều bản mẫu cùng một lúc. (v0.85.11)</li>
  <li>Nút để dịch chuyển đến góc trên cùng bên trái của bản mẫu đã chọn. (v0.85.12)</li>
  <li>Tùy chọn ẩn các màu bị khóa (màu chưa được mở khóa) khỏi danh sách màu. (v0.85.17)</li>
  <li>Cung cấp phiên bản bookmarklet. (v0.85.22)</li>
  <li>Cho phép ẩn các màu đã hoàn thành khỏi danh sách màu. (v0.85.23)</li>
  <li>Các tùy chọn khác nhau để thay đổi thứ tự hiển thị của các màu, bao gồm số lượng đã/chưa tô, sắc độ và độ sáng. (v0.85.23)
    <ul>
      <li>Đã thêm tùy chọn sắp xếp theo ID màu. (v0.87.16)</li>
    </ul>
  </li>
  <li>Thanh tiến trình phía sau mỗi màu trong danh sách hiển thị tiến độ tương đối (v0.85.24)</li>
  <li>Cho phép các định dạng tọa độ khác nhau (`a, b, c, d`, `a b c d` và `Tl X: a, Tl Y: b, Px X: c, Px Y: d`) được dán vào hộp văn bản tọa độ đầu tiên. (v0.85.28)</li>
  <li>Cho phép tải xuống tác phẩm nghệ thuật (theo đúng kích thước) từ bản đồ qua Nút Chia sẻ bằng hai tọa độ của các góc đối diện (Một từ các hộp văn bản, một từ pixel bạn chọn trên bản đồ trước khi nhấp vào nút "Chia sẻ") (v0.85.28)</li>
  <li>Chế độ Tiết kiệm bộ nhớ: Tạo ImageBitmap chỉ khi các bản mẫu được xử lý và giải phóng ngay sau đó để ngăn sử dụng hết tất cả bộ nhớ khả dụng. (v0.85.33)</li>
  <li>Cho phép đặt điểm neo cho tọa độ được chỉ định để đặt bản mẫu. (Theo mặc định, tọa độ là góc trên cùng bên trái của bản mẫu) (v0.85.34)</li>
  <li>Hỗ trợ hiển thị vị trí của các Vật phẩm Sự kiện. (Cần cung cấp nhà cung cấp dữ liệu JSON (ví dụ: <a href="https://wplace.samuelscheit.com/tiles/pumpkin.json">Wplace Archive pumpkin.json</a>) để tính năng này hoạt động) (v0.85.35)</li>
  <li>Cho phép chỉ hiển thị các pixel của màu hiện được chọn trong Wplace một cách tự động. (v0.85.37)</li>
  <li>Cố gắng làm mới các ô khi màu đã chọn / bản mẫu thay đổi càng sớm càng tốt. (v0.85.38)</li>
  <li>Cố gắng làm mới các ô sau khi gửi pixel càng sớm càng tốt. (v0.85.39)</li>
  <li>Chuyển đổi giữa các chủ đề tích hợp sẵn của Wplace. (v0.85.40)</li>
  <li>Kiểm tra tính năng bản đồ lỗi (Đỏ: Sai, Vàng: Chưa lấp đầy, Xanh lá: Đúng). (v0.85.46)</li>
  <li>Tách lớp phủ và lớp lỗi khỏi lớp tác phẩm nghệ thuật. (v0.86.1)</li>
  <li>Lớp phủ không còn đợi fetch để cập nhật. (v0.86.1)</li>
  <li>Cho phép đổi tên bản mẫu bằng cách nhấp vào tên bản mẫu. (v0.86.1)</li>
  <li>
  Cho phép cuộn bản đồ theo đường chéo mượt mà qua bàn phím bằng các phím mũi tên (<kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd>). (v0.86.5)
    <ul>
      <li>Được triển khai bởi <a href="https://github.com/due2e">@due2e</a> theo <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/pull/7">PR #7</a>.</li>
      <li>Lưu ý rằng wplace có các phím tắt mặc định cho việc xoay theo trục qua <kbd>↑</kbd> <kbd>←</kbd> <kbd>↓</kbd> <kbd>→</kbd> (và xoay / nghiêng với phím <kbd>Shift</kbd> kết hợp)</li>
    </ul>
  </li>
  <li>Hiển thị thời gian đếm ngược tạm ngưng và lý do nếu có. (v0.86.6)</li>
  <li>Hiển thị các nút tỷ lệ thu phóng bổ sung để cho phép ảnh chụp màn hình có cùng kích thước pixel chính xác cho mỗi pixel được vẽ hoặc mức thu phóng tối thiểu có thể trước khi tác phẩm nghệ thuật biến mất (Giải quyết <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/issues/8">#8</a>). (v0.86.10)
    <ul>
      <li>Được mở rộng bởi <a href="https://github.com/Commenter25">@Commenter25</a> theo <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/pull/13">PR #13</a>. (v0.86.15)</li>
    </ul>
  </li>
  <li>Cho phép tạo bản mẫu đường thẳng / hình tròn của màu hiện được chọn bằng cách chọn hai tọa độ của các góc đối diện (Một từ các hộp văn bản, một từ pixel bạn chọn trên bản đồ trước khi nhấp vào nút "Chia sẻ") (v0.86.13)
    <ul>
      <li>Đối với hình tròn, tọa độ hộp văn bản đề cập đến tâm và điểm hiện được chọn đề cập đến một điểm trên hình tròn xác định bán kính. (v0.86.16)</li>
    </ul>
  </li>
  <li>Thêm tùy chọn để chỉ cho phép các màu hiện đang được bật được bao gồm trong bản đồ lỗi. (Giải quyết <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/issues/11">#11</a>). (v0.86.14)</li>
  <li>Sửa một số vấn đề về ranh giới từ thượng nguồn Blue Marble và Wplace. (v0.86.16)
    <ul>
      <li>Blue Marble: Tạo bản mẫu vượt qua ranh giới Tl X: 2047 - 0 không hiển thị từ Ô X = 0.</li>
      <li>Blue Marble: (Tl X, Tl Y, Px X, Px Y) không cập nhật khi chọn pixel từ Ô X = 2047 trong khi Trung tâm Bản đồ ở Ô X = 0.</li>
      <li>Blue Marble & Wplace: Nút Pin sao chép (Tl X, Tl Y, Px X, Px Y) bị lỗi từ yêu cầu thông tin pixel (tức là Tl X và Px X bị âm) khi chọn pixel từ Ô X = 2047 trong khi Trung tâm Bản đồ ở Ô X = 0.</li>
      <li>Wplace: Thông tin Pixel không hiển thị khi chọn pixel từ Ô X = 0 trong khi Trung tâm Bản đồ ở Ô X = 2047.</li>
    </ul>
  </li>
  <li>Cho phép bản mẫu không tạo lớp phủ trên bản đồ để tiết kiệm thời gian xử lý. Hữu ích khi được sử dụng cùng với tính năng lớp phủ chính thức hoặc các công cụ lớp phủ khác. (v0.87.15)
    <ul>
      <li>Lưu ý rằng trong trường hợp này, các màu hiển thị trên lớp phủ được quản lý bởi công cụ lớp phủ bên ngoài, không phải tập lệnh này.</li>
    </ul>
  </li>
</ul>

<h2 id="quick-guide">Hướng dẫn nhanh</h2>
<p>
  Nhấn các mũi tên để hiển thị tùy chọn bạn muốn.
  <details>
    <summary>
      <b>Tôi muốn tải Blue Marble.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="#installation-instructions">Nhấp vào đây</a> để xem hướng dẫn cài đặt.
  </details>
  <details>
    <summary>
      <b>Tôi muốn đặt câu hỏi về Blue Marble.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="https://discord.gg/tpeBPy46hf" target="_blank" rel="noopener noreferrer">Nhấp vào đây</a> để nhận lời mời tham gia máy chủ Discord của máy chủ hỗ trợ Blue Marble.
    <br>
    <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/discussions/categories/q-a">Nhấp vào đây</a> để đến trang trợ giúp và câu hỏi GitHub của Blue Marble.
  </details>
  <details>
    <summary>
      <b>Tôi muốn báo lỗi.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/issues/new/choose">Nhấp vào đây</a> để báo lỗi, sau đó chọn tùy chọn "Bug Report".
  </details>
  <details>
    <summary>
      <b>Tôi muốn đề xuất tính năng.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/issues/new/choose">Nhấp vào đây</a> để đề xuất tính năng, sau đó chọn tùy chọn "Feature Request".
  </details>
  <details>
    <summary>
      <b>Tôi muốn đóng góp.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/CONTRIBUTING.md">Nhấp vào đây</a> để đọc các hướng dẫn đóng góp.
  </details>
  <details>
    <summary>
      <b>Tôi muốn báo cáo lỗ hổng.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/security">Nhấp vào đây</a> để gửi báo cáo lỗ hổng.
  </details>
  <details>
    <summary>
      <b>Tôi muốn truy cập trang web.</b> <sup>(Nhấp để mở rộng)</sup>
    </summary>
    <a href="https://bluemarble.camilledaguin.fr/" target="_blank" rel="noopener noreferrer">Nhấp vào đây</a> để truy cập trang web chính thức của Blue Marble.
  </details>
</p>

<h2 id="overview">Tổng quan</h2>
<p>
  Chào mừng bạn đến với Blue Marble! Blue Marble là một userscript cho trang web <a href="https://wplace.live/" target="_blank" rel="noopener noreferrer">wplace.live</a>. Mục đích của Blue Marble là cho phép bạn lấy một hình ảnh và xếp lớp nó lên canvas! Bằng cách đó, bạn có thể dễ dàng phác thảo hình ảnh tác phẩm nghệ thuật của mình mà không cần phải nhìn qua lại giữa nhiều tab/màn hình. Ngoài ra, Blue Marble hỗ trợ một số tính năng bổ sung tiện lợi như:
  <ul>
    <li>Hiển thị số pixel bạn cần để lên cấp</li>
    <li>Hiển thị hệ tọa độ đơn giản (tọa độ ô và tọa độ pixel)</li>
    <li>Cho phép bạn di chuyển bảng màu lên đầu màn hình khi đặt pixel</li>
    <li>Cho phép bạn sử dụng ống nhỏ giọt màu trên hình ảnh bản mẫu, miễn là màu sắc chính xác</li>
    <li>...và hơn thế nữa!</li>
  </ul>
  Nếu bạn thích userscript này, hãy ⭐ kho lưu trữ! Để biết thêm thông tin và cập nhật, hãy truy cập <a href="https://bluemarble.camilledaguin.fr/" target="_blank" rel="noopener noreferrer">trang web Blue Marble</a>. Nếu bạn muốn đóng góp cho Blue Marble, hãy xem tệp <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/CONTRIBUTING.md" target="_blank" rel="noopener noreferrer">CONTRIBUTING.md</a> trong <code>docs/</code>.

  <img alt="Hình ảnh giới thiệu bản mẫu Blue Marble" src="./assets/Showcase1.png">

  <h3 id="installation-instructions">Hướng dẫn cài đặt</h3>
  <a href="" target="_blank" rel="noopener noreferrer"><img alt="Trình duyệt được hỗ trợ" src="https://img.shields.io/badge/Supported%20Browsers-Chrome%20%7C%20Firefox%2A%20%7C%20Safari%20%7C%20Edge%20%7C%20Brave-orange?style=flat"></a>
  <a href="" target="_blank" rel="noopener noreferrer"><img alt="Trình duyệt không được hỗ trợ" src="https://img.shields.io/badge/Unsupported%20Browsers-Firefox%2A%20%7C%20Kiwi%20%7C%20Vivaldi-red?style=flat"></a>
  <p>
    Blue Marble đã được xác minh hoạt động trên thiết bị di động. Blue Marble được thiết kế trên Chrome, nhưng Blue Marble có thể hoạt động trên các trình duyệt "không được hỗ trợ" không được liệt kê ở trên. Một số phiên bản/nhánh của Firefox hoạt động. Một số phiên bản/nhánh của Firefox không hoạt động.
    <br>
    Hướng dẫn cài đặt cho Blue Marble ở bên dưới. Nhấp vào mũi tên để mở rộng hướng dẫn bạn muốn xem. Văn bản màu xanh là liên kết.
    <details>
      <summary>
        <b>Cài đặt trên Chrome</b> <sup>(Nhấp để mở rộng)</sup>
      </summary>
      <a href="https://www.youtube.com/watch?v=gg5oiJcftEc" target="_blank" rel="noopener noreferrer"><img alt="Hướng dẫn cài đặt" src="https://img.shields.io/badge/Install_Tutorial-gray?style=flat&logo=YouTube&logoColor=white&logoSize=auto&labelColor=darkred"></a>
      <ol>
        <li>Cài đặt tiện ích mở rộng <a href="https://chromewebstore.google.com/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo" target="_blank" rel="noopener noreferrer">TamperMonkey</a> cho Chrome.
        <br>
        <img alt="Nhấp vào nút 'Add extension'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerChromeInstall1.png"></li>
        <li>Nhấp chuột phải vào tiện ích mở rộng.
        <br>
        <img alt="Truy cập menu 'Manage Extension'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerChromeInstall2.png"></li>
        <li>Nhấp chuột trái vào "Manage Extension".</li>
        <li>Bật "Developer Mode".
        <br>
        <img alt="Bật 'Developer Mode' và 'Allow user scripts'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerChromeInstall3.png"></li>
        <li>Bật "Allow user scripts".</li>
        <li><strong>Cài đặt một lần:</strong> Nhấp vào liên kết này để cài đặt Blue Marble trực tiếp: <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/releases/download/pre/BlueMarble.user.js" target="_blank" rel="noopener noreferrer"><strong>Cài đặt Blue Marble</strong></a>
        <br>
        TamperMonkey sẽ tự động phát hiện userscript và nhắc bạn cài đặt nó.</li>
        <li>Làm mới trang web <a href="https://wplace.live/" target="_blank" rel="noopener noreferrer">wplace.live</a>.</li>
      </ol>
    </details>
    <details>
      <summary>
        <b>Cài đặt trên Microsoft Edge</b> <sup>(Nhấp để mở rộng)</sup>
      </summary>
      <ol>
        <li>Cài đặt tiện ích bổ sung <a href="https://microsoftedge.microsoft.com/addons/detail/iikmkjmpaadaobahmlepeloendndfphd" target="_blank" rel="noopener noreferrer">TamperMonkey</a> cho Microsoft Edge.
        <br>
        <img alt="Nhấp vào nút 'Get'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerEdgeInstall1.png"></li>
        <li>Nhấp chuột phải vào tiện ích mở rộng.
        <br>
        <img alt="Truy cập menu 'Manage Extension'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerEdgeInstall2.png"></li>
        <li>Nhấp chuột trái vào "Manage Extension".</li>
        <li>Bật "Developer Mode".
        <br>
        <img alt="Bật 'Developer Mode'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerEdgeInstall3.png"></li>
        <li>Tải xuống tệp <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/releases" target="_blank" rel="noopener noreferrer">BlueMarble.user.js</a> trong "Assets" của bản phát hành mới nhất.</li>
        <li>Mở Bảng điều khiển TamperMonkey.
        <br>
        <img alt="Truy cập 'Dashboard' của TamperMonkey" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerEdgeInstall4.png"></li>
        <li>Kéo tệp <code>BlueMarble.user.js</code> vào bên trong bảng điều khiển của TamperMonkey.
        <br>
        <img alt="Kéo userscript vào bảng điều khiển" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerChromeInstall5.png"></li>
        <li>Nhấp vào nút "Install" để cài đặt Blue Marble.
        <br>
        <img alt="Nhấp vào nút 'Install'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerChromeInstall6.png"></li>
        <li>Bật Blue Marble trong bảng điều khiển TamperMonkey.
        <br>
        <img alt="Bật Blue Marble" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerChromeInstall7.png"></li>
        <li>Làm mới trang web <a href="https://wplace.live/" target="_blank" rel="noopener noreferrer">wplace.live</a>.</li>
      </ol>
    </details>
    <details>
      <summary>
        <b>Cài đặt trên Firefox</b> <sup>(Nhấp để mở rộng)</sup>
      </summary>
      <ol>
        <li>Cài đặt tiện ích bổ sung <a href="https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/" target="_blank" rel="noopener noreferrer">TamperMonkey</a> cho Firefox.
        <br>
        <img alt="Nhấp vào nút 'Add to Firefox'" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/ComputerFireFoxInstall1.png"></li>
        <li><strong>Cài đặt một lần:</strong> Nhấp vào liên kết này để cài đặt Blue Marble trực tiếp: <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/releases/download/pre/BlueMarble.user.js" target="_blank" rel="noopener noreferrer"><strong>Cài đặt Blue Marble</strong></a>
        <br>
        TamperMonkey sẽ tự động phát hiện userscript và nhắc bạn cài đặt nó.</li>
        <li>Làm mới trang web <a href="https://wplace.live/" target="_blank" rel="noopener noreferrer">wplace.live</a>.</li>
      </ol>
    </details>
    <details>
      <summary>
        <b>Cài đặt trên Safari bằng Userscripts thay vì TamperMonkey</b> <sup>(Nhấp để mở rộng)</sup>
      </summary>
      <ol>
        <li>Cài đặt ứng dụng <a href="https://apps.apple.com/us/app/userscripts/id1463298887" target="_blank" rel="noopener noreferrer">Userscripts</a> từ App Store.
        <br>
        Đảm bảo rằng các quyền thích hợp đã được cấp cho ứng dụng và Safari được cấu hình để bật tiện ích mở rộng.</li>
        <br>
        <li>Tải xuống tập lệnh Blue Marble và lưu vào Vị trí Lưu theo quy định của ứng dụng: <a href="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/releases/download/pre/BlueMarble.user.js" target="_blank" rel="noopener noreferrer"><strong>Tải xuống Blue Marble</strong></a>
        <br>
        Userscripts sẽ tự động phát hiện userscript.</li>
        <li>Làm mới trang web <a href="https://wplace.live/" target="_blank" rel="noopener noreferrer">wplace.live</a>.</li>
        <li>Các vấn đề liên quan đến Cài đặt và Sử dụng Userscripts nên tham khảo: <a href="https://github.com/quoid/userscripts/" target="_blank" rel="noopener noreferrer"><strong>Kho lưu trữ của Userscripts</strong></a> thay vào đó.</li>
      </ol>
    </details>
  </p>

  <h3 id="script-settings">Cài đặt tập lệnh</h3>
  <p>
    Có nhiều cài đặt có sẵn cho userscript Blue Marble! Thông qua các cài đặt này, bạn có thể kiểm soát cách tập lệnh hoạt động.
  </p>

  <h3 id="template-settings">Cài đặt bản mẫu</h3>
  <p>
    <h4>Pixel trong suốt</h4>
    <p>
      Bản mẫu cho Blue Marble hoạt động hơi khác so với bình thường. Vì có màu "Trong suốt" và các pixel trong suốt trong bản mẫu thường bị bỏ qua, bản mẫu của bạn nên có một màu tùy chỉnh để biểu thị các pixel có màu "Trong suốt".
      <ul>
        <li>Nếu bạn muốn một pixel cụ thể có bất kỳ màu nào, nó sẽ trong suốt trong bản mẫu của bạn.</li>
        <li>Nếu bạn muốn một pixel cụ thể là màu "Trong suốt" trên bảng màu Wplace, nó phải có mã màu hex <code>#deface</code>.</li>
      </ul>
    </p>
    <h4>Tọa độ</h4>
    <p>
      <h5>Tọa độ ô</h5>
      <p>
        Hệ tọa độ cho wplace.live rất độc đáo. Thay vì tất cả pixel có một số tọa độ toàn cầu (x, y), số tọa độ tương đối với ô. Điều này có nghĩa là bạn cần biết số ô và số tọa độ để làm bất cứ điều gì. Trong Blue Marble, tọa độ ô và tọa độ pixel được hiển thị khi bạn nhấp vào một pixel. Đây là những tọa độ bạn nên sử dụng để căn chỉnh một bản mẫu.
        <br>
        <img alt="Nơi tìm tọa độ ô" src="https://github.com/CheemsGalaxy/BlueMarble-Userscripts-Vietsub/blob/main/docs/assets/TemplateCoordinatesDisplay.png">
      </p>
      <h5>Tọa độ bản mẫu</h5>
      <p>
        Bản mẫu được căn chỉnh từ góc trên cùng bên trái của bản mẫu. Bạn có thể tự động điền vị trí này bằng biểu tượng "pin" (còn gọi là "waypoint") bên cạnh các hộp nhập tọa độ.
      </p>
    </p>
  </p>
</p>

<h2 id="how-versioning-works">Cách thức hoạt động của phiên bản</h2>
<p>
  Hệ thống phiên bản cho userscript này tuân theo <a href="https://semver.org/" target="_blank" rel="noopener noreferrer">các quy tắc Phiên bản Ngữ nghĩa</a>. Do đó, nó được định dạng theo định dạng <code>X.Y.Z</code> trong đó:
  <ul>
    <li>X là phiên bản chính. Điều này được tăng lên khi một bản cập nhật không tương thích ngược được đẩy lên. Điều này dành cho các tính năng mới phá vỡ các phiên bản trước của userscript. Ngoài ra, nếu wplace.live phá vỡ userscript, điều này sẽ được tăng lên.</li>
    <li>Y là phiên bản phụ. Điều này được tăng lên bất cứ khi nào tôi đẩy lên GitHub. Điều này dành cho các bản sửa lỗi ổn định và các tính năng mới (không phá vỡ).</li>
    <li>Z là phiên bản vá. Điều này được tăng lên bất cứ khi nào tôi khởi chạy phiên bản phát triển của userscript để kiểm tra một bản vá. Điều này dành cho các bản sửa lỗi/tính năng không ổn định.</li>
  </ul>
</p>

<h2 id="licenses">Giấy phép</h2>
<p>
  (Dưới đây, tất cả đề cập đến "userscript" đề cập đến userscript "Blue Marble" được tạo bởi SwingTheVine) <br>
  Hầu hết userscript này được cấp phép theo <code>Mozilla Public License Version 2.0</code> (MPL-2.0). Tất cả phần mềm, mã nguồn và thư viện trong kho lưu trữ này được cấp phép theo giấy phép MPL-2.0. Tuy nhiên, hình ảnh "Blue Marble" trong userscript này thuộc sở hữu của NASA và được cấp phép theo giấy phép <code>Creative Commons 0 1.0 Universal</code> (CC0 1.0).
</p>

<h2 id="faq">Câu hỏi thường gặp</h2>
<p>
  <h3 id="is-blue-marble-malware">Blue Marble có phải là phần mềm độc hại không?</h3>
  <p><b>Trả lời:</b> Blue Marble không chứa mã độc hại. Mã nguồn Blue Marble có thể được tìm thấy trong thư mục <code>src/</code>. Nếu bạn lo lắng Blue Marble là phần mềm độc hại, bạn có thể đọc mã, sau đó tự đóng gói nó bằng các công cụ trong <code>build/</code>.</p>

  <h3 id="how-can-blue-marble-place-pixels-for-me">Blue Marble có thể đặt pixel cho tôi bằng cách nào?</h3>
  <p><b>Trả lời:</b> Rất tiếc, Blue Marble sẽ không hỗ trợ việc tự động đặt pixel mà không có tương tác của người dùng vì điều đó không được Wplace cho phép.</p>

  <h3 id="how-do-i-hide-the-overlay">Làm thế nào để ẩn lớp phủ?</h3>
  <p><b>Trả lời:</b> Tắt userscript và làm mới trang.</p>

  <h3 id="why-do-game-notifications-appear-on-top-of-the-overlay">Tại sao thông báo trò chơi xuất hiện trên lớp phủ?</h3>
  <p><b>Trả lời:</b> Thông báo trò chơi chỉ xuất hiện khi chúng cần được chú ý ngay lập tức. Do đó, chúng được ưu tiên hơn lớp phủ (thường không cần chú ý).</p>
</p>
