



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:51:53
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Sisipkan tanda tangan gambar ke dalam file JPEG dengan Python"
head_description: "Sisipkan tanda tangan gambar dalam dokumen JPEG untuk Python hanya dengan beberapa baris kode. Manfaatkan API GroupDocs.Signature for Python via .NET untuk menambahkan tanda tangan berbasis gambar secara mulus."

############################# Header ############################
title: "Tambahkan tanda tangan gambar ke JPEG" 
description: "Gunakan GroupDocs.Signature for Python via .NET untuk menggabungkan tanda tangan gambar ke berbagai format dokumen kantor, termasuk PDF, Word, Excel, dan file gambar. Menambahkan gambar tanda tangan manajer Anda meningkatkan profesionalisme, memperkuat dampak visual dan keaslian dokumen."
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
    title: "Jelajahi GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) menyediakan opsi yang fleksibel untuk menyematkan tanda tangan gambar di mana saja dalam dokumen bisnis Anda. Permudah alur kerja dengan menambahkan gambar ke PDF, dokumen Word, lembar Excel, presentasi PowerPoint, dan format gambar populer menggunakan perpustakaan kami yang kuat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menyisipkan tanda tangan gambar ke dalam file JPEG menggunakan Python"
    content: |
      Gunakan [GroupDocs.Signature](/signature/python-net/) untuk memberikan aplikasi Python via .NET kemampuan untuk menambahkan tanda tangan gambar dengan akurat di mana saja dalam dokumen JPEG. Tingkatkan produk Anda dengan mengintegrasikan solusi kami.
      
      1. Buat instance Signature dengan dokumen JPEG.
      2. Konfigurasi ImageSignOptions dengan gambar yang diinginkan untuk tanda tangan.
      3. Posisikan gambar dengan tepat di lokasi pilihan Anda pada dokumen.
      4. Simpan dokumen yang telah ditandatangani ke lokasi yang ditentukan.
   
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
            with sg.Signature('input.jpeg') as signature:

                # Siapkan ImageSignOptions dengan gambar yang dipilih untuk tanda tangan
                options = sg.ImageSignOptions("company_logo.jpg")

                # Posisikan gambar di sudut kiri atas setiap halaman
                options.AllPages = True
                options.Left = 100
                options.Top = 200
                
                # Simpan dokumen yang telah ditandatangani
                result = signature.Sign("output.jpeg", options)
        ```          

############################# More features ############################
more_features:
  enable: true
  title: "Fitur tanda tangan dokumen yang komprehensif"
  description: "API kami mendukung berbagai fungsi tanda tangan. Anda dapat menambahkan, memperbarui, menghapus, mencari, dan memvalidasi berbagai jenis tanda tangan, termasuk tanda tangan berbasis gambar."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Integrasi Tanda Tangan Gambar"
  features:
    # feature loop
    - title: "Sisipkan gambar ke dalam dokumen kantor"
      content: "Sisipkan tanda tangan elektronik dan gambar di setiap tempat yang dipilih dalam dokumen. Tingkatkan dokumen Anda dengan gambar, kode batang, teks, metadata, atau sertifikat digital untuk meningkatkan fungsionalitas dan keamanan."

    # feature loop
    - title: "Pencarian dan validasi tanda tangan"
      content: "Pastikan integritas dokumen dengan memverifikasi keaslian tanda tangan. Dapatkan daftar rinci semua tanda tangan dalam dokumen dan evaluasi properti individualnya."

    # feature loop
    - title: "Edit tanda tangan yang ada"
      content: "Perbarui konten, tampilan, ukuran, atau posisi tanda tangan dalam dokumen Anda untuk memenuhi kebutuhan yang berubah."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "API kami menyediakan kontrol penuh, memungkinkan Anda untuk menghapus tanda tangan dari sebagian besar format file yang didukung kapan pun diperlukan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tingkatkan dokumen dengan tanda tangan gambar"
      content: |
        Pelajari cara menyisipkan tanda tangan gambar dalam dokumen bisnis Anda untuk memperkaya konten.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Pilih dokumen yang akan ditandatangani
              with sg.Signature('input.jpeg') as signature:

                    # Siapkan opsi gambar dengan jalur file gambar
                    options = sg.ImageSignOptions("manager_signature.jpg")

                    # Tentukan ukuran tanda tangan gambar
                    options.Width = 100
                    options.Height = 100

                    # Posisikan gambar di sudut kanan bawah halaman
                    options.VerticalAlignment = sg.VerticalAlignment.Bottom
                    options.HorizontalAlignment = sg.HorizontalAlignment.Right

                    # Terapkan padding dari tepi halaman sesuai kebutuhan
                    options.Margin = sg.Padding()
                    options.Margin.Bottom = 120
                    options.Margin.Right = 120

                    # Opsional, tambahkan batas di sekitar gambar
                    options.Border = sg.Border()
                    options.Border.Visible = True
                    options.Border.Color = sg.Color.OrangeRed
                    options.Border.DashStyle = sg.DashStyle.DashDotDot
                    options.Border.Weight = 5

                    # Putar gambar untuk memastikan penyelarasan yang tepat
                    options.RotationAngle = 45

                    # Simpan dokumen yang telah diperbarui
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
            link: "/examples/signature/formats/signature_image.jpeg"
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
    title: "Jelajahi fitur kami"
    exclude: "image"
    description: "Temukan berbagai jenis tanda tangan dan operasi yang ditawarkan platform kami."
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
    title: "Sisipkan gambar dalam berbagai format file"
    exclude: "JPEG"
    description: "Gunakan API Python via .NET untuk menyisipkan gambar ke dalam berbagai format dokumen. Atur ulang ukuran, posisi, pilih halaman tertentu, dan terapkan tanda tangan berbasis gambar, memberi Anda kontrol penuh atas tata letak dokumen Anda."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan PDF dengan Gambar"
          format: "PDF"
          link: "/signature/python-net/image/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan DOCX dengan Gambar"
          format: "DOCX"
          link: "/signature/python-net/image/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan JPEG dengan Gambar"
          format: "JPEG"
          link: "/signature/python-net/image/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan PPTX dengan Gambar"
          format: "PPTX"
          link: "/signature/python-net/image/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan XLSX dengan Gambar"
          format: "XLSX"
          link: "/signature/python-net/image/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---