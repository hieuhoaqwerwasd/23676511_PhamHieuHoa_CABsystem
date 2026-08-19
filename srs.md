## Bước 1 — Business Context & Business Problem 

### 1. Business Context

Câu 1: xác định business context và business problem

1. Business Context
ABC đang có nhu cầu chuyển đổi hoạt động đặt xe sang một nền tảng số có khả năng kết nối trực tiếp giữa khách hàng – tài xế – bộ phận vận hành. Hệ thống CAB sẽ đóng vai trò là nền tảng quản lý tập trung, hỗ trợ xuyên suốt từ lúc khách hàng tạo yêu cầu đến khi chuyến xe kết thúc, thanh toán và đánh giá.

Ngoài các nhóm người dùng chính, CAB còn cần kết nối với một số dịch vụ bên ngoài như bản đồ/vị trí, cổng thanh toán và các nhà cung cấp thông báo. Điều này giúp hệ thống không phải tự xây dựng tất cả thành phần mà vẫn có thể cung cấp đầy đủ dịch vụ cho người dùng.

Về định hướng kinh doanh, ABC mong muốn giảm sự phụ thuộc vào điều phối thủ công, rút ngắn thời gian xử lý yêu cầu đặt xe, sử dụng tài xế hiệu quả hơn và cung cấp cho khách hàng thông tin rõ ràng về tình trạng chuyến đi. Đồng thời, nền tảng cần được thiết kế với khả năng mở rộng để ABC có thể phát triển thêm dịch vụ trong tương lai.

Một số chính sách nghiệp vụ hiện vẫn chưa được xác định cụ thể, chẳng hạn như cách tính giá, nguyên tắc lựa chọn tài xế, thời gian chờ phản hồi, chính sách hủy, xử lý thanh toán thất bại và thời gian lưu trữ dữ liệu. Đây là những nội dung BA cần làm rõ với các stakeholder trước khi chốt giải pháp.

### 2. Business Problem
Vấn đề chính của ABC không chỉ nằm ở việc thiếu một ứng dụng đặt xe mới, mà là quy trình vận hành hiện tại chưa được số hóa và liên kết thành một luồng thống nhất.

Việc phân tài xế còn phụ thuộc vào nhân viên vận hành khiến khả năng xử lý nhiều yêu cầu cùng lúc bị hạn chế. Khách hàng cũng chưa có đủ thông tin để chủ động theo dõi chuyến xe, trong khi dữ liệu về chuyến đi, thanh toán và hoạt động của tài xế chưa được quản lý tập trung. Khi xảy ra các tình huống bất thường, nhân viên vận hành phải mất nhiều thời gian để kiểm tra và xử lý.

Bên cạnh đó, hệ thống hiện tại chưa tạo được nền tảng tốt cho việc mở rộng quy mô. Khi số lượng khách hàng, tài xế hoặc chuyến xe tăng lên, các quy trình thủ công có thể trở thành điểm nghẽn. Việc bổ sung phương thức thanh toán, dịch vụ mới hoặc kênh thông báo mới cũng có nguy cơ ảnh hưởng đến các chức năng đang hoạt động.

Vì vậy, ABC cần giải quyết bài toán ở cấp độ nền tảng, thay vì chỉ xây dựng một ứng dụng đặt xe. CAB cần giúp doanh nghiệp tự động hóa các hoạt động cốt lõi, tăng khả năng quan sát và kiểm soát vận hành, đồng thời tạo một kiến trúc đủ linh hoạt để tiếp tục phát triển trong những giai đoạn sau.

## Bước 2 — Stakeholder 

# Stakeholder

Stakeholder của dự án CAB được phân loại dựa trên vai trò, mức độ ảnh hưởng đến dự án và mức độ tham gia vào quá trình xây dựng hệ thống.

## 1. Project & Business Stakeholders

- Ban Giám đốc / Project Sponsor
- Finance / Accounting

## 2. Operational Stakeholders

- Operation Staff
- Customer Support
- Admin

## 3. Primary Users

