



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Tạo mã QR cho các tệp PDF bằng Python"
head_description: "Sử dụng API GroupDocs.Signature để tạo và nhúng mã QR vào các tệp PDF. Đặt mã QR trên bất kỳ trang nào để thêm chức năng bổ sung."

############################# Header ############################
title: "Tạo mã QR cho PDF" 
description: "Tạo nhanh mã vạch 2D sử dụng dữ liệu văn bản hoặc số và áp dụng chúng cho nhiều trang và định dạng khác nhau, bao gồm PDF, Word, Excel và nhiều hơn nữa với GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dùng thử miễn phí"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Khám phá các tính năng của GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) cung cấp một loạt các khả năng, cho phép người dùng tạo và nhúng các loại chữ ký khác nhau trên các định dạng tài liệu chính. Cho dù là PDF, Word, Excel, PowerPoint hay hình ảnh, hãy nâng cao tài liệu của bạn với chữ ký dạng Văn bản, Hình ảnh, Mã vạch, Mã QR, Siêu dữ liệu, Chữ ký số hoặc Dấu.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để tạo và chèn mã QR vào PDF"
    content: |
      [GroupDocs.Signature](/signature/python-net/) cho phép bạn tạo mã QR trong các định dạng phổ biến và đặt chúng trên các trang PDF. Với sự hỗ trợ cho hơn 10 loại mã QR, bạn có thể tích hợp chức năng này mượt mà vào các ứng dụng Python via .NET. Nâng cao tài liệu của bạn với chữ ký mã QR bằng sản phẩm của chúng tôi.
      
      1. Lấy tệp PDF hoặc luồng mà mã QR sẽ được thêm vào.
      2. Cung cấp văn bản cần thiết cho QrCodeSignOptions.
      3. Tùy chỉnh cài đặt hình ảnh như màu sắc, vị trí và kích thước.
      4. Lưu tài liệu với mã QR đã nhúng.
   
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

            # Khởi tạo một instance Signature mới với tài liệu
            with sg.Signature('input.pdf') as signature:

                # Sử dụng QrCodeSignOptions để nhúng mã QR vào tài liệu
                options = sg.QrCodeSignOptions("Text Content")

                # Xác định loại chữ ký và đặt vị trí của nó trên trang
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Lưu tài liệu với mã QR đã nhúng
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tích hợp chữ ký hoàn chỉnh cho tài liệu"
  description: "Với API GroupDocs.Signature for Python via .NET, người dùng có thể tạo, sửa đổi, tìm kiếm, xác thực và xóa các loại chữ ký khác nhau, đơn giản hóa quy trình công việc tài liệu một cách chính xác."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Các Tính năng Chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Áp dụng nhiều loại chữ ký"
      content: "GroupDocs.Signature cho phép áp dụng chữ ký Văn bản, Hình ảnh, Mã vạch, Mã QR và Dấu lên bất kỳ tài liệu nào. Bạn có thể đặt chữ ký một cách chính xác trên bất kỳ trang nào và quản lý siêu dữ liệu dễ dàng. Bảo vệ tài liệu của bạn khỏi những thay đổi trái phép bằng chứng nhận số."

    # feature loop
    - title: "Tìm kiếm và xác thực chữ ký"
      content: "Xác minh chữ ký tài liệu để đảm bảo tính xác thực và độ chính xác bằng các công cụ xác thực nâng cao. Dễ dàng lấy danh sách chi tiết tất cả chữ ký đã nhúng trong một tài liệu để có cái nhìn tổng quan tốt hơn."

    # feature loop
    - title: "Sửa đổi chữ ký hiện có"
      content: "Bạn có thể cập nhật các chữ ký đã áp dụng trước đó bằng cách điều chỉnh nội dung, vị trí, màu sắc, kích thước và các thuộc tính khác để phù hợp với nhu cầu cụ thể của bạn."

    # feature loop
    - title: "Dễ dàng xóa chữ ký"
      content: "Đơn giản hóa quản lý tài liệu bằng cách nhanh chóng xóa các chữ ký không mong muốn. Cho dù đó là chứng nhận số hay một loại chữ ký khác, việc xóa có thể thực hiện hiệu quả."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tùy chỉnh Một Mã QR Được Tạo"
      content: |
        Ví dụ này cho thấy cách đặt một mã QR tùy chỉnh trên một trang PDF.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Lấy tài liệu cần ký và chuyển nó cho Signature
              with sg.Signature('input.pdf') as signature:

                    # Cấu hình các tùy chọn mã QR với văn bản cần thiết
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Đặt vị trí của mã QR trên trang
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Đặt khoảng cách cho chữ ký
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Chọn màu sắc cho mã QR
                    options.ForeColor = sg.Color.Red

                    # Xác định các tùy chọn phông chữ cho thông điệp
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Đặt màu nền và cọ cho mã QR
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Nhúng mã QR vào tài liệu
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
            link: "/examples/signature/formats/signature_qrcode.pdf"
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
    title: "Khám phá các giải pháp chữ ký của chúng tôi"
    exclude: "qrcode"
    description: "Chúng tôi cung cấp một loạt các loại chữ ký và hoạt động để đáp ứng nhu cầu tài liệu của bạn."
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
    title: "Nhúng mã QR vào các định dạng tài liệu khác nhau"
    exclude: "PDF"
    description: "Sử dụng API Python via .NET để nhúng mã QR vào bất kỳ định dạng tài liệu tiêu chuẩn nào trong ngành. Lưu trữ và mã hóa thông tin quan trọng trong mã vạch 2D để dễ dàng quét và truy xuất dữ liệu."
    items: 
          
        # format loop 1
        - name: "Mã QR cho PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Mã QR cho DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Mã QR cho JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Mã QR cho PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Mã QR cho XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---