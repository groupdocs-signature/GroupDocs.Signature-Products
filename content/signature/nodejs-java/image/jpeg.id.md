



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:10
draft: false
lang: id
format: Jpeg
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Menambahkan Tanda Tangan Gambar ke file JPEG dengan JavaScript"
head_description: "Tempatkan tanda tangan gambar pada file JPEG untuk Node.js hanya dengan beberapa baris kode. Gunakan API GroupDocs.Signature for Node.js via Java untuk menambahkan gambar."

############################# Header ############################
title: "Tandai file JPEG menggunakan tanda tangan gambar" 
description: "Manfaatkan kemampuan dari GroupDocs.Signature for Node.js via Java untuk cara efisien menyematkan gambar ke dalam berbagai format dokumen kantor seperti PDF, Word, Excel, dan berbagai file gambar. Menambahkan gambar tanda tangan eksekutif dapat secara signifikan meningkatkan profesionalisme dan kredibilitas dokumen Anda, menciptakan presentasi yang lebih baik dan halus."
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
    title: "Memperkenalkan GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) memberi pengguna kemampuan untuk memasukkan tanda tangan gambar di mana saja dalam dokumen Anda. Alat ini memungkinkan bisnis untuk merampingkan alur kerja mereka dengan menambahkan gambar ke PDF, Word, Excel, PowerPoint, dan format gambar populer, meningkatkan efisiensi manajemen dokumen.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk menambahkan gambar di JPEG menggunakan JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) memberdayakan aplikasi Node.js via Java untuk secara seamless mengintegrasikan tanda tangan gambar ke dalam dokumen JPEG. Tingkatkan kemampuan aplikasi Anda dengan perpustakaan komprehensif kami.
      
      1. Instantiate Signature dengan dokumen JPEG
      2. Gunakan ImageSignOptions untuk menentukan gambar tanda tangan
      3. Posisikan gambar dengan tepat di halaman mana pun
      4. Simpan dokumen yang ditandatangani di lokasi yang diinginkan
   
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

        // Inisialisasi Signature dengan jalur ke dokumen
        const signature = new signatureLib.Signature('input.jpeg');

        // Konfigurasikan ImageSignOptions untuk menyertakan tanda tangan gambar yang diinginkan
        const options = new signatureLib.ImageSignOptions('company_logo.jpg');

        // Tempatkan gambar di sudut kiri atas pada semua halaman
        options.setAllPages(true);
        options.setLeft(100);
        options.setTop(200);
        
        // Simpan dokumen dengan tanda tangan gambar yang diterapkan
        const result = signature.sign('output.jpeg', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kemampuan tanda tangan dokumen yang canggih"
  description: "API kami menawarkan serangkaian fitur yang menyederhanakan tanda tangan elektronik. Anda dapat menambahkan, memodifikasi, menghapus, mencari, dan memverifikasi berbagai jenis tanda tangan, termasuk tanda tangan gambar, dengan efektif."
  image: "/img/signature/features_image.webp" # 500x500 px
  image_description: "Tanda tangan gambar"
  features:
    # feature loop
    - title: "Sisipkan gambar ke dalam dokumen kantor"
      content: "Letakkan tanda tangan gambar di mana saja dalam dokumen Anda, baik itu file PDF, Word, atau Excel. Tingkatkan dokumen Anda dengan menambahkan gambar, barcode, metadata, atau sertifikat digital untuk meningkatkan fungsionalitas."

    # feature loop
    - title: "Cari dan verifikasi tanda tangan"
      content: "Pastikan keaslian dokumen yang telah Anda tanda tangani dengan memverifikasi tanda tangan tersebut. Gunakan fungsi pencarian untuk mengambil dan meninjau semua tanda tangan yang disematkan dalam dokumen Anda."

    # feature loop
    - title: "Modifikasi tanda tangan yang sudah ada"
      content: "API kami memungkinkan pengguna untuk memperbarui dan menyesuaikan tanda tangan sesuai kebutuhan. Ubah ukuran, posisi, atau atribut lainnya dari setiap tanda tangan yang telah ditambahkan untuk fleksibilitas dalam penanganan dokumen."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diperlukan"
      content: "Kelola dokumen Anda dengan efisien dengan menghapus tanda tangan yang sudah tidak diperlukan lagi. API kami mendukung operasi CRUD penuh untuk hampir semua jenis tanda tangan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Tingkatkan dokumen dengan tanda tangan gambar"
      content: |
        Pelajari cara memasukkan gambar ke dalam dokumen bisnis untuk menambah informasi tambahan.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Pilih dokumen yang akan ditandatangani
          const signature = new signatureLib.Signature('input.jpeg');

          // Konfigurasikan opsi gambar dengan jalur gambar
          const options = new signatureLib.ImageSignOptions('manager_signature.jpg');

          // Sesuaikan ukuran tanda tangan gambar
          options.setWidth(100);
          options.setHeight(100);

          // Tempatkan gambar di sudut kanan bawah
          options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);

          // Terapkan padding dari sudut halaman jika perlu
          const padding = new signatureLib.Padding();
          padding.setRight(120);
          padding.setBottom(120);
          options.setMargin(padding);

          // Opsional, tambahkan border kustom pada gambar
          const border = new signatureLib.Border();
          border.setColor(signatureLib.Color.RED);
          border.setDashStyle(signatureLib.DashStyle.DashDotDot);
          border.setWeight(5);
          border.setVisible(true);
          options.setBorder(border);

          // Putar tanda tangan gambar untuk penampilan yang optimal
          options.setRotationAngle(45);

          // Simpan dokumen yang telah diperbarui di lokasi yang diinginkan
          const result = signature.sign('output.jpeg', options);
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
            link: "/examples/signature/formats/signature_image.jpeg"
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
    title: "Temukan fungsi yang kami tawarkan"
    exclude: "image"
    description: "Kami bangga menunjukkan berbagai metode dan operasi tanda tangan yang kami miliki."
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
    title: "Tambahkan gambar ke berbagai tipe file"
    exclude: "JPEG"
    description: "API Node.js via Java memungkinkan Anda menyematkan gambar ke dalam berbagai format dokumen. Sesuaikan ukuran, penempatan, dan posisi halaman untuk meningkatkan proses penandatanganan dokumen Anda."
    items: 
          
        # format loop 1
        - name: "Tanda Tangan PDF dengan Gambar"
          format: "PDF"
          link: "/signature/nodejs-java/image/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Tanda Tangan DOCX dengan Gambar"
          format: "DOCX"
          link: "/signature/nodejs-java/image/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Tanda Tangan JPEG dengan Gambar"
          format: "JPEG"
          link: "/signature/nodejs-java/image/jpeg/"
          description: "Gambar JPEG"
          
        # format loop 4
        - name: "Tanda Tangan PPTX dengan Gambar"
          format: "PPTX"
          link: "/signature/nodejs-java/image/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 5
        - name: "Tanda Tangan XLSX dengan Gambar"
          format: "XLSX"
          link: "/signature/nodejs-java/image/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---