- Customer
- Driver

## 4. Technology & Governance Stakeholders

- IT / Technical Team
- Security / Compliance

## 5. External Partners

- Payment Provider
- Notification Provider
- Map / Location Provider
- Other External Service Providers

---

## Stakeholder Matrix

| Stakeholder | Influence | Interest | Priority | Engagement |
|---|---|---|---|---|
| Ban Giám đốc / Project Sponsor | Cao | Cao | P1 | Tham gia quyết định và review các vấn đề quan trọng |
| Operation Staff | Cao | Cao | P1 | Tham gia phân tích và xác nhận quy trình nghiệp vụ |
| IT / Technical Team | Cao | Cao | P1 | Phối hợp về giải pháp, tích hợp và giới hạn kỹ thuật |
| Security / Compliance | Cao | Cao | P1 | Xác nhận yêu cầu về bảo mật, quyền truy cập và dữ liệu |
| Customer | Thấp | Cao | P1 | Thu thập nhu cầu và phản hồi về trải nghiệm |
| Driver | Trung bình | Cao | P1 | Xác nhận quy trình nhận và thực hiện chuyến |
| Finance / Accounting | Cao | Trung bình | P2 | Tham vấn về tính cước, thanh toán và đối soát |
| Customer Support | Trung bình | Cao | P2 | Xác nhận quy trình hỗ trợ và xử lý ngoại lệ |
| Admin | Trung bình | Trung bình | P2 | Xác nhận chức năng quản trị và phân quyền |
| Payment Provider | Trung bình | Trung bình | P2 | Phối hợp về tích hợp thanh toán và xử lý lỗi |
| Map / Location Provider | Trung bình | Trung bình | P2 | Phối hợp về bản đồ và dữ liệu vị trí |
| Notification Provider | Thấp | Trung bình | P3 | Theo dõi và phối hợp khi có vấn đề tích hợp |
| Other External Service Providers | Thấp | Thấp | P3 | Theo dõi dependency và phối hợp khi cần |

---

## Influence–Interest Matrix

| | Interest thấp | Interest cao |
|---|---|---|
| Influence cao | Finance / Accounting | Ban Giám đốc / Project Sponsor<br>Operation Staff<br>IT / Technical Team<br>Security / Compliance |
| Influence thấp | Admin<br>Notification Provider<br>Other External Service Providers | Customer<br>Driver<br>Customer Support<br>Map / Location Provider |

---

## Stakeholder Engagement Strategy

- **Influence cao – Interest cao:** Làm việc thường xuyên, tham gia workshop, review requirement và đưa ra quyết định khi cần.
- **Influence cao – Interest thấp:** Cập nhật những vấn đề có ảnh hưởng trực tiếp đến phạm vi hoặc hoạt động của stakeholder.
- **Influence thấp – Interest cao:** Chủ động thu thập nhu cầu, phản hồi và thông tin từ người sử dụng hệ thống.
- **Influence thấp – Interest thấp:** Theo dõi ở mức phù hợp và phối hợp khi phát sinh vấn đề liên quan.
  

## Bước 3 — Business Goal 

