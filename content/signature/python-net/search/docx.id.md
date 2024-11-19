



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:33
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Python via .NET"
platform_tag: "python-net"

############################# Head ############################
head_title: "Pencarian tanda tangan elektronik untuk DOCX menggunakan Python"
head_description: "Manfaatkan API GroupDocs.Signature for Python via .NET untuk mencari tanda tangan elektronik yang disematkan dalam format seperti PDF, Word, Excel, Presentasi, dan Gambar."

############################# Header ############################
title: "Pencarian tanda tangan digital DOCX" 
description: "Ekstrak daftar lengkap tanda tangan elektronik dari berbagai format, termasuk PDF, Word, Excel, Presentasi, dan Gambar, dengan kekuatan GroupDocs.Signature for Python via .NET."
subtitle: "GroupDocs.Signature for Python via .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh sekarang"
      link: "https://releases.groupdocs.com/signature/python-net/"
      
############################# About ############################
about:
    enable: true
    title: "Maksimalkan potensi GroupDocs.Signature for Python via .NET"
    link: "/signature/python-net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Python via .NET](/signature/python-net/) menawarkan kemampuan lanjutan untuk menandatangani dan mengelola dokumen digital. Dengan dukungan untuk lebih dari 60 format file, termasuk PDF, dokumen Office, Gambar, dan file ZIP, Anda dapat menambahkan, mencari, memverifikasi, memodifikasi, atau menghapus tanda tangan seperti teks, gambar, kode batang, kode QR, sertifikat digital, dan stempel.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mencari tanda tangan dalam DOCX menggunakan Python"
    content: |
      [GroupDocs.Signature](/signature/python-net/) menyediakan mesin yang kuat untuk mendeteksi tanda tangan digital dalam file DOCX. Pengembang Python via .NET dapat dengan mudah meningkatkan aplikasi mereka dengan fungsionalitas ini.
      
      1. Berikan jalur file DOCX untuk pencarian tanda tangan.
      2. Gunakan SearchOptions untuk mempersempit kriteria pencarian.
      3. Panggil metode Search untuk mengambil hasil.
      4. Tinjau daftar tanda tangan yang teridentifikasi.
   
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

            # Inisialisasi objek Signature dengan jalur file dokumen
            with sg.Signature('input.docx') as signature:

                # Buat instance TextSearchOptions untuk mencari di semua halaman
                options = sg.TextSearchOptions()
                options.AllPages = True

                # Jalankan pencarian untuk menemukan tanda tangan berbasis teks dalam dokumen
                signatures = signature.Search(options)
                print("\nSource document contains following text signature(s).")

                # Kompilasi daftar tanda tangan yang ditemukan untuk ditinjau secara mendetail
                for textSignature in signatures:
                    print("\nFound Text signature at page ", textSignature.PageNumber)
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Platform tanda tangan dokumen yang lengkap"
  description: "Rasakan solusi tanda tangan yang kuat dan kaya fitur yang mengamankan dokumen Anda dengan berbagai jenis tanda tangan, meliputi berbagai format file."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Cari dan kelola tanda tangan"
  features:
    # feature loop
    - title: "Tandatangani dan amankan dokumen bisnis"
      content: "Tambahkan tanda tangan elektronik di mana saja dalam dokumen. GroupDocs.Signature mendukung berbagai jenis tanda tangan, termasuk teks, gambar, kode batang, metadata, stempel, dan sertifikat digital, memastikan keaslian dan keamanan dokumen."

    # feature loop
    - title: "Manajemen tanda tangan yang komprehensif"
      content: "Setelah dokumen ditandatangani, gunakan fitur pencarian untuk menemukan semua tanda tangan yang disematkan. Anda dapat memodifikasi atau menghapus tanda tangan sesuai kebutuhan, memberikan Anda kendali penuh atas integritas dokumen."

    # feature loop
    - title: "Pastikan integritas dokumen"
      content: "Gunakan alat lanjutan untuk mengelola metadata tersembunyi dalam dokumen. Tambahkan atau hapus metadata, dan terapkan sertifikat digital untuk melindungi dokumen Anda dari perubahan yang tidak sah, memastikan keasliannya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cari tanda tangan gambar"
      content: |
        Contoh ini menunjukkan cara menemukan tanda tangan gambar dalam dokumen tertentu.
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # Berikan dokumen sumber ke konstruktor
              with sg.Signature('input.docx') as signature:

                    # Cari tanda tangan berbasis teks
                    signatures = signature.Search(sg.SignatureType.Image)
                    print("\nSource document contains following image signature(s).")

                    # Tampilkan properti rinci dari tanda tangan yang teridentifikasi
                    for imageSignature in signatures:
                        print("\nFound image signature at page ", imageSignature.PageNumber)
          ```
        platform: "python-net"
        copy_title: "Salin"
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
    title: "Fitur inti"
    exclude: "search"
    description: "API kami menyediakan fleksibilitas yang luas, memungkinkan pengguna untuk menandatangani dokumen dan melakukan operasi pasca-tanda tangan seperti mencari, memverifikasi, dan mengedit tanda tangan."
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
    title: "Ekstrak tanda tangan dari berbagai format file"
    exclude: "DOCX"
    description: "API GroupDocs.Signature for Python via .NET memungkinkan Anda untuk mengekstrak dan mengelola tanda tangan dari berbagai format dokumen. Dengan mudah ambil tanda tangan yang disematkan dari jenis file utama untuk analisis atau pemrosesan lebih lanjut."
    items: 
          
        # format loop 1
        - name: "Cari tanda tangan dalam PDF"
          format: "PDF"
          link: "/signature/python-net/search/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Temukan tanda tangan dalam DOCX"
          format: "DOCX"
          link: "/signature/python-net/search/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Temukan tanda tangan dalam PPTX"
          format: "PPTX"
          link: "/signature/python-net/search/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Cari tanda tangan dalam XLSX"
          format: "XLSX"
          link: "/signature/python-net/search/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---