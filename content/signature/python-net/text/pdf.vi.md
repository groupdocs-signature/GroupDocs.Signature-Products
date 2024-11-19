



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:15
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Thêm chữ ký văn bản vào PDF bằng Python"
head_description: "Tận dụng API Python để nhúng chữ ký dựa trên văn bản vào các tệp PDF, hỗ trợ các định dạng như PDF, Word, Excel, PowerPoint, hình ảnh và ZIP."

############################# Header ############################
title: "Thêm chữ ký văn bản vào PDF một cách dễ dàng" 
description: "Tích hợp liền mạch chữ ký văn bản tùy chỉnh vào tài liệu của bạn bằng GroupDocs.Signature for Python via .NET. Đơn giản hóa quy trình công việc của bạn với các tùy chọn tùy chỉnh chữ ký linh hoạt."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dùng thử miễn phí hôm nay"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Khám phá sức mạnh của GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) cung cấp một nền tảng toàn diện để nhúng chữ ký văn bản tùy chỉnh, giúp quy trình công việc tài liệu suôn sẻ hơn. Tùy chỉnh nội dung và hình thức của chữ ký trên các tài liệu để tăng cường hiệu suất và cải thiện quản lý tài liệu.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tạo chữ ký văn bản PDF với Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) cho phép tích hợp chữ ký văn bản dễ dàng vào các tệp PDF trong các ứng dụng Python via .NET. Nhanh chóng thêm chức năng cho sản phẩm của bạn với giải pháp này.
      
      1. Cung cấp tài liệu PDF cho trình tạo Signature.
      2. Tạo TextSignOptions với văn bản chữ ký của bạn.
      3. Thiết lập các thuộc tính trực quan của chữ ký.
      4. Chèn chữ ký vào các trang mong muốn của tài liệu.
   
    code:
      platform: "python-net"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Chữ ký mẫu"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "nhấp để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Khởi tạo Signature với đường dẫn tài liệu
            with sg.Signature('input.pdf') as signature:

                # Thiết lập TextSignOptions với nội dung chữ ký mong muốn của bạn
                options = sg.TextSignOptions("Approved")

                # Chọn màu sắc và phông chữ cho chữ ký
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Áp dụng chữ ký văn bản vào tài liệu
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Quản lý chữ ký văn bản hoàn chỉnh"
  description: "GroupDocs.Signature for Python via .NET giúp bạn quản lý quy trình công việc tài liệu bằng cách thêm chữ ký văn bản tùy chỉnh vào các định dạng phổ biến. Dễ dàng kiểm soát hình thức, vị trí và nội dung của chữ ký để phù hợp với nhu cầu của bạn."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Khám phá các tính năng của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Chữ ký tài liệu linh hoạt"
      content: "Thêm nhiều loại chữ ký—văn bản, hình ảnh, mã vạch, mã QR và con dấu—vào bất kỳ trang tài liệu nào. Sử dụng metadata để bao gồm thông tin ẩn và bảo vệ tệp của bạn bằng chứng chỉ số."

    # feature loop
    - title: "Xác minh và tìm kiếm chữ ký"
      content: "Sử dụng các công cụ nâng cao để kiểm tra tính toàn vẹn của các tài liệu đã ký. Tìm kiếm và phân tích tất cả chữ ký trong một tệp để xác minh thêm."

    # feature loop
    - title: "Chỉnh sửa hoặc xóa chữ ký"
      content: "Cập nhật dễ dàng nội dung, hình thức hoặc vị trí của các chữ ký hiện có. Xóa các chữ ký cũ để giữ cho tài liệu của bạn luôn cập nhật."

    # feature loop
    - title: "Chữ ký văn bản chuyên dụng"
      content: "Áp dụng chữ ký văn bản đặc thù cho từng tài liệu, như bản quyền cho tệp Word hoặc con dấu cho PDF, mang lại mức độ kiểm soát và tùy chỉnh bổ sung."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Thêm chữ ký văn bản vào tài liệu"
      content: |
        Tìm hiểu cách nhúng chữ ký văn bản vào tài liệu để cải thiện quy trình của bạn.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Chọn tài liệu để ký
              with sg.Signature('input.pdf') as signature:

                    # Thiết lập tùy chọn văn bản với nội dung mong muốn
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Định nghĩa kích thước và vị trí của chữ ký
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Đặt khoảng cách từ các cạnh trang
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Chọn màu sắc văn bản và kiểu chữ
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Thêm viền quanh chữ ký văn bản
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Tùy chỉnh nền nếu cần
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Tùy chọn lưu chữ ký dưới dạng hình ảnh để tương thích
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Lưu tài liệu với chữ ký đã nhúng
                    result = signature.Sign("output.pdf", options)
          ```
        platform: "python-net"
        copy_title: "Sao chép"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/signature/formats/signature_text.pdf"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng bắt đầu? "
  description: "Dùng thử các tính năng của GroupDocs.Signature miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Các tính năng chữ ký nâng cao"
    exclude: "text"
    description: "API của chúng tôi hỗ trợ quản lý chu trình hoàn chỉnh cho bảy loại chữ ký, cho phép bạn tạo, quản lý, xác minh và tùy chỉnh chữ ký của mình một cách dễ dàng."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/python-net/esign/pdf/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/python-net/text/pdf/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/python-net/image/pdf/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/python-net/barcode/pdf/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/python-net/stamp/pdf/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Nhúng chữ ký văn bản trong nhiều định dạng"
    exclude: "PDF"
    description: "Với API Python via .NET, bạn có thể thêm chữ ký văn bản vào các tài liệu Office khác nhau, cho phép bạn hoàn toàn kiểm soát chu trình của tài liệu và nâng cao bảo mật."
    items: 
          
        # format loop 1
        - name: "Chữ ký văn bản PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Chữ ký văn bản DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Chữ ký văn bản JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Chữ ký văn bản PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Chữ ký văn bản XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---