| Mã | Business Goal | Mô tả |
|---|---|---|
| **BG1** | **Chuyển đổi quy trình đặt xe sang môi trường số** | Đưa các hoạt động từ tiếp nhận yêu cầu, lựa chọn xe, tìm tài xế đến hoàn tất chuyến lên một nền tảng thống nhất, qua đó giảm sự phụ thuộc vào tổng đài và các thao tác điều phối thủ công. |
| **BG2** | **Nâng cao hiệu quả kết nối khách hàng và tài xế** | Rút ngắn thời gian tìm kiếm tài xế và tăng khả năng phục vụ yêu cầu đặt xe bằng cách lựa chọn tài xế dựa trên vị trí, trạng thái hoạt động và các điều kiện vận hành phù hợp. |
| **BG3** | **Mang lại trải nghiệm dịch vụ minh bạch và thuận tiện** | Giúp khách hàng chủ động nắm được tình trạng yêu cầu và chuyến đi, thông tin tài xế, chi phí phải trả và kết quả thanh toán; đồng thời tạo điều kiện để tài xế tiếp nhận và cập nhật chuyến một cách thuận tiện. |
| **BG4** | **Tăng cường khả năng quản lý hoạt động kinh doanh** | Tập trung dữ liệu về khách hàng, tài xế, phương tiện, chuyến xe và giao dịch trên một hệ thống, giúp bộ phận vận hành dễ dàng giám sát, xử lý tình huống bất thường và hỗ trợ ban lãnh đạo theo dõi hiệu quả kinh doanh. |
| **BG5** | **Đảm bảo hoạt động ổn định khi nhu cầu tăng** | Xây dựng hệ thống có khả năng đáp ứng sự gia tăng về số lượng người dùng và chuyến xe, đồng thời hạn chế việc sự cố tại một chức năng như thanh toán hoặc thông báo ảnh hưởng đến hoạt động đặt xe. |
| **BG6** | **Tạo tiền đề cho việc mở rộng dịch vụ** | Xây dựng nền tảng đủ linh hoạt để ABC có thể bổ sung loại hình dịch vụ, phương thức thanh toán, nhà cung cấp bên ngoài hoặc các tính năng mới mà không phải thay đổi toàn bộ hệ thống hiện có. |
| **BG7** | **Tăng cường bảo vệ thông tin và kiểm soát hoạt động** | Đảm bảo thông tin khách hàng, tài xế, phương tiện, vị trí và giao dịch được bảo vệ phù hợp; đồng thời kiểm soát quyền thực hiện các chức năng quản trị và lưu lại các hoạt động quan trọng để phục vụ kiểm tra khi cần. |
| **BG8** | **Hỗ trợ doanh nghiệp ra quyết định dựa trên dữ liệu** | Cung cấp thông tin và báo cáo về tình hình đặt xe, doanh thu, tỷ lệ hoàn thành hoặc hủy chuyến và hiệu quả hoạt động của tài xế, giúp doanh nghiệp đánh giá tình hình và đưa ra quyết định phù hợp. |

## Bước 4 — Project Scope
### 4.1 In-Scope (MVP)

#### A. Customer Management

- Tạo tài khoản và đăng nhập hệ thống
- Quản lý các thông tin cá nhân cần thiết
- Cung cấp thông tin điểm đón, điểm trả và nhu cầu về loại xe
- Khởi tạo và gửi yêu cầu chuyến đi
- Kiểm tra tình trạng chuyến trong từng giai đoạn
- Xem lại các chuyến đã thực hiện và chi phí tương ứng
- Gửi đánh giá cơ bản đối với tài xế sau khi chuyến kết thúc

#### B. Driver Management

- Tạo tài khoản tài xế thông qua đăng ký hoặc bởi nhân viên vận hành
- Quản lý thông tin cá nhân và phương tiện
- Thiết lập trạng thái hoạt động khi muốn nhận chuyến
- Tiếp nhận yêu cầu chuyến và lựa chọn nhận hoặc bỏ qua
- Cập nhật tiến trình thực hiện chuyến theo từng trạng thái
- Cung cấp thông tin vị trí phục vụ hoạt động điều phối tài xế

#### C. Trip & Driver Assignment

- Tiếp nhận yêu cầu và xác định nhóm tài xế có khả năng phục vụ
- Ưu tiên tài xế dựa trên vị trí và trạng thái hiện tại
- Chuyển yêu cầu sang tài xế khác khi tài xế được đề xuất không phản hồi hoặc từ chối
- Cập nhật kết quả tìm tài xế cho khách hàng
- Kết thúc quy trình tìm kiếm khi không còn tài xế phù hợp

#### D. Fare & Payment

