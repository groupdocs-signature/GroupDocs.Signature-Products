



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:03
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Hasilkan kode QR dalam dokumen JPEG dengan JavaScript"
head_description: "Manfaatkan API GroupDocs.Signature untuk membuat dan mengintegrasikan barcode 2D ke dalam file JPEG. Tempatkan kode QR di halaman dokumen mana pun."

############################# Header ############################
title: "Buat kode QR untuk JPEG" 
description: "Ciptakan dan sematkan barcode 2D dengan konten yang dapat disesuaikan, termasuk teks dan data numerik, di berbagai jenis dokumen seperti PDF, Word, Excel, dan Gambar dengan GroupDocs.Signature for Node.js via Java."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba Gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Jelajahi kemampuan GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) menawarkan alat peningkatan dokumen yang canggih, memungkinkan pembuatan dan penyematan berbagai jenis tanda tangan, termasuk kode QR, ke dalam format file yang populer. Tandatangani dan amankan PDF, dokumen Word, spreadsheet Excel, presentasi PowerPoint, dan gambar dengan Teks, Gambar, Barcode, Kode QR, Metadata, Digital, dan tanda tangan Stempel.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk menghasilkan dan menyematkan kode QR di mana saja dalam JPEG"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) memungkinkan pembuatan kode QR dalam berbagai format yang banyak digunakan dan integrasinya ke dalam halaman JPEG. Mendukung lebih dari 10 jenis kode QR yang berbeda, solusi kami dapat dengan mulus diintegrasikan ke dalam aplikasi Node.js via Java, memperkaya mereka dengan kemampuan tanda tangan kode QR.
      
      1. Sediakan file atau stream JPEG untuk penandatanganan kode QR.
      2. Masukkan teks yang diinginkan ke dalam instance QrCodeSignOptions.
      3. Sesuaikan pengaturan visual seperti warna, posisi, ukuran, dll.
      4. Simpan dokumen yang berisi kode QR.
   
    code:
      platform: "nodejs-java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // Buat instance Signature dan berikan jalur dokumen
        const signature = new signatureLib.Signature('input.jpeg');

        // Manfaatkan QrCodeSignOptions untuk menyisipkan kode QR ke dalam dokumen
        // Create QR code sign options
        const options = new signatureLib.QrCodeSignOptions('Text Content');

        // Tentukan jenis tanda tangan dan penempatan di halaman
        options.setEncodeType(signatureLib.QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);
  
        // Simpan dokumen dengan kode QR yang baru ditambahkan
        signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Integrasi tanda tangan dan kode QR yang komprehensif"
  description: "Dengan API GroupDocs.Signature for Node.js via Java, Anda dapat mengelola berbagai jenis tanda tangan. Hasilkan, sesuaikan, verifikasi, cari, dan hapus tanda tangan dengan mudah di berbagai jenis dokumen, menawarkan fleksibilitas yang tiada tara untuk alur kerja Anda."
  image: "/img/signature/features_qrcode.webp" # 500x500 px
  image_description: "Fitur tanda tangan dan kode QR"
  features:
    # feature loop
    - title: "Tandatangan dokumen multi-format"
      content: "Tambahkan berbagai jenis tanda tangan, termasuk Teks, Gambar, Barcode, Kode QR, dan tanda tangan Stempel, ke dalam format dokumen yang didukung. Tempatkan di halaman mana pun dan kelola metadata dokumen. Pastikan keamanan dokumen melalui sertifikat digital untuk mencegah perubahan tanpa izin."

    # feature loop
    - title: "Validasi tanda tangan yang efisien"
      content: "Validasi semua tanda tangan dalam dokumen untuk memastikan memenuhi standar yang diperlukan. Dengan mudah mengambil dan meninjau tanda tangan melalui fungsi pencarian bawaan."

    # feature loop
    - title: "Pengeditan tanda tangan yang fleksibel"
      content: "Perbarui atau modifikasi tanda tangan yang ada, menyesuaikan aspek seperti konten, lokasi, ukuran, dan warna, sesuai kebutuhan dokumen Anda setelah tanda tangan awal."

    # feature loop
    - title: "Penghapusan tanda tangan yang mudah"
      content: "Hapus tanda tangan yang tidak diinginkan atau usang, termasuk sertifikat digital, dengan mudah. Pengendalian penuh atas manajemen tanda tangan memastikan dokumen yang rapi dan terorganisir."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menyesuaikan kode QR yang dihasilkan"
      content: |
        Contoh ini menjelaskan proses penambahan kode QR yang disesuaikan ke halaman JPEG.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Dapatkan dokumen yang akan ditandatangani dan berikan kepada Signature
          const signature = new signatureLib.Signature('input.jpeg');

          // Siapkan opsi kode QR dengan teks yang diperlukan
          const signOptions = new signatureLib.QrCodeSignOptions('Archived on July 11, 2019');

          // Tentukan posisi kode QR di halaman
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Tentukan padding tanda tangan
          const padding = new signatureLib.Padding();
          padding.setRight(20);
          padding.setTop(20);
          signOptions.setMargin(padding);

          // Pilih warna kode QR
          signOptions.setForeColor(signatureLib.Color.RED);

          // Tentukan opsi font untuk pesan yang menyertainya
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName("Comic Sans MS");
          signOptions.setFont(font);

          // Sesuaikan warna latar belakang dan kuas untuk kode QR
          const background = new signatureLib.Background();
          background.setColor(signatureLib.Color.GREEN);
          background.setTransparency(0.5);
          background.setBrush(new signatureLib.LinearGradientBrush(signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0));
          signOptions.setBackground(background);

          // Sematkan kode QR ke dalam dokumen
          signature.sign('output.jpeg', signOptions);
          ```
        platform: "nodejs-java"
        copy_title: "Salin"
        install:
          command: "npm i @groupdocs/groupdocs.signature"
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
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan NPM"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Pahami kemampuan utama kami"
    exclude: "qrcode"
    description: "Kami menyediakan berbagai format tanda tangan dan operasi yang disesuaikan dengan kebutuhan Anda"
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/nodejs-java/text/jpeg/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/nodejs-java/search/pdf/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/nodejs-java/verify/pdf/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/nodejs-java/modify/pdf/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Integrasikan kode QR dengan berbagai format file"
    exclude: "JPEG"
    description: "Manfaatkan API Node.js via Java untuk menghasilkan kode QR dan menyematkannya ke dalam berbagai format file yang banyak digunakan. Kemas data penting dalam barcode ini untuk integrasi yang mulus dan pengambilan di masa mendatang."
    items: 
          
        # format loop 1
        - name: "QR-Code untuk PDF"
          format: "PDF"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "QR-Code untuk DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/qrcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "QR-Code untuk JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/qrcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "QR-Code untuk PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/qrcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "QR-Code untuk XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---