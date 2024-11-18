



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:52
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Chèn chữ ký hình ảnh vào tệp DOCX với Python"
head_description: "Nhúng chữ ký hình ảnh vào tài liệu DOCX cho Python chỉ với vài dòng mã. Sử dụng API GroupDocs.Signature for Python via .NET để thêm chữ ký dạng hình ảnh một cách dễ dàng."

############################# Header ############################
title: "Thêm chữ ký hình ảnh vào DOCX" 
description: "Sử dụng GroupDocs.Signature for Python via .NET để tích hợp chữ ký hình ảnh vào nhiều định dạng tài liệu văn phòng khác nhau, bao gồm PDF, Word, Excel và các tệp hình ảnh. Thêm hình ảnh chữ ký của quản lý vào tài liệu sẽ tăng tính chuyên nghiệp, nâng cao cả ấn tượng thị giác và tính xác thực của tài liệu."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Khám phá GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) cung cấp nhiều tùy chọn linh hoạt để nhúng chữ ký hình ảnh vào bất kỳ đâu trong tài liệu của bạn. Tối ưu hóa quy trình làm việc bằng cách thêm hình ảnh vào PDF, tài liệu Word, bảng tính Excel, bài thuyết trình PowerPoint và các định dạng hình ảnh phổ biến bằng cách sử dụng thư viện mạnh mẽ của chúng tôi.

############################# Steps ############################
steps:
    enable: true
    title: "Cách chèn chữ ký hình ảnh vào tệp DOCX bằng Python"
    content: |
      Sử dụng [GroupDocs.Signature](/signature/python-net/) để cung cấp cho ứng dụng Python via .NET khả năng chính xác thêm chữ ký hình ảnh vào bất kỳ đâu trong tài liệu DOCX. Nâng cao sản phẩm của bạn bằng cách tích hợp giải pháp của chúng tôi.
      
      1. Tạo một thể hiện Signature với tài liệu DOCX.
      2. Cấu hình ImageSignOptions với hình ảnh mong muốn cho chữ ký.
      3. Đặt hình ảnh chính xác tại vị trí đã chọn trên tài liệu.
      4. Lưu tài liệu đã ký vào vị trí đã chỉ định.
   
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
            with sg.Signature('input.docx') as signature:

                # Cấu hình ImageSignOptions với hình ảnh đã chọn cho chữ ký
                options = sg.ImageSignOptions("company_logo.jpg")

                # Đặt hình ảnh ở góc trên bên trái của mỗi trang
                options.AllPages = True
                options.Left = 100
                options.Top = 200
                
                # Lưu tài liệu đã ký
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Các tính năng ký tài liệu toàn diện"
  description: "API của chúng tôi hỗ trợ nhiều chức năng chữ ký khác nhau. Bạn có thể thêm, cập nhật, xóa, tìm kiếm và xác thực các loại chữ ký khác nhau, bao gồm chữ ký hình ảnh."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Tích hợp chữ ký hình ảnh"
  features:
    # feature loop
    - title: "Chèn hình ảnh vào tài liệu văn phòng"
      content: "Nhúng chữ ký điện tử và hình ảnh tại bất kỳ vị trí nào trong tài liệu. Nâng cao chức năng và tính bảo mật của tài liệu bằng cách cải thiện nội dung với hình ảnh, mã vạch, văn bản, siêu dữ liệu hoặc chứng thư số."

    # feature loop
    - title: "Tìm kiếm và xác thực chữ ký"
      content: "Đảm bảo tính toàn vẹn của tài liệu bằng cách xác thực tính xác thực của các chữ ký. Lấy danh sách chi tiết tất cả chữ ký trong tài liệu và đánh giá các thuộc tính của từng chữ ký."

    # feature loop
    - title: "Chỉnh sửa chữ ký hiện có"
      content: "Cập nhật dễ dàng nội dung, hình thức, kích thước hoặc vị trí của các chữ ký trong tài liệu của bạn để đáp ứng các nhu cầu thay đổi."

    # feature loop
    - title: "Xóa chữ ký không cần thiết"
      content: "API của chúng tôi cung cấp quyền kiểm soát hoàn toàn, cho phép bạn xóa chữ ký khỏi hầu hết các định dạng tệp được hỗ trợ bất cứ khi nào cần thiết."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Nâng cao tài liệu với chữ ký hình ảnh"
      content: |
        Tìm hiểu cách nhúng chữ ký hình ảnh vào tài liệu kinh doanh của bạn để làm phong phú nội dung.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Chọn tài liệu cần ký
              with sg.Signature('input.docx') as signature:

                    # Cấu hình tùy chọn hình ảnh với đường dẫn tệp hình ảnh
                    options = sg.ImageSignOptions("manager_signature.jpg")

                    # Chỉ định kích thước của chữ ký hình ảnh
                    options.Width = 100
                    options.Height = 100

                    # Đặt hình ảnh ở góc dưới bên phải của trang
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right

                    # Áp dụng khoảng cách từ các cạnh trang theo yêu cầu
                    options.Margin = sg.Padding()
                    options.Margin.Bottom = 120
                    options.Margin.Right = 120

                    # Tùy chọn, thêm viền quanh hình ảnh
                    options.Border = sg.Border()
                    options.Border.Visible = True
                    options.Border.Color = sg.Color.OrangeRed
                    options.Border.DashStyle = sg.DashStyle.DashDotDot
                    options.Border.Weight = 5

                    # Xoay hình ảnh để đảm bảo căn chỉnh chính xác
                    options.RotationAngle = 45

                    # Lưu tài liệu đã cập nhật
                    result = signature.Sign("output.docx", options)
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
            link: "/examples/signature/formats/signature_image.docx"
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
    title: "Khám phá các tính năng của chúng tôi"
    exclude: "image"
    description: "Khám phá các loại chữ ký và thao tác mà nền tảng của chúng tôi cung cấp."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Nhúng hình ảnh vào nhiều định dạng tệp"
    exclude: "DOCX"
    description: "Sử dụng API Python via .NET để chèn hình ảnh vào nhiều định dạng tài liệu khác nhau. Dễ dàng thay đổi kích thước, xác định vị trí, chọn các trang cụ thể và áp dụng chữ ký hình ảnh, giúp bạn hoàn toàn kiểm soát bố cục tài liệu của mình."
    items: 
          
        # format loop 1
        - name: "Ký PDF bằng hình ảnh"
          format: "PDF"
          link: "/signature/python-net/image/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Ký DOCX bằng hình ảnh"
          format: "DOCX"
          link: "/signature/python-net/image/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Ký JPEG bằng hình ảnh"
          format: "JPEG"
          link: "/signature/python-net/image/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Ký PPTX bằng hình ảnh"
          format: "PPTX"
          link: "/signature/python-net/image/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Ký XLSX bằng hình ảnh"
          format: "XLSX"
          link: "/signature/python-net/image/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---