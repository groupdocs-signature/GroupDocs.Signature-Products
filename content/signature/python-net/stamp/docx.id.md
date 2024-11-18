



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:48
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Buat cap bulat dan persegi dalam DOCX menggunakan Python"
head_description: "Hasilkan dan masukkan cap yang dipersonalisasi ke dalam file DOCX menggunakan API GroupDocs.Signature for Python via .NET."

############################# Header ############################
title: "Buat cap untuk DOCX" 
description: "Tambahkan cap yang dirancang khusus ke bagian manapun dari dokumen Anda dengan GroupDocs.Signature for Python via .NET, menawarkan fleksibilitas besar dalam penempatan dan konfigurasi sesuai kebutuhan bisnis Anda."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Gambaran Umum GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) adalah alat komprehensif yang memungkinkan Anda menyisipkan berbagai jenis tanda tangan ke dalam dokumen, termasuk cap kustom. Mendukung lebih dari 60 format file—dari PDF dan dokumen Word hingga gambar dan file ZIP—Anda dapat meningkatkan dokumen Anda dengan teks, gambar, kode batang, metadata, sertifikat digital, dan cap. Anda juga memiliki kontrol penuh untuk mencari, memverifikasi, mengedit, atau menghapus tanda tangan yang diterapkan.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menambahkan cap ke DOCX menggunakan Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) menyediakan alat pembuatan cap yang kuat untuk meningkatkan aplikasi Python via .NET Anda. Gunakan alat ini untuk merancang dan menerapkan cap kustom pada halaman dokumen Anda.
      
      1. Berikan dokumen DOCX yang ingin Anda cap.
      2. Gunakan StampSignOptions untuk mengonfigurasi semua pengaturan yang diperlukan.
      3. Tambahkan beberapa garis cap jika diperlukan.
      4. Terapkan cap dan simpan dokumen yang diperbarui.
   
    code:
      platform: "python-net"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command: "pip install groupdocs-signature-net"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/python-net/"
          
      content: |
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Lampirkan jalur dokumen ke instance Signature
            with sg.Signature('input.docx') as signature:

                # Siapkan StampSignOptions dengan detail cap yang diperlukan
                options = sg.StampSignOptions()
                options.Height = 180
                options.Width = 180

                # Tambahkan satu atau beberapa garis ke cap
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

                # Simpan dokumen dengan cap yang diterapkan
                result = signature.Sign("output.docx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Gunakan tanda tangan untuk mengamankan dan meningkatkan integritas dokumen"
  description: "Dengan pustaka GroupDocs.Signature for Python via .NET, Anda dapat dengan mulus menambahkan fungsionalitas tanda tangan ke dalam dokumen Anda. Buat, modifikasi, verifikasi, atau hapus cap kustom dan jenis tanda tangan lainnya, memberikan fleksibilitas dan keamanan untuk alur kerja dokumen Anda."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Tanda Tangan Cap Didukung oleh GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen lengkap"
      content: "Tingkatkan dokumen Anda dengan menambahkan tanda tangan seperti teks, gambar, kode batang, kode QR, dan cap di posisi mana pun pada halaman mana pun. Kelola metadata yang disematkan dan terapkan sertifikat digital untuk melindungi dari perubahan yang tidak sah."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan yang efisien"
      content: "Setelah menandatangani, gunakan alat pencarian canggih untuk menemukan semua tanda tangan yang disematkan. Verifikasi atau kelola data tanda tangan dengan mudah untuk memastikan integritas dokumen."

    # feature loop
    - title: "Edit dan sesuaikan tanda tangan"
      content: "Lakukan perubahan pada tanda tangan yang telah ditambahkan sebelumnya. Baik Anda ingin mengubah konten, posisi, ukuran, atau warna, GroupDocs.Signature for Python via .NET memberikan Anda kontrol penuh untuk menyesuaikan tanda tangan sesuai kebutuhan."

    # feature loop
    - title: "Mudah menghapus tanda tangan"
      content: "Jika Anda perlu menghapus tanda tangan, GroupDocs.Signature for Python via .NET menyediakan semua alat yang diperlukan untuk menghapus jenis apa pun, termasuk cap dan sertifikat digital, membantu Anda menjaga dokumen tetap terkini dan sesuai."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menambahkan cap kustom ke dokumen"
      content: |
        Contoh ini menunjukkan cara membuat dan menyisipkan cap kustom dengan detail teks tertentu ke dalam sebuah dokumen.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Berikan dokumen yang ingin Anda cap
              with sg.Signature('input.docx') as signature:

                    # Siapkan opsi cap dengan pengaturan yang diinginkan
                    options = sg.StampSignOptions()

                    # Tentukan ukuran dan letak cap di halaman
                    options.Height = 200
                    options.Width = 200
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right
                    options.AllPages = True

                    # Tambahkan garis luar melingkar dengan teks
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

                    # Jika perlu, tambahkan garis persegi bagian dalam
                    innerLine = sg.StampLine()
                    innerLine.Text = "Company #1"
                    innerLine.TextColor = sg.Color.MediumVioletRed
                    innerLine.Font = sg.SignatureFont()
                    innerLine.Font.Size = 20
                    innerLine.Font.Bold = True
                    innerLine.Height = 40
                    options.InnerLines.Add(innerLine)

                    # Finalisasi dan simpan dokumen yang dicap
                    result = signature.Sign("output.docx", options)
          ```
        platform: "python-net"
        copy_title: "Salin"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/signature/formats/signature_stamp.docx"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Python-via-.NET/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/python-net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan PyPi"
      link: "https://releases.groupdocs.com/signature/python-net/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/python-net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Jelajahi fitur kunci"
    exclude: "stamp"
    description: "Temukan berbagai opsi untuk membuat, mengelola, dan menghapus tanda tangan, memberikan Anda kontrol penuh atas alur kerja dokumen."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/python-net/esign/docx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/python-net/text/docx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/python-net/image/docx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/python-net/barcode/docx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/docx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/python-net/digital/docx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/python-net/stamp/docx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/python-net/search/docx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/python-net/verify/docx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/python-net/modify/docx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/python-net/delete/docx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Terapkan cap ke berbagai format dokumen"
    exclude: "DOCX"
    description: "Dengan API GroupDocs.Signature, Anda dapat menyisipkan cap kustom ke lebih dari 60 jenis file standar. Terapkan cap di mana saja dalam dokumen Anda, meningkatkan personalisasi dan pelacakan."
    items: 
          
        # format loop 1
        - name: "Stempel PDF"
          format: "PDF"
          link: "/signature/python-net/stamp/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Stempel DOCX"
          format: "DOCX"
          link: "/signature/python-net/stamp/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Stempel JPEG"
          format: "JPEG"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Stempel PPTX"
          format: "PPTX"
          link: "/signature/python-net/stamp/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Stempel XLSX"
          format: "XLSX"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---