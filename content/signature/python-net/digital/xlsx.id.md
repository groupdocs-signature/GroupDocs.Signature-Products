



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:19
draft: false
lang: id
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Buat tanda tangan digital untuk XLSX menggunakan Python"
head_description: "Tanda tangani dokumen XLSX secara digital menggunakan Python hanya dengan beberapa baris kode. Gunakan GroupDocs.Signature for Python via .NET untuk menandatangani berbagai format file."

############################# Header ############################
title: "Tanda tangani XLSX secara digital" 
description: "Pastikan keamanan dan keaslian dokumen Anda dengan menerapkan sertifikat digital melalui GroupDocs.Signature for Python via .NET. Solusi kami memungkinkan Anda untuk menandatangani dan melindungi dokumen Anda dengan alat yang kuat."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan secara gratis"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Signature for Python via .NET?"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) adalah alat penandatanganan komprehensif yang mendukung berbagai tugas pemrosesan dokumen. Ini memungkinkan Anda untuk menambahkan teks, gambar, sertifikat digital, dan cap pada lebih dari 60 format file—termasuk PDF, file MS Office, gambar, dan ZIP. Dengan GroupDocs.Signature for Python via .NET, Anda juga dapat mencari, memverifikasi, memperbarui, atau menghapus tanda tangan kapan saja diperlukan.

############################# Steps ############################
steps:
    enable: true
    title: "Cara melindungi XLSX dengan sertifikat digital di Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) membantu pengembang Python via .NET mengamankan file XLSX dengan menambahkan tanda tangan digital. Perkuat aplikasi bisnis Anda dengan fitur perlindungan dokumen yang tangguh.
      
      1. Muat file XLSX ke dalam kelas Signature.
      2. Terapkan sertifikat digital dan kata sandinya untuk mengamankan file.
      3. Secara opsional, tambahkan tampilan visual tanda tangan digital di halaman dokumen.
      4. Tanda tangani dokumen untuk mencegah perubahan yang tidak sah.
   
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

            # Gunakan Signature untuk menandatangani dokumen secara digital
            with sg.Signature('input.xlsx') as signature:

                # Masukkan sertifikat digital dan kata sandinya
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Secara opsional sesuaikan penampilan tanda tangan
                options.PageNumber = 1
                options.Left = 50
                options.Top = 50

                # Selesaikan dokumen dengan sertifikat digital
                result = signature.Sign("output.xlsx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan dan amankan dokumen dengan tanda tangan digital"
  description: "Perpustakaan GroupDocs.Signature for Python via .NET dirancang untuk menandatangani semua format file utama. Sederhanakan alur kerja Anda dengan menambahkan, memverifikasi, memperbarui, atau menghapus berbagai jenis tanda tangan dengan mudah."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tambahkan tanda tangan ke dokumen Anda"
      content: "Sisipkan tanda tangan teks, gambar, kode batang, kode QR, atau cap dengan tepat di mana saja dalam dokumen yang didukung. Anda juga dapat mengelola metadata tersembunyi, seperti EXIF pada gambar, untuk memastikan integritas dokumen dengan tanda tangan digital."

    # feature loop
    - title: "Verifikasi dan cari tanda tangan"
      content: "Setelah menandatangani, Anda dapat dengan mudah memverifikasi dokumen untuk memastikan pemrosesan yang benar. Ambil dan kelola semua tanda tangan dalam file Anda dengan kemampuan pencarian yang kuat."

    # feature loop
    - title: "Edit tanda tangan yang ada"
      content: "Sebagian besar tanda tangan dapat disesuaikan sepenuhnya. Anda dapat mengedit teks, memindahkan elemen, mengubah warna, menyesuaikan ukuran, dan lebih banyak lagi untuk memenuhi kebutuhan Anda."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "Solusi kami mendukung manajemen tanda tangan secara lengkap, memungkinkan Anda untuk menghapus tanda tangan, termasuk sertifikat digital, dari dokumen kapan pun diperlukan."
      
  code_samples:
    # code sample loop
    - title: "Lindungi dokumen dengan tanda tangan digital"
      content: |
        Pelajari cara mengamankan dokumen Anda dengan menerapkan tanda tangan digital untuk mencegah modifikasi yang tidak sah.
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # Muat dokumen yang akan ditandatangani
            with sg.Signature('input.xlsx') as signature:

                # Gunakan sertifikat digital yang valid dengan kata sandinya yang sesuai
                options = sg.DigitalSignOptions("certificate.pfx")
                options.Password = "1234567890"

                # Tambahkan informasi teks tambahan jika diperlukan
                options.Reason = "Security issue"
                options.Contact = "John Smith"
                options.Location = "Office D.W."

                # Sertakan gambar atau opsi lain untuk representasi visual dari tanda tangan
                options.ImageFilePath = "image.png"
                options.AllPages = True
                options.VerticalAlignment = sg.VerticalAlignment.Center
                options.HorizontalAlignment = sg.HorizontalAlignment.Left
                options.Width = 60
                options.Height = 80

                options.Margin = sg.Padding()
                options.Margin.Bottom = 10
                options.Margin.Right = 10

                # Simpan dokumen yang ditandatangani di lokasi yang aman
                result = signature.Sign("output.xlsx", options)
        ```
        {{< /landing/code >}}


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
    title: "Jelajahi fitur utama kami"
    exclude: "digital"
    description: "Kami menawarkan berbagai opsi tanda tangan dan operasi dokumen yang kuat."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/python-net/esign/xlsx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/python-net/text/xlsx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/python-net/image/xlsx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/python-net/digital/xlsx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/python-net/stamp/xlsx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/python-net/search/xlsx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/python-net/verify/xlsx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/python-net/modify/xlsx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/python-net/delete/xlsx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tanda tangani dokumen dalam berbagai format"
    exclude: "XLSX"
    description: "Dengan API Python via .NET, Anda dapat memproses lebih dari 60 format berbeda, menambahkan tanda tangan, menerapkan sertifikat digital untuk keamanan, dan mengelola tanda tangan di berbagai halaman."
    items: 
          
        # format loop 1
        - name: "Lindungi PDF"
          format: "PDF"
          link: "/signature/python-net/digital/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Lindungi DOCX"
          format: "DOCX"
          link: "/signature/python-net/digital/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Lindungi PPTX"
          format: "PPTX"
          link: "/signature/python-net/digital/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Lindungi XLSX"
          format: "XLSX"
          link: "/signature/python-net/digital/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---