



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:19
draft: false
lang: vi
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Tạo chữ ký điện tử cho PDF bằng Python"
head_description: "Ký xác thực tài liệu PDF bằng Python chỉ trong vài dòng mã. Sử dụng GroupDocs.Signature for Python via .NET để ký nhiều định dạng tệp khác nhau."

############################# Header ############################
title: "Ký điện tử PDF" 
description: "Đảm bảo an ninh và tính xác thực của tài liệu bằng cách áp dụng chứng chỉ điện tử thông qua GroupDocs.Signature for Python via .NET. Giải pháp của chúng tôi cho phép bạn ký và bảo vệ tài liệu của mình bằng các công cụ mạnh mẽ."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Những gì là GroupDocs.Signature for Python via .NET?"
    link: "/signature/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) là một công cụ ký toàn diện hỗ trợ nhiều nhiệm vụ xử lý tài liệu. Nó cho phép bạn thêm văn bản, hình ảnh, chứng chỉ điện tử, và dấu vào hơn 60 định dạng tệp—bao gồm PDF, tệp MS Office, hình ảnh, và ZIP. Với GroupDocs.Signature for Python via .NET, bạn cũng có thể tìm kiếm, xác minh, cập nhật hoặc xóa chữ ký khi cần.

############################# Steps ############################
steps:
    enable: true
    title: "Cách bảo vệ PDF bằng chứng chỉ điện tử trong Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) giúp các nhà phát triển Python via .NET bảo mật tệp PDF bằng cách thêm chữ ký điện tử. Củng cố các ứng dụng doanh nghiệp của bạn với các tính năng bảo vệ tài liệu mạnh mẽ.
      
      1. Tải tệp PDF vào lớp Signature.
      2. Áp dụng chứng chỉ điện tử và mật khẩu của nó để bảo mật tệp.
      3. Tùy chọn, thêm hiển thị hình ảnh của chữ ký điện tử trên các trang tài liệu.
      4. Ký tài liệu để ngăn chặn các thay đổi trái phép.
   
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

            # Sử dụng Signature để ký điện tử tài liệu
            with sg.Signature('input.pdf') as signature:

                # Nhập chứng chỉ điện tử và mật khẩu của nó
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Tùy chọn cấu hình cách chữ ký sẽ trông như thế nào
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # Hoàn tất tài liệu với chứng chỉ điện tử
                result = signature.Sign("output.pdf", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Nâng cao và bảo mật tài liệu với chữ ký điện tử"
  description: "Thư viện GroupDocs.Signature for Python via .NET được thiết kế để ký tất cả các định dạng tệp chính. Đơn giản hóa quy trình của bạn bằng cách thêm, xác minh, cập nhật hoặc xóa các loại chữ ký khác nhau một cách dễ dàng."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Signature"
  features:
    # feature loop
    - title: "Thêm chữ ký vào tài liệu của bạn"
      content: "Chèn chữ ký văn bản, hình ảnh, mã vạch, mã QR, hoặc dấu một cách chính xác vào bất kỳ đâu trong tài liệu được hỗ trợ. Bạn cũng có thể quản lý siêu dữ liệu ẩn, như EXIF trong hình ảnh, để đảm bảo tính toàn vẹn của tài liệu với chữ ký điện tử."

    # feature loop
    - title: "Xác minh và tìm kiếm chữ ký"
      content: "Sau khi ký, bạn có thể xác minh tài liệu một cách dễ dàng để đảm bảo quá trình chính xác. Truy xuất và quản lý tất cả chữ ký trong tệp của bạn với khả năng tìm kiếm mạnh mẽ."

    # feature loop
    - title: "Chỉnh sửa chữ ký hiện có"
      content: "Hầu hết các chữ ký có thể tùy chỉnh hoàn toàn. Bạn có thể chỉnh sửa văn bản, di chuyển các phần tử, thay đổi màu sắc, điều chỉnh kích thước, và nhiều hơn nữa để phù hợp với nhu cầu của bạn."

    # feature loop
    - title: "Xóa chữ ký không cần thiết"
      content: "Giải pháp của chúng tôi hỗ trợ quản lý chữ ký hoàn chỉnh, cho phép bạn xóa chữ ký, bao gồm cả chứng chỉ điện tử, khỏi bất kỳ tài liệu nào khi cần."
      
  code_samples:
    # code sample loop
    - title: "Bảo vệ tài liệu bằng chữ ký điện tử"
      content: |
        Tìm hiểu cách bảo mật tài liệu của bạn bằng cách áp dụng chữ ký điện tử để ngăn chặn các thay đổi trái phép.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Tải tài liệu cần được ký
            with sg.Signature('input.pdf') as signature:

                # Sử dụng chứng chỉ điện tử hợp lệ với mật khẩu tương ứng
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Thêm thông tin văn bản bổ sung nếu cần
                options.Reason = "Security issue"
                options.Contact = "John Smith"
                options.Location = "Office D.W."

                # Bao gồm hình ảnh hoặc các tùy chọn khác để đại diện hình ảnh cho chữ ký
                options.ImageFilePath = "image.png"
                options.AllPages = True
                options.VerticalAlignment = sg.VerticalAlignment.Center
                options.HorizontalAlignment = sg.HorizontalAlignment.Left
                options.Width = 60
                options.Height = 80

                options.Margin = sg.Padding()
                options.Margin.Bottom = 10
                options.Margin.Right = 10

                # Lưu tài liệu đã ký ở một vị trí an toàn
                result = signature.Sign("output.pdf", options)
        ```
        {{< /landing/code >}}


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
    exclude: "digital"
    description: "Chúng tôi cung cấp một loạt các lựa chọn chữ ký và các thao tác tài liệu mạnh mẽ."
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
    title: "Ký tài liệu trên nhiều định dạng"
    exclude: "PDF"
    description: "Với API Python via .NET, bạn có thể xử lý hơn 60 định dạng khác nhau, thêm chữ ký, áp dụng chứng chỉ điện tử để bảo mật và quản lý chữ ký trên các trang khác nhau."
    items: 
          
        # format loop 1
        - name: "Bảo vệ PDF"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Bảo vệ DOCX"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Bảo vệ PPTX"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 4
        - name: "Bảo vệ XLSX"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---