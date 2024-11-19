



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:23
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Hasilkan kode QR untuk file JPEG menggunakan Python"
head_description: "Gunakan API GroupDocs.Signature untuk menghasilkan dan menyematkan kode QR dalam file JPEG. Tempatkan kode QR di halaman mana pun untuk menambahkan fungsionalitas tambahan."

############################# Header ############################
title: "Hasilkan kode QR untuk JPEG" 
description: "Ciptakan barcode 2D menggunakan data teks atau numerik dan terapkan pada berbagai halaman dan format, termasuk PDF, Word, Excel, dan lainnya dengan GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Uji coba gratis"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Jelajahi fitur-fitur GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) menawarkan beragam kemampuan, memungkinkan pengguna untuk menghasilkan dan menyematkan berbagai jenis tanda tangan di berbagai format dokumen utama. Baik itu PDF, Word, Excel, PowerPoint, atau gambar, tingkatkan dokumen Anda dengan tanda tangan Teks, Gambar, Barcode, Kode QR, Metadata, Digital, atau Stempel.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menghasilkan dan menyisipkan kode QR di JPEG"
    content: |
      [GroupDocs.Signature](/signature/python-net/) memungkinkan Anda membuat kode QR dalam format populer dan menempatkannya di halaman JPEG. Dengan dukungan lebih dari 10 jenis kode QR, Anda dapat mengintegrasikan fungsionalitas ini ke dalam aplikasi Python via .NET. Tingkatkan dokumen Anda dengan tanda tangan kode QR menggunakan produk kami.
      
      1. Dapatkan file atau stream JPEG tempat kode QR akan ditambahkan.
      2. Berikan teks yang diperlukan ke QrCodeSignOptions.
      3. Sesuaikan pengaturan visual seperti warna, posisi, dan ukuran.
      4. Simpan dokumen dengan kode QR yang disematkan.
   
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

            # Inisialisasi instance Signature baru dengan dokumen
            with sg.Signature('input.jpeg') as signature:

                # Gunakan QrCodeSignOptions untuk menyematkan kode QR ke dalam dokumen
                options = sg.QrCodeSignOptions("Text Content")

                # Tentukan jenis tanda tangan dan atur posisinya di halaman
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # Simpan dokumen dengan kode QR yang disematkan
                result = signature.Sign("output.jpeg", options)
        ```                 

############################# More features ############################
more_features:
  enable: true
  title: "Integrasi tanda tangan lengkap untuk dokumen"
  description: "Dengan API GroupDocs.Signature for Python via .NET, pengguna dapat menghasilkan, memodifikasi, mencari, memvalidasi, dan menghapus berbagai jenis tanda tangan, menyederhanakan alur kerja dokumen dengan presisi."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Terapkan berbagai jenis tanda tangan"
      content: "GroupDocs.Signature memungkinkan penerapan Tanda Tangan Teks, Gambar, Barcode, Kode QR, dan Stempel ke dokumen mana pun. Anda dapat menempatkan tanda tangan dengan tepat di halaman mana pun dan mengelola metadata dengan mudah. Lindungi dokumen Anda dari perubahan yang tidak sah dengan sertifikat digital."

    # feature loop
    - title: "Cari dan validasi tanda tangan"
      content: "Verifikasi tanda tangan dokumen untuk keaslian dan akurasi menggunakan alat validasi canggih. Dapatkan daftar terperinci dari semua tanda tangan yang disematkan dalam dokumen untuk pengawasan yang lebih baik."

    # feature loop
    - title: "Modifikasi tanda tangan yang ada"
      content: "Anda dapat memperbarui tanda tangan yang telah diterapkan sebelumnya dengan menyesuaikan konten, posisi, warna, ukuran, dan atribut lainnya agar sesuai dengan kebutuhan spesifik Anda."

    # feature loop
    - title: "Hapus tanda tangan dengan mudah"
      content: "Permudah manajemen dokumen dengan cepat menghapus tanda tangan yang tidak diinginkan. Baik itu sertifikat digital atau jenis tanda tangan lainnya, penghapusan dapat dilakukan dengan efisien."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sesuaikan Kode QR yang Dihasilkan"
      content: |
        Contoh ini menunjukkan cara menempatkan kode QR yang disesuaikan di halaman JPEG.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Ambil dokumen yang akan ditandatangani dan serahkan ke Signature
              with sg.Signature('input.jpeg') as signature:

                    # Konfigurasikan opsi kode QR dengan teks yang diperlukan
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # Atur posisi kode QR di halaman
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # Atur padding untuk tanda tangan
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Pilih warna untuk kode QR
                    options.ForeColor = sg.Color.Red

                    # Tentukan opsi font untuk pesan
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Atur warna latar belakang dan kuas untuk kode QR
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # Sisipkan kode QR ke dalam dokumen
                    result = signature.Sign("output.jpeg", options)
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
            link: "/examples/signature/formats/signature_qrcode.jpeg"
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
    title: "Jelajahi solusi tanda tangan kami"
    exclude: "qrcode"
    description: "Kami menawarkan berbagai jenis tanda tangan dan operasi untuk memenuhi kebutuhan dokumen Anda."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/python-net/esign/jpeg/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/python-net/text/jpeg/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/python-net/image/jpeg/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/python-net/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/python-net/stamp/jpeg/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/python-net/search/pdf/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/python-net/verify/pdf/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/python-net/modify/pdf/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/python-net/delete/pdf/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sisipkan kode QR dalam berbagai format dokumen"
    exclude: "JPEG"
    description: "Gunakan API Python via .NET untuk menyematkan kode QR ke dalam format dokumen standar industri mana pun. Simpan dan encode informasi penting ke dalam barcode 2D untuk pemindaian dan pengambilan data yang mudah."
    items: 
          
        # format loop 1
        - name: "QR-Code untuk PDF"
          format: "PDF"
          link: "/signature/python-net/qrcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "QR-Code untuk DOCX"
          format: "DOCX"
          link: "/signature/python-net/qrcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "QR-Code untuk JPEG"
          format: "JPEG"
          link: "/signature/python-net/qrcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "QR-Code untuk PPTX"
          format: "PPTX"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "QR-Code untuk XLSX"
          format: "XLSX"
          link: "/signature/python-net/qrcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---