



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:08
draft: false
lang: vi
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Nhúng mã vạch vào DOCX với Python"
head_description: "Thêm chữ ký mã vạch vào tài liệu DOCX một cách hiệu quả chỉ với vài dòng mã trong Python. GroupDocs.Signature cung cấp giải pháp ký kết liền mạch cho nhiều định dạng tài liệu."

############################# Header ############################
title: "Tạo mã vạch cho DOCX" 
description: "Với GroupDocs.Signature for Python via .NET, bạn có thể đặt mã vạch vào tài liệu kinh doanh của mình bất cứ lúc nào cần thiết. Giải pháp của chúng tôi cung cấp các tùy chọn linh hoạt để tùy chỉnh chữ ký mã vạch."
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
    title: "Giới thiệu về GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) là công cụ ký tài liệu mạnh mẽ hỗ trợ nhiều loại chữ ký, bao gồm văn bản, hình ảnh, mã vạch, chứng chỉ số và con dấu. Tương thích với hơn 60 định dạng tệp, chẳng hạn như PDF, MS Office, hình ảnh, ZIP, và nhiều hơn nữa, nó không chỉ cho phép bạn áp dụng chữ ký mà còn cho phép bạn tìm kiếm, xác minh, chỉnh sửa hoặc xóa chúng theo nhu cầu.

############################# Steps ############################
steps:
    enable: true
    title: "Bước để tạo và nhúng mã vạch vào DOCX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) cho phép bạn nhanh chóng và hiệu quả tạo và nhúng mã vạch vào tài liệu DOCX. Hỗ trợ hơn 60 định dạng mã vạch, các ứng dụng Python via .NET có thể dễ dàng thêm chức năng ký mã vạch bằng cách tích hợp thư viện của chúng tôi.
      
      1. Cung cấp tệp hoặc luồng DOCX để xử lý.
      2. Gán văn bản mã vạch cho đối tượng BarcodeSignOptions.
      3. Điều chỉnh tùy chọn mã vạch như vị trí và kích thước.
      4. Lưu tài liệu với mã vạch được nhúng.
   
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

            # Khởi tạo đối tượng Signature với đường dẫn tài liệu
            with sg.Signature('input.docx') as signature:

                # Sử dụng BarcodeSignOptions để thêm mã vạch vào tài liệu
                options = sg.BarcodeSignOptions('Business data')

                # Đặt loại mã vạch và cấu hình các thuộc tính của nó
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Lưu tài liệu đã ký
                result = signature.Sign('output.docx', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Nâng cao tài liệu của bạn với các tính năng chữ ký tiên tiến"
  description: "Thư viện GroupDocs.Signature for Python via .NET cung cấp các giải pháp toàn diện cho việc ký và xử lý tài liệu ở các định dạng thường dùng. Bạn có thể dễ dàng thêm, chỉnh sửa, xác minh hoặc xóa nhiều loại chữ ký để phù hợp với nhu cầu của mình."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Ký tài liệu linh hoạt"
      content: "Ký bất kỳ trang nào trong tài liệu hỗ trợ bằng văn bản, hình ảnh, mã vạch, mã QR hoặc con dấu. Thêm metadata ẩn như dữ liệu EXIF trong hình ảnh và đảm bảo bảo mật nội dung với chứng chỉ số để ngăn chặn các thay đổi trái phép."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký"
      content: "Công cụ của chúng tôi đảm bảo tính toàn vẹn của tài liệu của bạn bằng cách cho phép xác minh chữ ký. Bạn cũng có thể lấy danh sách đầy đủ tất cả chữ ký trong một tài liệu để quản lý dễ dàng."

    # feature loop
    - title: "Chỉnh sửa chữ ký một cách dễ dàng"
      content: "Chỉnh sửa các chữ ký hiện có một cách đơn giản. Điều chỉnh văn bản, điều chỉnh vị trí các phần tử, hoặc thay đổi màu sắc để phù hợp với nhu cầu tài liệu của bạn."

    # feature loop
    - title: "Dễ dàng xóa chữ ký"
      content: "Với chức năng toàn diện CRUD, GroupDocs.Signature for Python via .NET giúp bạn dễ dàng loại bỏ bất kỳ chữ ký không cần thiết hoặc lỗi thời nào khỏi tài liệu của bạn."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tạo và đặt chữ ký mã vạch"
      content: |
        Ví dụ này minh họa cách chèn một mã vạch tùy chỉnh vào tài liệu DOCX.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Cung cấp tài liệu cần ký
              with sg.Signature('input.docx') as signature:

                  # Đặt văn bản mã vạch và các tùy chọn chữ ký
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Chọn vị trí cho mã vạch trên trang
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Đặt khoảng cách giữa mã vạch và cạnh trang
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Chỉ định màu của các thanh mã vạch
                  options.ForeColor = sg.Color.Red

                  # Chọn kiểu chữ cho thông điệp mã vạch
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Đặt vị trí của văn bản thông điệp
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Ký và lưu tài liệu
                  result = signature.Sign('output.docx', options)
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
            link: "/examples/signature/formats/signature_barcode.docx"
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
    title: "Khám phá các tính năng chính của chúng tôi"
    exclude: "barcode"
    description: "Chúng tôi cung cấp nhiều tùy chọn chữ ký và hoạt động cho nhu cầu tài liệu của bạn."
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
    title: "Ký tài liệu ở nhiều định dạng"
    exclude: "DOCX"
    description: "API Python via .NET hỗ trợ ký hơn 60 định dạng tệp, cho phép bạn thêm nhiều loại chữ ký vào bất kỳ trang hoặc vị trí cụ thể nào trong tài liệu của bạn."
    items: 
          
        # format loop 1
        - name: "Thêm mã vạch vào PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Thêm mã vạch vào DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Thêm mã vạch vào JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Thêm mã vạch vào PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Thêm mã vạch vào XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---