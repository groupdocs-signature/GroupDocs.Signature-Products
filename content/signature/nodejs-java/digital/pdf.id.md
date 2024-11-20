



---
############################# Static ############################
layout: "format"
date:  2024-11-20T08:57:23
draft: false
lang: id
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Menambahkan tanda tangan elektronik digital ke file PDF dengan JavaScript"
head_description: "Tambahkan tanda tangan digital pada file PDF menggunakan JavaScript hanya dengan beberapa baris kode. Gunakan GroupDocs.Signature for Node.js via Java untuk menandatangani berbagai format file."

############################# Header ############################
title: "Lindungi PDF dengan sertifikat digital" 
description: "Pastikan keamanan dokumen bisnis Anda dengan menyematkan sertifikat digital menggunakan kemampuan canggih dari GroupDocs.Signature for Node.js via Java. Kami menawarkan opsi fleksibel untuk melindungi dan mengautentikasi dokumen Anda."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) adalah solusi penandatanganan menyeluruh yang dirancang untuk menangani berbagai kebutuhan pemrosesan dokumen. Ini memungkinkan Anda untuk menggabungkan teks, gambar, sertifikat digital, dan stempel ke dalam lebih dari 60 format file berbeda, termasuk PDF, MS Office, gambar, dan file ZIP. Selain itu, dokumen yang ditandatangani dapat dengan mudah dicari, diverifikasi, diedit, atau dihapus jika diperlukan.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk mengamankan PDF dengan sertifikat digital dalam JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) memungkinkan pengembang Node.js via Java untuk melindungi dokumen PDF dari modifikasi dengan menggunakan tanda tangan digital. Tingkatkan aplikasi bisnis Anda dengan fitur keamanan data yang komprehensif.
      
      1. Lepaskan dokumen PDF ke konstruktor kelas Signature.
      2. Terapkan sertifikat digital dan kata sandi yang sesuai untuk mengamankan dokumen.
      3. Opsional, tambahkan representasi visual tanda tangan digital pada halaman dokumen.
      4. Tandatangani dokumen untuk mencegah perubahan di masa mendatang.
   
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

        // Gunakan Signature untuk menerapkan tanda tangan digital pada dokumen
        const signature = new signatureLib.Signature('input.pdf');

        // Sediakan sertifikat digital dan kata sandi yang diperlukan
        const options = new signatureLib.DigitalSignOptions('certificate.pfx');
        options.setPassword('1234567890');

        // Sesuaikan pengaturan tampilan tanda tangan jika diperlukan
        options.setPageNumber(1);
        options.setLeft(100);
        options.setTop(100);
        
        // Enkripsi dokumen menggunakan sertifikat digital
        const result = signature.sign('output.pdf', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Optimalkan atau amankan konten dokumen dengan tanda tangan"
  description: "GroupDocs.Signature for Node.js via Java dirancang untuk menandatangani semua format file utama, memberikan Anda kemampuan untuk menambahkan, menyesuaikan, memverifikasi, atau menghapus berbagai jenis tanda tangan dengan efektif."
  image: "/img/signature/features_digital.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Signature"
  features:
    # feature loop
    - title: "Tambahkan tanda tangan ke dokumen Anda"
      content: "Tempatkan dengan mudah tanda tangan Teks, Gambar, Kode Batang, QR-Code, atau Stempel di halaman mana pun dari dokumen yang didukung. Anda juga dapat menyisipkan atau mengedit metadata tersembunyi, seperti EXIF pada gambar. Lindungi konten dokumen Anda dari perubahan yang tidak sah dengan sertifikat digital."

    # feature loop
    - title: "Temukan dan verifikasi tanda tangan"
      content: "Setelah penandatanganan, dokumen Anda dapat menjalani banyak verifikasi. Konfirmasi integritas konten yang ditandatangani, atau lakukan pencarian mendetail untuk mencantumkan semua tanda tangan yang ada."

    # feature loop
    - title: "Revisi tanda tangan yang ada"
      content: "Sebagian besar jenis tanda tangan memungkinkan pengeditan setelah pembuatan. Anda dapat dengan mudah memodifikasi teks, mengubah posisi elemen, menyesuaikan warna, mengubah ukuran, dan melakukan perubahan lain yang diperlukan."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "Solusi kami memungkinkan operasi CRUD penuh untuk tanda tangan. Jika diperlukan, Anda dapat menghapus berbagai jenis tanda tangan, termasuk sertifikat digital, dari dokumen Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Lindungi dokumen dengan tanda tangan digital"
      content: |
        Pelajari cara mengunci dokumen dari perubahan menggunakan tanda tangan digital.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Sediakan dokumen yang memerlukan penandatanganan
          const signature = new signatureLib.Signature('input.pdf');

          // Gunakan sertifikat digital yang sesuai dan kata sandinya
          const options = new signatureLib.DigitalSignOptions('certificate.pfx');
          options.setPassword('1234567890');

          // Sertakan informasi teks tambahan
          options.setReason('Security issue');
          options.setContact('John Smith');
          options.setLocation('Office D.W.');

          // Tambahkan elemen visual seperti gambar untuk representasi tanda tangan
          options.setImageFilePath('image.png');
          options.setAllPages(true);
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
          options.setWidth(80);
          options.setHeight(60);

          const padding = new signatureLib.Padding();
          padding.setBottom(10);
          padding.setRight(10);
          options.setMargin(padding);
          
          // Simpan dokumen yang diamankan secara digital ke lokasi yang ditentukan
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
            link: "/examples/signature/formats/signature_digital.pdf"
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
    title: "Kenali fungsi utama kami"
    exclude: "digital"
    description: "Kami bangga mendukung serangkaian opsi tanda tangan dan fungsionalitas yang komprehensif."
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
    title: "Tandatangani dokumen dalam berbagai format"
    exclude: "PDF"
    description: "API Node.js via Java mendukung lebih dari 60 format, memungkinkan Anda menerapkan berbagai tanda tangan di mana saja, memaksakan keamanan konten dengan sertifikat digital, dan mengelola tanda tangan dalam dokumen secara efektif."
    items: 
          
        # format loop 1
        - name: "Lindungi PDF"
          format: "PDF"
          link: "/signature/nodejs-java/digital/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Lindungi DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/digital/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Lindungi PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/digital/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Lindungi XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/digital/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---