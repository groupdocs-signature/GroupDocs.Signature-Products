



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:06
draft: false
lang: id
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Buat dan tambahkan cap ke PDF melalui JavaScript"
head_description: "Manfaatkan kekuatan GroupDocs.Signature dan JavaScript untuk menghasilkan dan menempatkan cap kustom di setiap halaman dalam dokumen PDF Anda."

############################# Header ############################
title: "Sisipkan cap kustom ke dalam file PDF" 
description: "Gunakan GroupDocs.Signature for Node.js via Java untuk membuat cap yang disesuaikan dan menyisipkannya di lokasi mana pun dalam dokumen Anda. Platform kami menyediakan berbagai opsi untuk mempersonalisasi cap sesuai kebutuhan bisnis spesifik Anda."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Uji coba gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Signature for Node.js via Java?"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) menyediakan solusi yang kuat dan serbaguna untuk penandatanganan dokumen. Ini memungkinkan pengguna untuk menambahkan cap dan jenis tanda tangan lain di lebih dari 60 format yang berbeda, seperti PDF, Word, Excel, file gambar, dan file ZIP. Platform ini memungkinkan Anda untuk menyisipkan teks, gambar, barcode, kode QR, metadata, sertifikat digital, dan tanda tangan cap. Selain menandatangani, Anda dapat mencari, memverifikasi, memodifikasi, atau menghapus tanda tangan yang ada dalam dokumen Anda.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk menyematkan cap di PDF menggunakan JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) menyediakan alat yang kuat untuk membuat dan menyematkan cap, yang dapat secara signifikan meningkatkan aplikasi Node.js via Java. Gunakan fitur ini untuk merancang dan menerapkan cap kustom ke halaman dokumen Anda.
      
      1. Masukkan dokumen PDF yang memerlukan cap.
      2. Terapkan StampSignOptions untuk mendefinisikan semua parameter penting.
      3. Sisipkan sebanyak mungkin garis cap sesuai kebutuhan.
      4. Terapkan cap dan simpan dokumen yang telah selesai.
   
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

        // Hubungkan jalur dokumen dengan instance Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Buat StampSignOptions dengan konten tanda tangan yang diperlukan
        const options = new signatureLib.StampSignOptions();
        options.Height = 180;
        options.Width = 180;

        // Sisipkan satu atau lebih garis cap
        const outerLine = new signatureLib.StampLine();
        outerLine.setText("* The Best Company *");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // Simpan dokumen dengan cap yang diterapkan
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Perkuat keamanan dokumen dengan tanda tangan"
  description: "Dengan GroupDocs.Signature for Node.js via Java, Anda dapat menambahkan, mengedit, memvalidasi, atau menghapus cap dan jenis tanda tangan lain dalam semua format dokumen yang populer. API ini menyederhanakan proses pengelolaan tanda tangan untuk meningkatkan integritas dan kustomisasi dokumen."
  image: "/img/signature/features_stamp.webp" # 500x500 px
  image_description: "Fitur GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen kustom"
      content: "Terapkan tanda tangan seperti teks, gambar, barcode, kode QR, dan cap ke bagian manapun dari dokumen Anda. Alat ini juga memungkinkan penyertaan metadata tersembunyi dan sertifikat digital untuk melindungi konten Anda dari modifikasi yang tidak sah."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Setelah dokumen ditandatangani, gunakan sistem verifikasi kami untuk memastikan integritas tanda tangan. Selain itu, platform kami memungkinkan Anda untuk mencari dan mengambil informasi terperinci tentang semua tanda tangan yang diterapkan pada dokumen."

    # feature loop
    - title: "Modifikasi tanda tangan sesuai kebutuhan"
      content: "Sesuaikan dan perbarui tanda tangan yang telah diterapkan sebelumnya dengan mudah. Baik itu mengubah konten, warna, ukuran, atau posisi tanda tangan, GroupDocs.Signature for Node.js via Java menawarkan opsi kustomisasi penuh."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diinginkan"
      content: "Hapus dengan mudah tanda tangan yang tidak perlu dari dokumen Anda. API kami mendukung penghapusan berbagai jenis tanda tangan, termasuk cap dan sertifikat digital, memberikan Anda fleksibilitas penuh untuk mengelola dokumen Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Integrasikan cap kustom ke dalam dokumen"
      content: |
        Pelajari cara merancang dan menerapkan cap yang disesuaikan yang berisi teks penting ke dokumen Anda.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Berikan dokumen untuk dicap
          const signature = new signatureLib.Signature('input.pdf');

          // Atur opsi cap dengan konfigurasi yang diinginkan
          const options = new signatureLib.StampSignOptions();

          // Tentukan dimensi dan posisi cap di halaman
          options.setHeight(200);
          options.setWidth(200);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setAllPages(true);

          // Sertakan garis luar melingkar dengan teks kustom
          const outerLine1 = new signatureLib.StampLine();
          outerLine1.setText('* The best  choice *');
          outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
          const signatureFont1 = new signatureLib.SignatureFont();
          signatureFont1.setSize(12);
          signatureFont1.setFamilyName('Arial');
          outerLine1.setFont(signatureFont1);
          outerLine1.setHeight(30);
          outerLine1.setTextBottomIntent(6);
          outerLine1.setTextColor(signatureLib.Color.WHITE);
          outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
          options.getOuterLines().add(outerLine1);

          // Tambahkan garis dalam persegi sesuai kebutuhan
          const innerLine1 = new signatureLib.StampLine();
          innerLine1.setText('Company #1');
          innerLine1.setTextColor(signatureLib.Color.RED);
          const signFont1 = new signatureLib.SignatureFont();
          signFont1.setSize(20);
          signFont1.setBold(true);
          innerLine1.setFont(signFont1);
          innerLine1.setHeight(40);
          options.getInnerLines().add(innerLine1);
          
          // Simpan dokumen yang telah dicap
          const result = signature.sign('output.pdf', options);
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
            link: "/examples/signature/formats/signature_stamp.pdf"
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
    title: "Jelajahi fitur kunci"
    exclude: "stamp"
    description: "Solusi kami menawarkan berbagai alat untuk membuat, mengelola, dan menghapus berbagai jenis tanda tangan, memberikan pengguna kontrol penuh atas alur kerja dokumen mereka."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/nodejs-java/esign/pdf/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/nodejs-java/text/pdf/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/nodejs-java/qrcode/pdf/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/nodejs-java/stamp/pdf/"
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
    title: "Terapkan tanda tangan cap di berbagai jenis file"
    exclude: "PDF"
    description: "API GroupDocs.Signature mendukung tanda tangan cap di lebih dari 60 format file, memungkinkan pengguna untuk menempatkan cap kustom di setiap halaman atau area, meningkatkan aksesibilitas dan keamanan dokumen."
    items: 
          
        # format loop 1
        - name: "Stempel PDF"
          format: "PDF"
          link: "/signature/nodejs-java/stamp/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Stempel DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/stamp/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Stempel JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/stamp/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Stempel PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/stamp/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Stempel XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/stamp/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---