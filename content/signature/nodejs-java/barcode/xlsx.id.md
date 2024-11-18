



---
############################# Static ############################
layout: "format"
date:  2024-11-18T11:52:07
draft: false
lang: id
format: Xlsx
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Hasilkan kode batang untuk XLSX menggunakan Aplikasi JavaScript"
head_description: "Dengan cepat hasilkan dan sisipkan tanda tangan kode batang dalam dokumen XLSX menggunakan JavaScript hanya dengan beberapa baris kode. GroupDocs.Signature mendukung penandatanganan di berbagai format file."

############################# Header ############################
title: "Hasilkan dan tambahkan Kode Batang di XLSX dengan mudah" 
description: "Manfaatkan GroupDocs.Signature for Node.js via Java untuk memasukkan kode batang ke dalam dokumen bisnis Anda, menempatkannya tepat di lokasi yang dibutuhkan. Solusi kami menawarkan berbagai opsi kustomisasi untuk menyesuaikan tanda tangan kode batang sesuai keperluan Anda."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Sekarang – Gratis!"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Pengenalan ke GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) adalah alat penandatanganan dokumen yang kuat, mendukung berbagai jenis tanda tangan termasuk teks, gambar, kode batang, sertifikat digital, dan stempel. Dengan kompatibilitas di lebih dari 60 format file, seperti PDF, file MS Office, gambar, dan arsip ZIP, memungkinkan manajemen dokumen yang komprehensif. Tanda tangan dalam dokumen dapat dicari, diverifikasi, diubah, atau dihapus sesuai kebutuhan.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menghasilkan dan menyisipkan kode batang dalam file XLSX"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) memungkinkan penghasilan dan penempatan kode batang dalam berbagai format populer di halaman XLSX. Dengan dukungan lebih dari 60 jenis kode batang, aplikasi Node.js via Java dapat dengan mudah ditingkatkan dengan fitur penandatanganan kode batang dengan mengintegrasikan pustaka kami.
      
      1. Sediakan file atau aliran XLSX untuk diproses.
      2. Kirimkan teks kode batang ke dalam instance BarcodeSignOptions.
      3. Sesuaikan pengaturan kode batang seperti posisi, ukuran, dll.
      4. Simpan dokumen dengan kode batang yang baru ditambahkan.
   
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

        // Instansiasi objek Signature dengan jalur dokumen
        const signature = new signatureLib.Signature('input.xlsx');

        // Gunakan BarcodeSignOptions untuk mengintegrasikan kode batang ke dalam dokumen
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Konfigurasikan jenis kode batang dan parameter tambahan
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Simpan dokumen yang ditandatangani
        signature.sign('output.xlsx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan dan amankan dokumen Anda dengan opsi tanda tangan canggih"
  description: "Koleksi pustaka GroupDocs.Signature for Node.js via Java dirancang untuk menyederhanakan penandatanganan dan manajemen format dokumen populer. Tambahkan, ubah, verifikasi, atau hapus berbagai tanda tangan dengan cepat dan efisien."
  image: "/img/signature/features_barcode.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen dinamis"
      content: "Tandatangani sembarang halaman dokumen Anda menggunakan berbagai jenis tanda tangan, termasuk teks, gambar, kode batang, kode QR, dan stempel. Selain itu, Anda dapat menyisipkan metadata tersembunyi, seperti data EXIF dalam gambar, atau mengamankan dokumen dari perubahan tidak sah menggunakan sertifikat digital."

    # feature loop
    - title: "Verifikasi dan pencarian tanda tangan yang kuat"
      content: "Solusi kami menyediakan alat yang lengkap untuk mengelola dokumen yang ditandatangani. Verifikasi keaslian tanda tangan untuk memastikan integritas dokumen, dan gunakan fitur pencarian untuk mencantumkan semua tanda tangan yang disisipkan dalam dokumen."

    # feature loop
    - title: "Edit tanda tangan dengan mudah"
      content: "Sebagian besar tanda tangan yang ditambahkan sebelumnya dapat dimodifikasi dengan efisien. Perbarui teks, posisikan ulang, atau ubah tampilan tanda tangan untuk memenuhi kebutuhan Anda."

    # feature loop
    - title: "Penghapusan tanda tangan yang terampil"
      content: "Dengan dukungan komprehensif untuk operasi CRUD, alat kami memungkinkan penghapusan tanda tangan dari dokumen Anda secara efisien, memastikan hanya tanda tangan yang paling relevan yang tersisa."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cara menerapkan tanda tangan kode batang"
      content: |
        Contoh ini menggambarkan bagaimana menyisipkan kode batang yang disesuaikan pada halaman dokumen XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Sediakan dokumen yang akan ditandatangani
          const signature = new signatureLib.Signature('input.xlsx');

          // Gunakan BarcodeSignOptions untuk mengintegrasikan kode batang ke dalam dokumen
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // Konfigurasikan jenis kode batang dan parameter tambahan
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // Tentukan jarak padding kode batang dari tepi halaman
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Pilih warna batang
          signOptions.setForeColor(signatureLib.Color.RED);

          // Tentukan gaya font untuk pesan
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // Tunjukkan posisi pesan
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // Tandatangani dan simpan dokumen
          signature.sign('output.xlsx', signOptions);

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
            link: "/examples/signature/formats/signature_barcode.xlsx"
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
    title: "Selami fitur utama kami"
    exclude: "barcode"
    description: "Rasakan berbagai jenis tanda tangan dan alat yang kami sediakan"
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
    title: "Tandatangani di berbagai format dokumen"
    exclude: "XLSX"
    description: "API Node.js via Java memberdayakan Anda untuk menandatangani lebih dari 60 format berbeda. Apakah menambahkan tanda tangan di halaman tertentu atau menempatkannya secara presisi, alat kami memudahkan penerapan berbagai jenis tanda tangan."
    items: 
          
        # format loop 1
        - name: "Tambahkan barcode ke PDF"
          format: "PDF"
          link: "/signature/nodejs-java/barcode/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tambahkan barcode ke DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/barcode/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tambahkan barcode ke JPEG"
          format: "JPEG"
          link: "/signature/nodejs-java/barcode/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tambahkan barcode ke PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/barcode/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tambahkan barcode ke XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/barcode/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---