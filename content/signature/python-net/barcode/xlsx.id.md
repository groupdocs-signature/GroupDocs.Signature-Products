



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:26
draft: false
lang: id
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Menyematkan kode batang dalam XLSX dengan Python"
head_description: "Tambahkan tanda tangan kode batang dengan efisien ke dokumen XLSX hanya dengan beberapa baris di Python. GroupDocs.Signature memberikan solusi penandatanganan yang mulus untuk berbagai format dokumen."

############################# Header ############################
title: "Buat kode batang untuk XLSX" 
description: "Dengan GroupDocs.Signature for Python via .NET, Anda dapat menempatkan kode batang di dokumen bisnis Anda di mana pun diperlukan. Solusi kami menawarkan berbagai opsi untuk kustomisasi tanda tangan kode batang."
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
    title: "Tentang GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) adalah alat penandatanganan dokumen yang kuat dan mendukung berbagai jenis tanda tangan, termasuk teks, gambar, kode batang, sertifikat digital, dan cap. Kompatibel dengan lebih dari 60 format file, seperti PDF, MS Office, gambar, ZIP, dan banyak lagi, alat ini tidak hanya memungkinkan Anda untuk menerapkan tanda tangan tetapi juga mencari, memverifikasi, memodifikasi, atau menghapusnya sesuai kebutuhan.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menghasilkan dan menyisipkan kode batang dalam XLSX"
    content: |
      [GroupDocs.Signature](/signature/python-net/) memungkinkan Anda untuk menghasilkan dan menyematkan kode batang dalam dokumen XLSX dengan cepat dan efisien. Mendukung lebih dari 60 format kode batang, aplikasi Python via .NET dapat menambahkan fungsi penandatanganan kode batang dengan mengintegrasikan pustaka kami.
      
      1. Sediakan file atau stream XLSX untuk pemrosesan.
      2. Tetapkan teks kode batang ke objek BarcodeSignOptions.
      3. Sesuaikan opsi kode batang, seperti posisi dan ukuran.
      4. Simpan dokumen dengan kode batang yang disematkan.
   
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

            # Inisialisasi objek Signature dengan jalur dokumen
            with sg.Signature('input.xlsx') as signature:

                # Gunakan BarcodeSignOptions untuk menambahkan kode batang ke dokumen
                options = sg.BarcodeSignOptions('Business data')

                # Tentukan jenis kode batang dan sesuaikan propertinya
                options.EncodeType = sg.BarcodeTypes.Code128
                options.Left = 50
                options.Top = 150

                # Simpan dokumen yang sudah ditandatangani
                result = signature.Sign('output.xlsx', options)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan dokumen Anda dengan fitur tanda tangan canggih"
  description: "Perpustakaan GroupDocs.Signature for Python via .NET menyediakan solusi komprehensif untuk menandatangani dan memproses dokumen dalam format yang umum digunakan. Anda dapat menambahkan, memodifikasi, memverifikasi, atau menghapus berbagai jenis tanda tangan sesuai kebutuhan."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen yang fleksibel"
      content: "Tandatangani halaman mana pun di dokumen yang didukung dengan teks, gambar, kode batang, kode QR, atau cap. Tambahkan metadata tersembunyi seperti data EXIF di gambar dan pastikan perlindungan konten dengan sertifikat digital untuk mencegah perubahan yang tidak sah."

    # feature loop
    - title: "Cari dan verifikasi tanda tangan"
      content: "Alat kami memastikan integritas dokumen Anda dengan memungkinkan verifikasi tanda tangan. Anda juga dapat mengambil daftar lengkap semua tanda tangan dalam sebuah dokumen untuk manajemen yang mudah."

    # feature loop
    - title: "Edit tanda tangan dengan mudah"
      content: "Modifikasi tanda tangan yang ada dengan usaha minimal. Sesuaikan teks, ubah posisi elemen, atau ganti warna agar sesuai dengan kebutuhan dokumen Anda."

    # feature loop
    - title: "Hapus tanda tangan tanpa usaha"
      content: "Dengan fungsionalitas CRUD penuh, GroupDocs.Signature for Python via .NET memudahkan penghapusan tanda tangan yang tidak diinginkan atau usang dari dokumen Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Buat dan tempatkan tanda tangan kode batang"
      content: |
        Contoh ini menunjukkan bagaimana cara menyisipkan kode batang kustom ke dalam dokumen XLSX.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Sediakan dokumen yang akan ditandatangani
              with sg.Signature('input.xlsx') as signature:

                  # Tetapkan teks kode batang dan opsi tanda tangan
                  options = sg.BarcodeSignOptions('Accepted')
                  options.EncodeType = sg.BarcodeTypes.Code39FullASCII

                  # Pilih posisi untuk kode batang di halaman
                  options.VerticalAlignment = sg.VerticalAlignment.Top
                  options.HorizontalAlignment = sg.HorizontalAlignment.Left

                  # Tetapkan jarak antara kode batang dan tepi halaman
                  options.Margin = sg.Padding()
                  options.Margin.Top = 180
                  options.Margin.Right = 20

                  # Tentukan warna batang kode batang
                  options.ForeColor = sg.Color.Red

                  # Pilih gaya font untuk pesan kode batang
                  options.Font = sg.SignatureFont()
                  options.Font.Size = 12
                  options.Font.FamilyName = 'Arial'

                  # Setel posisi teks pesan
                  options.CodeTextAlignment = sg.CodeTextAlignment.Above

                  # Tandatangani dan simpan dokumen
                  result = signature.Sign('output.xlsx', options)
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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Jelajahi fitur utama kami"
    exclude: "barcode"
    description: "Kami menawarkan berbagai pilihan tanda tangan dan operasi untuk kebutuhan dokumen Anda."
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
    title: "Tandatangani dokumen dalam berbagai format"
    exclude: "XLSX"
    description: "API Python via .NET mendukung penandatanganan lebih dari 60 format file, memungkinkan Anda menambahkan berbagai jenis tanda tangan ke halaman mana pun atau lokasi tertentu di dalam dokumen Anda."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/signature/python-net/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/signature/python-net/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke JPEG"
          format: "JPEG"
          link: "/signature/python-net/barcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/signature/python-net/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/signature/python-net/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---