- Xác định chi phí chuyến dựa trên loại dịch vụ và thông tin chuyến đi
- Hỗ trợ thanh toán trực tiếp bằng tiền mặt
- Kết nối với một đơn vị thanh toán bên ngoài cho giao dịch điện tử
- Không lưu thông tin nhạy cảm của thẻ hoặc tài khoản thanh toán tại CAB
- Ghi nhận kết quả giao dịch và thông báo cho khách hàng
- Cho phép thực hiện lại giao dịch thất bại theo chính sách được xác định

#### E. Notification

- Gửi thông tin đến khách hàng khi yêu cầu được tiếp nhận, tài xế được phân công, tài xế đến điểm đón, chuyến hoàn tất và thanh toán có kết quả
- Gửi thông báo cho tài xế khi có yêu cầu mới hoặc có thay đổi liên quan đến chuyến
- MVP triển khai một phương thức thông báo chính
- Thiết kế cơ chế tích hợp để có thể bổ sung thêm các phương thức khác trong tương lai

#### F. Operation & Administration

- Theo dõi các chuyến đang hoạt động
- Kiểm tra tình trạng và thông tin cơ bản của tài xế
- Tra cứu thông tin chuyến và giao dịch
- Hỗ trợ nhân viên xử lý thủ công các trường hợp chuyến gặp sự cố
- Phân biệt quyền hạn giữa Admin và nhân viên vận hành
- Quản lý các đối tượng chính như khách hàng, tài xế và phương tiện trong phạm vi MVP

#### G. Security & System Reliability

- Xác thực người dùng trước khi truy cập các chức năng yêu cầu tài khoản
- Giới hạn chức năng quản trị dựa trên quyền được cấp
- Ghi nhận các hoạt động quan trọng để phục vụ kiểm tra khi có sự cố
- Tách biệt các thành phần tích hợp để sự cố của payment hoặc notification không làm gián đoạn toàn bộ quy trình đặt xe

---

### 4.2 Out-of-Scope

Các nội dung sau chưa được đưa vào phiên bản MVP và có thể xem xét ở các giai đoạn tiếp theo:

- Hệ thống báo cáo chuyên sâu và dashboard phân tích kinh doanh
- Hỗ trợ đồng thời nhiều phương thức thanh toán điện tử
- Lưu sẵn nhiều phương thức thanh toán của khách hàng
- Triển khai nhiều kênh notification cùng lúc
- Cơ chế matching tài xế sử dụng AI/ML hoặc các thuật toán tối ưu nâng cao
- Dynamic pricing hoặc surge pricing
- Các dịch vụ ngoài đặt xe thông thường như giao hàng, xe ghép hoặc đặt xe theo lịch
- Hệ thống loyalty, voucher, khuyến mãi và chương trình khách hàng thân thiết
- Theo dõi vị trí nâng cao và cơ chế dự đoán ETA có độ chính xác cao
- Quy trình hủy chuyến phức tạp và cơ chế tính phí phạt tự động
- Kết nối đồng thời với nhiều Payment Provider
- Kết nối đồng thời với nhiều Notification Provider
- Kết nối đồng thời với nhiều Map / Location Provider
- Hệ thống BI và phân tích hiệu suất tài xế chuyên sâu
- Các tính năng tự động hóa vận hành nâng cao chưa cần thiết cho MVP

## Bước 5 — Business Requirement
## Business Requirement

> **Business Requirement** xác định những khả năng mà doanh nghiệp mong muốn hệ thống cung cấp để đáp ứng mục tiêu kinh doanh. Các yêu cầu được mô tả ở mức nghiệp vụ, chưa đi vào thiết kế giao diện hoặc chi tiết xử lý kỹ thuật.

