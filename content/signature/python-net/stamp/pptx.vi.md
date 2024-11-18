



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:49
draft: false
lang: vi
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Tạo dấu tròn và vuông trong PPTX bằng Python"
head_description: "Tạo và chèn các dấu cá nhân hóa vào tệp PPTX với API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Tạo dấu cho PPTX" 
description: "Thêm dấu tùy chỉnh vào bất kỳ phần nào của tài liệu của bạn với GroupDocs.Signature for Python via .NET, cung cấp tính linh hoạt tuyệt vời cho việc đặt và cấu hình để đáp ứng nhu cầu kinh doanh của bạn."
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
    title: "Tổng quan về GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) là một công cụ toàn diện cho phép bạn chèn nhiều loại chữ ký vào tài liệu, bao gồm dấu tùy chỉnh. Hỗ trợ hơn 60 định dạng tệp—từ PDF và tài liệu Word đến hình ảnh và tệp ZIP—bạn có thể nâng cao tài liệu của mình bằng văn bản, hình ảnh, mã vạch, siêu dữ liệu, chứng chỉ số và dấu. Bạn cũng có quyền kiểm soát hoàn toàn để tìm kiếm, xác minh, chỉnh sửa hoặc xóa bất kỳ chữ ký nào đã được áp dụng.

