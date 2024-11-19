



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:30
draft: false
lang: id
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tandai XLSX dengan tanda tangan elektronik di JavaScript"
head_description: "Manfaatkan kemampuan API JavaScript untuk menandatangani dan melindungi file XLSX secara digital, termasuk PDF, dokumen Word, lembar Excel, presentasi, dan format gambar."

############################# Header ############################
title: "Tandai file XLSX secara elektronik" 
description: "Gunakan GroupDocs.Signature for Node.js via Java untuk menyisipkan berbagai tanda tangan digital ke dalam dokumen Anda, memastikan integritas data dan kepatuhan untuk file seperti PDF, Word, Excel, presentasi, dan format gambar."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh sekarang gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Ikhtisar API GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) menawarkan serangkaian alat yang kuat untuk menambahkan tanda tangan elektronik. Dengan API yang intuitif, Anda dapat dengan mudah menandatangani, mencari, memverifikasi, memodifikasi, dan menghapus tanda tangan dari berbagai jenis file tanpa memerlukan perangkat lunak eksternal. Ini mendukung proses penandatanganan yang mulus untuk PDF, dokumen Word, spreadsheet Excel, slide PowerPoint, dan berbagai format gambar.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk menandatangani XLSX menggunakan JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) menyederhanakan proses penambahan tanda tangan kustom ke file XLSX. Pengembang Node.js via Java dapat secara mulus mengintegrasikan fungsionalitas penandatanganan ke dalam aplikasi mereka.
      
      1. Muat dokumen XLSX ke dalam instance Signature.
      2. Konfigurasi SignOptions untuk menentukan atribut tanda tangan.
      3. Sesuaikan properti seperti ukuran, warna, dan konten sesuai kebutuhan.
      4. Simpan dokumen yang ditandatangani ke lokasi yang ditentukan.
   
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

        // Impor dokumen ke dalam instance Signature
        const signature = new signatureLib.Signature('input.xlsx');

        // Instansiasi objek QrCodeSignOptions
        const options = new signatureLib.QrCodeSignOptions('QR code text');
        
        // Tentukan semua opsi yang diperlukan
        options.setLeft(100);
        options.setTop(100);
        options.setForeColor(new Color(255, 0, 0));

        // Simpan dokumen yang ditandatangani ke disk lokal
        signature.sign('output.xlsx', options);
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kemampuan tanda tangan digital yang canggih"
  description: "API kami yang canggih memperlancar operasi bisnis dengan memfasilitasi penandatanganan otomatis, verifikasi, modifikasi, dan manajemen tanda tangan elektronik untuk berbagai dokumen."
  image: "/img/signature/features_esign.webp" # 500x500 px
  image_description: "Fitur tanda tangan digital"
  features:
    # feature loop
    - title: "Penandatanganan digital untuk file kantor"
      content: "Tambahkan tanda tangan digital ke halaman atau posisi mana pun dalam dokumen. Sesuaikan tanda tangan Anda dengan opsi seperti sertifikat digital, metadata, kode batang, atau elemen visual untuk meningkatkan keamanan dan integritas dokumen."

    # feature loop
    - title: "Kontrol tanda tangan yang komprehensif"
      content: "Setelah dokumen ditandatangani, Anda dapat mengelola tanda tangan dengan mudah. Ambil daftar lengkap semua tanda tangan, sehingga Anda dapat melakukan pembaruan atau menghapusnya sesuai kebutuhan."

    # feature loop
    - title: "Perkuat keamanan dokumen"
      content: "Gunakan sertifikat digital untuk melindungi dokumen Anda dari penyalahgunaan. Anda dapat menyematkan atau mengekstrak metadata untuk meningkatkan pelacakan dan audit, memastikan kepatuhan dan keaslian dokumen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menerapkan tanda tangan gambar pada dokumen"
      content: |
        Panduan ini merinci proses untuk melampirkan tanda tangan gambar ke halaman tertentu dalam dokumen.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
        
          // Beri dokumen sumber sebagai parameter input
          const signature = new signatureLib.Signature('input.xlsx');

          // Tentukan jalur file gambar dalam opsi konfigurasi tanda tangan
          const options = new signatureLib.ImageSignOptions('image.jpg');

          // Konfigurasikan dimensi dan tentukan halaman target untuk tanda tangan
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setHeight(150);
          options.setWidth(200);
          options.setMargin(new signatureLib.Padding(50));
          options.setAllPages(true);

          // Terapkan aplikasi tanda tangan pada dokumen
          signature.sign('output.xlsx', options);

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
            link: "/examples/signature/formats/signature_esign.xlsx"
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
    title: "Lihat kemampuan kami yang luas"
    exclude: "esign"
    description: "Kami menawarkan beragam jenis tanda tangan dan operasi yang kaya fitur."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/nodejs-java/text/xlsx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/xlsx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/nodejs-java/search/xlsx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/nodejs-java/verify/xlsx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/nodejs-java/modify/xlsx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tandai berbagai jenis file secara digital"
    exclude: "XLSX"
    description: "API Node.js via Java memungkinkan Anda untuk menerapkan tanda tangan digital pada lebih dari 60 format file, memberikan fleksibilitas luas dalam mengamankan dokumen penting bisnis Anda."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan Elektronik PDF"
          format: "PDF"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan Elektronik DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/esign/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan Elektronik JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/esign/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan Elektronik PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/esign/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan Elektronik XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/esign/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---