| Mã | Business Requirement | Liên kết Business Goal | Nhóm |
|---|---|---|---|
| BR-01 | Khách hàng có thể chủ động tạo tài khoản và gửi yêu cầu đặt xe trực tiếp trên CAB mà không cần liên hệ với tổng đài | BG1 | Booking |
| BR-02 | CAB có khả năng tự xác định và lựa chọn tài xế đáp ứng điều kiện phục vụ dựa trên vị trí và trạng thái hoạt động | BG2 | Driver Matching |
| BR-03 | Khi tài xế được lựa chọn không tiếp nhận yêu cầu trong thời gian quy định hoặc từ chối chuyến, hệ thống tiếp tục tìm phương án thay thế mà không yêu cầu khách hàng đặt lại | BG2 | Driver Matching |
| BR-04 | Khách hàng có thể biết được tiến trình của chuyến xe từ lúc tạo yêu cầu cho đến khi chuyến kết thúc | BG3 | Trip Tracking |
| BR-05 | CAB xác định số tiền cần thanh toán dựa trên thông tin dịch vụ và dữ liệu thực tế của chuyến đi | BG5 | Fare |
| BR-06 | Hệ thống hỗ trợ thanh toán trực tiếp và thanh toán thông qua ít nhất một đối tác thanh toán điện tử | BG5 | Payment |
| BR-07 | Thông tin xác thực thanh toán nhạy cảm phải được xử lý thông qua đối tác thanh toán và không được lưu trực tiếp trong CAB | BG8 | Payment & Security |
| BR-08 | CAB cung cấp cơ chế thông báo cho khách hàng và tài xế khi xảy ra các sự kiện quan trọng trong quá trình đặt và thực hiện chuyến | BG3 | Notification |
| BR-09 | Nhân viên vận hành có thể theo dõi các chuyến đang hoạt động và can thiệp để xử lý những trường hợp không thể giải quyết tự động | BG4 | Operation |
| BR-10 | Quyền sử dụng các chức năng quản trị được kiểm soát theo vai trò, đặc biệt đối với những thao tác có ảnh hưởng đến dữ liệu hoặc hoạt động kinh doanh | BG8 | Access Control |
| BR-11 | Các sự kiện và thao tác có tính chất quan trọng phải được ghi nhận để phục vụ việc kiểm tra và truy nguyên khi xảy ra vấn đề | BG8 | Audit |
| BR-12 | Hệ thống cần được tổ chức để sự cố tại một dịch vụ như thanh toán hoặc thông báo không làm ngừng toàn bộ hoạt động đặt xe | BG6 | Reliability |
| BR-13 | Nền tảng cần hỗ trợ việc thay thế hoặc bổ sung các đối tác bên ngoài như Payment, Notification và Map/Location mà không ảnh hưởng lớn đến các chức năng nghiệp vụ hiện có | BG7 | Extensibility |

## Bước 6 - Business Process