############################# Steps ############################
steps:
    enable: true
    title: "Cách thêm một dấu vào PPTX bằng Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) cung cấp các công cụ tạo dấu mạnh mẽ để nâng cao các ứng dụng Python via .NET. Sử dụng nó để thiết kế và thực hiện các dấu tùy chỉnh cho các trang tài liệu của bạn.
      
      1. Cung cấp tài liệu PPTX mà bạn muốn đóng dấu.
      2. Sử dụng StampSignOptions để cấu hình tất cả các cài đặt cần thiết.
      3. Thêm nhiều dòng dấu nếu cần.
      4. Áp dụng dấu và lưu tài liệu đã được cập nhật.
   
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

            # Gắn đường dẫn tài liệu vào trường hợp Signature
            with sg.Signature('input.pptx') as signature:

                # Thiết lập StampSignOptions với các chi tiết dấu cần thiết
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Thêm một hoặc nhiều dòng vào dấu
                outerLine = sg.StampLine()
                outerLine.Text = "* The Best Company *"
                outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                outerLine.Font = sg.SignatureFont()
                outerLine.Font.Size = 12
                outerLine.Font.FamilyName = "Arial"
                outerLine.Height = 22
                outerLine.TextBottomIntent = 6
                outerLine.TextColor = sg.Color.WhiteSmoke
                outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                options.OuterLines.Add(outerLine)

                # Lưu tài liệu với dấu đã áp dụng
                result = signature.Sign("output.pptx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Sử dụng chữ ký để bảo mật và nâng cao tính toàn vẹn của tài liệu"
  description: "Với thư viện GroupDocs.Signature for Python via .NET, bạn có thể dễ dàng thêm chức năng chữ ký vào tài liệu của mình. Tạo, sửa đổi, xác minh hoặc xóa dấu tùy chỉnh và các loại chữ ký khác, cung cấp sự linh hoạt và bảo mật cho quy trình làm việc của tài liệu."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Chữ ký Dấu do GroupDocs.Signature cung cấp"
  features:
    # feature loop
    - title: "Ký tài liệu hoàn chỉnh"
      content: "Nâng cao tài liệu của bạn bằng cách thêm chữ ký như văn bản, hình ảnh, mã vạch, mã QR và dấu vào bất kỳ vị trí nào trên bất kỳ trang nào. Quản lý siêu dữ liệu nhúng và áp dụng chứng chỉ số để bảo vệ chống lại các thay đổi trái phép."

    # feature loop
    - title: "Tìm kiếm và xác minh chữ ký hiệu quả"
      content: "Sau khi ký, sử dụng công cụ tìm kiếm nâng cao để tìm tất cả các chữ ký nhúng. Dễ dàng xác minh hoặc quản lý dữ liệu chữ ký để đảm bảo tính toàn vẹn của tài liệu."

    # feature loop
    - title: "Chỉnh sửa và tùy chỉnh chữ ký"
      content: "Thay đổi chữ ký đã thêm trước đó một cách dễ dàng. Dù bạn muốn thay đổi nội dung, vị trí, kích thước hay màu sắc, GroupDocs.Signature for Python via .NET mang đến cho bạn quyền kiểm soát hoàn toàn để điều chỉnh chữ ký theo nhu cầu."

    # feature loop
    - title: "Dễ dàng xóa chữ ký"
      content: "Nếu bạn cần xóa chữ ký, GroupDocs.Signature for Python via .NET cung cấp tất cả các công cụ cần thiết để xóa bất kỳ loại nào, bao gồm dấu và chứng chỉ số, giúp bạn giữ cho tài liệu của mình luôn cập nhật và tuân thủ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cách thêm dấu tùy chỉnh vào tài liệu"
      content: |
        Ví dụ này cho thấy cách tạo và chèn dấu tùy chỉnh với các chi tiết văn bản cụ thể vào một tài liệu.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Cung cấp tài liệu mà bạn muốn đóng dấu
              with sg.Signature('input.pptx') as signature:

                    # Thiết lập các tùy chọn dấu với các cài đặt mong muốn của bạn
                    options = sg.StampSignOptions()

                    # Định nghĩa kích thước và vị trí của dấu trên trang
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Thêm các đường tròn bên ngoài với văn bản
                    outerLine = sg.StampLine()
                    outerLine.Text = "* The best  choice *"
                    outerLine.TextRepeatType = sg.StampTextRepeatType.FullTextRepeat
                    outerLine.Font = sg.SignatureFont()
                    outerLine.Font.Size = 12
                    outerLine.Font.FamilyName = "Arial"
                    outerLine.Height = 22
                    outerLine.TextBottomIntent = 6
                    outerLine.TextColor = sg.Color.WhiteSmoke
                    outerLine.BackgroundColor = sg.Color.DarkSlateBlue
                    options.OuterLines.Add(outerLine)

                    # Tùy chọn, thêm các đường vuông bên trong
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Hoàn tất và lưu tài liệu đã được đóng dấu
                    result = signature.Sign("output.pptx", options)
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
            link: "/examples/signature/formats/signature_stamp.pptx"
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
    title: "Khám phá các tính năng chính"
    exclude: "stamp"
    description: "Tìm một loạt các tùy chọn để tạo, quản lý và xóa chữ ký, mang lại cho bạn quyền kiểm soát hoàn toàn quy trình làm việc của tài liệu."
    items: 
          
        # operation loop 1
        - name: "Chữ ký điện tử"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "Thêm các loại chữ ký khác nhau vào các định dạng tệp được hỗ trợ"

        # operation loop 2
        - name: "Thêm văn bản vào tài liệu"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "Nâng cao nội dung tài liệu với các chữ ký văn bản tùy chỉnh"

        # operation loop 3
        - name: "Chữ ký hình ảnh"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "Đặt bất kỳ hình ảnh nào ở bất kỳ vị trí nào trong tài liệu"

        # operation loop 4
        - name: "Tạo mã vạch"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "Tạo và chèn các mã vạch khác nhau vào các tài liệu được hỗ trợ"

        # operation loop 5
        - name: "Tạo mã QR"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Tạo mã QR, bao gồm mã QR, để ký tài liệu"
          
        # operation loop 6
        - name: "Chứng chỉ số"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "Bảo mật doanh nghiệp và ký các tài liệu bằng chứng chỉ số"

        # operation loop 7
        - name: "Chữ ký đóng dấu"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "Sử dụng Trình tạo đóng dấu để tạo các dấu tròn hoặc vuông tùy chỉnh"
          
        # operation loop 8
        - name: "Tìm kiếm chữ ký"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "Tìm bất kỳ chữ ký nào đã được thêm trước đó trong tài liệu"
          
        # operation loop 9
        - name: "Xác minh chữ ký"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "Xác minh tính xác thực của chữ ký sau khi đã được áp dụng"
          
        # operation loop 10
        - name: "Chỉnh sửa chữ ký"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "Chỉnh sửa dễ dàng nhiều loại chữ ký trong một tài liệu"
          
        # operation loop 11
        - name: "Xóa chữ ký"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "Xóa một loạt các chữ ký đã được áp dụng trước đó"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Áp dụng dấu cho nhiều định dạng tài liệu"
    exclude: "PPTX"
    description: "Với API GroupDocs.Signature, bạn có thể chèn dấu tùy chỉnh vào hơn 60 loại tệp tiêu chuẩn. Dễ dàng áp dụng dấu ở bất kỳ đâu trong tài liệu của bạn, nâng cao tính cá nhân hóa và theo dõi."
    items: 
          
        # format loop 1
        - name: "Đóng dấu PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 2
        - name: "Đóng dấu DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 3
        - name: "Đóng dấu JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Hình ảnh JPEG"
          
        # format loop 4
        - name: "Đóng dấu PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"
          
        # format loop 5
        - name: "Đóng dấu XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"


          

---