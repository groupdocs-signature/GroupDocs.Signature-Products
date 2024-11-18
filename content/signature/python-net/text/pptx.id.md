



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:56
draft: false
lang: id
format: Pptx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Tambahkan tanda tangan teks ke PPTX menggunakan Python"
head_description: "Manfaatkan API Python untuk menyematkan tanda tangan berbasis teks dalam file PPTX, mendukung format seperti PDF, Word, Excel, PowerPoint, gambar, dan ZIP."

############################# Header ############################
title: "Tambahkan tanda tangan teks ke PPTX" 
description: "Integrasikan tanda tangan teks kustom ke dalam dokumen Anda menggunakan GroupDocs.Signature for Python via .NET. Sederhanakan alur kerja Anda dengan opsi kustomisasi tanda tangan yang fleksibel."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba gratis hari ini"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Jelajahi kekuatan GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) menawarkan platform komprehensif untuk menyematkan tanda tangan teks yang dapat disesuaikan, membuat alur kerja dokumen lebih lancar. Personalisasi konten dan penampilan tanda tangan di seluruh dokumen untuk meningkatkan efisiensi dan pengelolaan dokumen.

############################# Steps ############################
steps:
    enable: true
    title: "Cara membuat tanda tangan teks PPTX dengan Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) memungkinkan integrasi tanda tangan teks dalam file PPTX di aplikasi Python via .NET. Tambahkan fungsionalitas dengan cepat ke produk Anda dengan solusi ini.
      
      1. Sediakan dokumen PPTX kepada konstruktor Signature.
      2. Buat TextSignOptions dengan teks tanda tangan Anda.
      3. Tetapkan properti visual tanda tangan.
      4. Sisipkan tanda tangan ke halaman-halaman yang diinginkan dari dokumen.
   
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

            # Inisialisasi Signature dengan jalur dokumen
            with sg.Signature('input.pptx') as signature:

                # Siapkan TextSignOptions dengan teks tanda tangan yang diinginkan
                options = sg.TextSignOptions("Approved")

                # Pilih warna dan font untuk tanda tangan
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # Terapkan tanda tangan teks ke dokumen
                result = signature.Sign("output.pptx", options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Manajemen tanda tangan teks yang lengkap"
  description: "GroupDocs.Signature for Python via .NET membantu Anda mengelola alur kerja dokumen dengan menambahkan tanda tangan teks kustom ke format populer. Kontrol dengan mudah tampilan, penempatan, dan konten tanda tangan sesuai kebutuhan Anda."
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "Temukan Fitur GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangan dokumen yang fleksibel"
      content: "Tambahkan berbagai jenis tanda tangan—teks, gambar, barcode, kode QR, dan cap—ke setiap halaman dokumen. Gunakan metadata untuk menyertakan informasi tersembunyi dan amankan file Anda dengan sertifikat digital."

    # feature loop
    - title: "Verifikasi dan cari tanda tangan"
      content: "Gunakan alat canggih untuk memeriksa integritas dokumen yang ditandatangani. Cari dan analisis semua tanda tangan dalam file untuk validasi lebih lanjut."

    # feature loop
    - title: "Edit atau hapus tanda tangan"
      content: "Perbarui dengan mudah konten, penampilan, atau penempatan tanda tangan yang ada. Hapus tanda tangan yang kedaluwarsa untuk menjaga dokumen Anda tetap terbaru."

    # feature loop
    - title: "Tanda tangan teks khusus"
      content: "Terapkan tanda tangan teks khusus dokumen, seperti watermark untuk file Word atau cap untuk PDF, menambahkan tingkat kontrol dan kustomisasi yang lebih."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tambahkan tanda tangan teks ke dokumen"
      content: |
        Pelajari cara menyematkan tanda tangan teks ke dalam dokumen untuk memperlancar proses Anda.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Pilih dokumen untuk ditandatangani
              with sg.Signature('input.pptx') as signature:

                    # Siapkan opsi teks dengan konten yang diinginkan
                    options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                    # Tentukan ukuran dan penempatan tanda tangan
                    options.Left = 100
                    options.Top = 180
                    options.Width = 230
                    options.Height = 30

                    # Tentukan jarak dari tepi halaman
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # Pilih warna teks dan gaya font
                    options.ForeColor = sg.Color.Red
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # Tambahkan garis batas di sekitar tanda tangan teks
                    options.Border = sg.Border()
                    options.Border.Color = sg.Color.Red
                    options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                    options.Border.Transparency = 0.5
                    options.Border.Visible = True
                    options.Border.Weight = 2

                    # Sesuaikan latar belakang jika perlu
                    options.Background = sg.Background()
                    options.Background.Color = sg.Color.Yellow
                    options.Background.Transparency = 0.8

                    # Opsional simpan tanda tangan sebagai gambar untuk kompatibilitas
                    options.SignatureImplementation = sg.TextSignatureImplementation.Image

                    # Simpan dokumen dengan tanda tangan yang disematkan
                    result = signature.Sign("output.pptx", options)
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
            link: "/examples/signature/formats/signature_text.pptx"
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
    title: "Fitur tanda tangan tingkat lanjut"
    exclude: "text"
    description: "API kami mendukung manajemen siklus hidup lengkap untuk tujuh jenis tanda tangan, memungkinkan Anda untuk membuat, mengelola, memverifikasi, dan menyesuaikan tanda tangan Anda."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/python-net/esign/pptx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/python-net/text/pptx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/python-net/image/pptx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/python-net/barcode/pptx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/python-net/qrcode/pptx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/python-net/digital/pptx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/python-net/stamp/pptx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/python-net/search/pptx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/python-net/verify/pptx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/python-net/modify/pptx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/python-net/delete/pptx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sisipkan tanda tangan teks dalam berbagai format"
    exclude: "PPTX"
    description: "Dengan API Python via .NET, Anda dapat menambahkan tanda tangan teks ke berbagai dokumen Office, memberi Anda kontrol penuh atas siklus hidup dokumen dan meningkatkan keamanan."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Teks PDF"
          format: "PDF"
          link: "/signature/python-net/text/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Teks DOCX"
          format: "DOCX"
          link: "/signature/python-net/text/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Teks JPEG"
          format: "JPEG"
          link: "/signature/python-net/text/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Teks PPTX"
          format: "PPTX"
          link: "/signature/python-net/text/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Teks XLSX"
          format: "XLSX"
          link: "/signature/python-net/text/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---