```mermaid
flowchart TD

    %% =========================
    %% CUSTOMER
    %% =========================
    subgraph CUSTOMER["Customer"]
        C1([Start])
        C2[Đăng nhập tài khoản]
        C3[Nhập điểm đón và điểm đến]
        C4[Lựa chọn loại xe]
        C5[Xác nhận yêu cầu đặt xe]
        C6[Theo dõi trạng thái chuyến]
        C7[Nhận thông báo]
        C8[Thanh toán]
        C9[Đánh giá tài xế]
        C10([End])
    end

    %% =========================
    %% CAB SYSTEM
    %% =========================
    subgraph CAB["CAB System"]
        B1[Tiếp nhận yêu cầu]
        B2[Khởi tạo chuyến xe]
        B3[Kiểm tra tài xế khả dụng]
        B4{Có tài xế phù hợp?}
        B5[Gửi yêu cầu nhận chuyến]
        B6{Tài xế phản hồi?}
        B7[Timeout / Từ chối]
        B8[Tìm tài xế tiếp theo]
        B9[Xác nhận tài xế]
        B10[Cập nhật trạng thái chuyến]
        B11[Xác nhận hoàn thành chuyến]
        B12[Tính cước]
        B13{Phương thức thanh toán?}
        B14[Tiếp nhận kết quả thanh toán]
        B15[Đánh dấu thanh toán thất bại]
        B16[Thực hiện thanh toán lại]
        B17[Hoàn tất chuyến]
    end

    %% =========================
    %% DRIVER
    %% =========================
    subgraph DRIVER["Driver"]
        D1[Nhận yêu cầu chuyến]
        D2{Nhận chuyến?}
        D3[Di chuyển đến điểm đón]
        D4[Xác nhận đã đến]
        D5[Đón khách]
        D6[Đang thực hiện chuyến]
        D7[Xác nhận hoàn thành]
    end

    %% =========================
    %% EXTERNAL SERVICES
    %% =========================
    subgraph EXTERNAL["External Services"]
        P1[Payment Provider]
        N1[Notification Provider]
        M1[Map / Location Provider]
    end

    %% =========================
    %% OPERATION
    %% =========================
    subgraph OPERATION["Operation / Admin"]
        O1[Theo dõi chuyến và tài xế]
        O2[Xử lý trường hợp bất thường]
    end

    %% =========================
    %% BOOKING
    %% =========================
    C1 --> C2
    C2 --> C3
    C3 --> C4
    C4 --> C5

    C5 --> B1
    B1 --> B2
    B2 --> B3

    %% =========================
    %% DRIVER MATCHING
    %% =========================
    M1 -. "Cung cấp dữ liệu vị trí" .-> B3
    B3 --> B4

    B4 -- "Không" --> N1
    N1 --> C7
    C7 --> C10

    B4 -- "Có" --> B5
    B5 --> N1
    N1 --> D1

    D1 --> D2

    D2 -- "Từ chối" --> B7
    D2 -- "Không phản hồi" --> B7
    B7 --> B8
    B8 --> B3

    D2 -- "Chấp nhận" --> B9
    B9 --> N1
    N1 --> C7
    C7 --> C6

    %% =========================
    %% TRIP EXECUTION
    %% =========================
    B9 --> D3
    D3 --> D4

    D4 --> B10
    B10 --> N1
    N1 --> C7

    D4 --> D5
    D5 --> B10

    B10 --> D6
    D6 --> C6

    D6 --> D7
    D7 --> B11

    %% =========================
    %% FARE CALCULATION
    %% =========================
    B11 --> B12
    B12 --> B13

    %% =========================
    %% PAYMENT
    %% =========================
    B13 -- "Tiền mặt" --> B14

    B13 -- "Điện tử" --> P1
    P1 --> B14

    B14 --> B17

    %% =========================
    %% PAYMENT FAILURE
    %% =========================
    P1 --> B15
    B15 --> N1
    N1 --> C7
    C7 --> B16

    B16 -- "Retry" --> P1
    B16 -- "Không retry" --> B17

    %% =========================
    %% COMPLETION
    %% =========================
    B17 --> N1
    N1 --> C7
    C7 --> C9
    C9 --> C10

    %% =========================
    %% OPERATION MONITORING
    %% =========================
    O1 -. "Giám sát" .-> B2
    O1 -. "Giám sát" .-> B3
    O1 -. "Giám sát" .-> B10
    O1 -. "Giám sát" .-> B11
    O1 -. "Giám sát" .-> B17

    O1 --> O2
    O2 -. "Can thiệp xử lý" .-> B10

    %% =========================
    %% STYLING
    %% =========================
    classDef customer fill:#E3F2FD,stroke:#1976D2,color:#0D47A1
    classDef cab fill:#E8F5E9,stroke:#388E3C,color:#1B5E20
    classDef driver fill:#FFF3E0,stroke:#F57C00,color:#E65100
    classDef external fill:#F3E5F5,stroke:#7B1FA2,color:#4A148C
    classDef operation fill:#FFFDE7,stroke:#FBC02D,color:#5F4600
    classDef startend fill:#ECEFF1,stroke:#455A64,color:#263238

    class C1,C10 startend
    class C2,C3,C4,C5,C6,C7,C8,C9 customer
    class B1,B2,B3,B4,B5,B6,B7,B8,B9,B10,B11,B12,B13,B14,B15,B16,B17 cab
    class D1,D2,D3,D4,D5,D6,D7 driver
    class P1,N1,M1 external
    class O1,O2 operation
```

## Bước 7 - Functional Requirement
