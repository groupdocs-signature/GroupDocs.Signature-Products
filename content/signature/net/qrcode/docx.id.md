



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:20
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Hasilkan kode QR untuk file DOCX menggunakan C#"
head_description: "Manfaatkan API GroupDocs.Signature untuk menghasilkan kode QR untuk file DOCX. Madalkan kode QR pada halaman mana pun untuk meningkatkan fungsionalitas."

############################# Header ############################
title: "Hasilkan kode QR untuk DOCX" 
description: "Buat kode batang 2D menggunakan data teks atau numerik dan terapkan di berbagai halaman dan format, termasuk PDF, Word, Excel, dan lainnya, melalui GroupDocs.Signature for .NET."
subtitle: "GroupDocs.Signature for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Mulai uji coba gratis Anda"
      link: "https://releases.groupdocs.com/signature/net/"
      
############################# About ############################
about:
    enable: true
    title: "Temukan kemampuan GroupDocs.Signature for .NET"
    link: "/signature/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for .NET](/signature/net/) menawarkan berbagai fitur yang luas, memberdayakan pengguna untuk menghasilkan dan menyematkan berbagai jenis tanda tangan di berbagai format dokumen terkemuka. Apakah itu PDF, dokumen Word, lembar Excel, presentasi PowerPoint, atau file gambar, Anda dapat meningkatkan dokumen Anda dengan Teks, Gambar, Barcode, Kode QR, Metadata, Digital, dan Tanda Tangan Stempel.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menghasilkan dan menyisipkan kode QR di mana saja dalam DOCX"
    content: |
      [GroupDocs.Signature](/signature/net/) memfasilitasi penghasilan kode QR dalam berbagai format populer dan penempatannya pada halaman DOCX. Mendukung lebih dari 10 jenis kode QR, perpustakaan kami dapat diintegrasikan dengan mulus ke dalam aplikasi .NET. Tingkatkan dokumen Anda dengan tanda tangan kode QR menggunakan produk kami.
      
      1. Dapatkan file DOCX atau aliran yang akan ditandatangani dengan kode QR.
      2. Sediakan teks yang diperlukan untuk QrCodeSignOptions.
      3. Sesuaikan parameter visual seperti warna, posisi, ukuran, dll.
      4. Simpan dokumen dengan kode QR yang disematkan.
   
    code:
      platform: "net"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command: "dotnet add package GroupDocs.Signature"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/net/"
          
      content: |
        ```csharp {style=abap}
        // Inisialisasi instance Signature baru dengan dokumen
        using (Signature signature = new Signature("input.docx"))
        {
            // Gunakan QrCodeSignOptions untuk menyematkan kode QR ke dalam dokumen
            QrCodeSignOptions options = new QrCodeSignOptions("Text Content")
                {
                    // Tentukan jenis tanda tangan dan tetapkan posisinya di halaman
                    EncodeType = QrCodeTypes.QR,
                    Left = 50,
                    Top = 150
                };

            // Simpan dokumen dengan kode QR yang terintegrasi
            SignResult result = signature.Sign("output.docx", options);
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integrasi tanda tangan komprehensif untuk dokumen"
  description: "Dengan API GroupDocs.Signature for .NET, pengguna dapat menghasilkan, memodifikasi, mencari, memvalidasi, dan menghapus beragam jenis tanda tangan dengan presisi yang tiada tara, menyederhanakan alur kerja dokumen."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tanda tangan dokumen dengan berbagai jenis tanda tangan"
      content: "GroupDocs.Signature memungkinkan penerapan Teks, Gambar, Barcode, Kode QR, dan tanda tangan Stempel pada format dokumen mana pun. Tanda tangan dapat ditempatkan dengan tepat di halaman mana pun, dan metadata dapat dikelola dengan mulus melalui tanda tangan metadata. Lindungi integritas dokumen Anda dengan mengintegrasikan sertifikat digital yang mencegah perubahan yang tidak sah."

    # feature loop
    - title: "Pencarian dan validasi tanda tangan"
      content: "Verifikasi keaslian dan akurasi tanda tangan dokumen melalui proses validasi yang canggih. Dengan mudah ambil daftar rinci semua tanda tangan yang disematkan dalam sebuah dokumen untuk pengawasan yang komprehensif."

    # feature loop
    - title: "Modifikasi tanda tangan yang dapat disesuaikan"
      content: "Perbarui dan sempurnakan tanda tangan yang sudah diterapkan sebelumnya dengan menyesuaikan konten, penempatan, warna, ukuran, dan atribut lainnya agar sesuai dengan kebutuhan spesifik Anda."

    # feature loop
    - title: "Penghapusan tanda tangan yang efisien"
      content: "Permudah manajemen dokumen Anda dengan menghapus tanda tangan yang tidak diinginkan secara programatik. Baik berkaitan dengan sertifikat digital atau jenis tanda tangan lainnya, penghapusan dapat dilakukan dengan cepat dan efektif."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menghasilkan kode QR dengan berbagai opsi?"
      content: |
        Contoh ini menunjukkan bagaimana menempatkan kode QR yang disesuaikan pada halaman DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Ambil dokumen yang akan ditandatangani dan berikan kepada Signature
          using (Signature signature = new Signature("input.docx"))
          {
              // Konfigurasi opsi kode QR dengan teks yang diperlukan
              QrCodeSignOptions options = new QrCodeSignOptions("Archived on July 11, 2019")
              {
                    // Tentukan posisi relatif dari kode QR di halaman
                    VerticalAlignment = Domain.VerticalAlignment.Top,
                    HorizontalAlignment = Domain.HorizontalAlignment.Right,

                    // Atur padding tanda tangan
                    Margin = new Padding() { Top = 20, Right = 20 },

                    // Tentukan warna kode QR
                    ForeColor = Color.Red,

                    // Tentukan opsi font untuk pesan
                    Font = new SignatureFont { Size = 12, FamilyName = "Comic Sans MS" },

                    // Kustomisasi warna latar belakang dan kuas untuk kode QR
                    Background = new Background()
                    {
                        Color = Color.LimeGreen,
                        Transparency = 0.5,
                        Brush = new Domain.Extensions.LinearGradientBrush(Color.LimeGreen, Color.DarkGreen)
                    }
              };

              // Sisipkan kode QR ke dalam dokumen
              SignResult result = signature.Sign("output.docx", options);
          }
          ```
        platform: "net"
        copy_title: "Salin"
        install:
          command: "dotnet add package GroupDocs.Signature"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/signature/formats/signature_qrcode.docx"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan Nuget"
      link: "https://releases.groupdocs.com/signature/net/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Pelajari tentang solusi tanda tangan kami"
    exclude: "qrcode"
    description: "Kami dengan bangga menghadirkan berbagai jenis tanda tangan dan fitur operasional"
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/net/esign/docx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/net/text/docx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/net/image/docx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/net/barcode/docx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/net/qrcode/docx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/net/digital/docx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/net/stamp/docx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/net/search/docx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/net/verify/docx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/net/modify/docx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/net/delete/docx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Hasilkan kode QR untuk format dokumen lainnya"
    exclude: "DOCX"
    description: "Tingkatkan semua format file standar industri dengan kemampuan untuk menyematkan kode QR melalui API .NET. Simpan dan enkode informasi penting ke dalam barcode 2D untuk pemindaian dan pengambilan data yang mulus."
    items: 
          
        # format loop 1
        - name: "QR-Code untuk PDF"
          format: "PDF"
          link: "/signature/net/qrcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "QR-Code untuk DOCX"
          format: "DOCX"
          link: "/signature/net/qrcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "QR-Code untuk JPEG"
          format: "JPEG"
          link: "/signature/net/qrcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "QR-Code untuk PPTX"
          format: "PPTX"
          link: "/signature/net/qrcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "QR-Code untuk XLSX"
          format: "XLSX"
          link: "/signature/net/qrcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---