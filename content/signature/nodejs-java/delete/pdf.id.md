



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:42
draft: false
lang: id
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Hapus tanda tangan dari PDF melalui JavaScript"
head_description: "Penghapusan tanda tangan Digital, Barcode, Teks, Gambar, Metadata dari dokumen PDF yang ditandatangani dapat dilakukan dengan menggunakan GroupDocs.Signature for Node.js via Java."

############################# Header ############################
title: "Hapus tanda tangan yang terdapat di PDF tanpa kesulitan" 
description: "Solusi komprehensif kami melampaui tanda tangan dokumen sederhana, menawarkan fitur kuat dalam GroupDocs.Signature for Node.js via Java untuk menemukan dan menghapus berbagai jenis tanda tangan."
subtitle: "GroupDocs.Signature for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan unduhan gratis Anda"
      link: "https://releases.groupdocs.com/signature/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Temukan GroupDocs.Signature for Node.js via Java"
    link: "/signature/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Node.js via Java](/signature/nodejs-java/) adalah perpustakaan tanda tangan digital tingkat perusahaan yang dirancang untuk mendukung berbagai jenis tanda tangan, termasuk teks, gambar, barcode, sertifikat digital, dan stempel. Dengan kompatibilitas di lebih dari 60 format dokumen—seperti PDF, file MS Office, gambar, arsip ZIP, dan format bisnis penting lainnya—alat ini menawarkan fleksibilitas tak tertandingi dalam alur kerja dokumen elektronik. Platform ini tidak hanya memfasilitasi penyisipan tanda tangan yang mulus tetapi juga memberikan fungsionalitas yang kuat untuk mencari, memvalidasi, memperbarui, dan menghapus tanda tangan, memastikan pengelolaan siklus penuh dari proses penandatanganan digital di lingkungan perusahaan.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk menghapus tanda tangan digital dari PDF menggunakan JavaScript"
    content: |
      [GroupDocs.Signature](/signature/nodejs-java/) memungkinkan pengembang Node.js via Java untuk secara efisien menghapus e-signatures dalam file PDF dengan mengikuti serangkaian langkah sederhana.
      
      1. Berikan jalur file PDF kepada instance kelas Signature.
      2. Gunakan metode Search untuk mengidentifikasi semua tanda tangan di dokumen.
      3. Hapus satu atau beberapa tanda tangan yang teridentifikasi.
      4. Tinjau hasil pemrosesan dokumen.
   
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

        // Serahkan dokumen dengan tanda tangan kepada instance Signature
        const signature = new signatureLib.Signature('input.pdf');

        // Hapus semua tanda tangan barcode
        const options = new signatureLib.DigitalSearchOptions();
        const signatures = signature.search(signatureLib.DigitalSignature.class, options);

        // Hapus tanda tangan digital yang terdeteksi pertama
        if(signatures.size() > 0)
        {
            const digitalSignature = signatures[0];
            const result = signature.delete('output.pdf', digitalSignature);

            // Tangani hasil penghapusan
            if(result)
            {
                console.log(`\n PDF digital signature deleted successfully`);
            }
        }

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tingkatkan keamanan dokumen dengan alat tanda tangan"
  description: "GroupDocs.Signature for Node.js via Java dirancang khusus untuk memperlancar penandatanganan dan pengelolaan format file bisnis, memungkinkan Anda untuk menambahkan, mengedit, memverifikasi, atau menghapus tanda tangan dengan presisi."
  image: "/img/signature/features_delete.webp" # 500x500 px
  image_description: "Jelajahi kemampuan komprehensif dari GroupDocs.Signature"
  features:
    # feature loop
    - title: "Penandatanganan dokumen"
      content: "Tambahkan tanda tangan teks, gambar, barcode, kode QR, atau stempel ke setiap halaman dokumen yang didukung. Manfaatkan metadata tersembunyi seperti EXIF dalam gambar, atau amankan integritas dokumen dengan sertifikat digital untuk mencegah modifikasi yang tidak sah."

    # feature loop
    - title: "Pencarian dan validasi tanda tangan"
      content: "Alat kami memungkinkan verifikasi menyeluruh tanda tangan dokumen, memastikan keasliannya. Lakukan pencarian komprehensif untuk mengambil semua tanda tangan dalam dokumen Anda, meningkatkan kontrol dokumen."

    # feature loop
    - title: "Edit tanda tangan yang sudah ada"
      content: "Modifikasi tanda tangan yang telah ditambahkan sebelumnya dengan menyesuaikan teks, mengubah posisi, atau mengganti warna sesuai kebutuhan spesifik Anda."

    # feature loop
    - title: "Hapus tanda tangan yang tidak diinginkan"
      content: "Dengan kemampuan CRUD penuh, solusi kami memungkinkan penghapusan yang efisien dari berbagai jenis tanda tangan dari dokumen Anda, memastikan fleksibilitas dan kontrol."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Hapus semua tanda tangan barcode"
      content: |
        Pelajari prosedur untuk menghilangkan semua tanda tangan barcode yang tertanam dalam dokumen.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const signatureLib = require('@groupdocs/groupdocs.signature')
          
          // Sediakan dokumen yang mencakup tanda tangan barcode
          const signature = new signatureLib.Signature('input.pdf');

          // Hapus semua tanda tangan barcode
          const result = await signature.delete('output.pdf', signatureLib.SignatureType.Barcode);
          if (result.getSucceeded().size() > 0) {

              // Tinjau hasil penghapusan
              console.log('Following PDF barcode signatures were deleted:');
              let number = 1;
              result.getSucceeded().toArray().forEach((o) => {
                    const temp = o;
                    console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                    Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
              });
          }
          ```
        platform: "nodejs-java"
        copy_title: "Salin"
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
    title: "Jelajahi fitur yang kami tawarkan"
    exclude: "delete"
    description: "Temukan berbagai solusi dan operasi tanda tangan yang tersedia di sistem kami"
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
    title: "Hapus tanda tangan dari berbagai format file"
    exclude: "PDF"
    description: "Solusi GroupDocs.Signature for Node.js via Java kami ahli dalam menghapus tanda tangan di lebih dari 60 format file yang bervariasi, memastikan kompatibilitas dan fungsionalitas yang luas."
    items: 
          
        # format loop 1
        - name: "Hapus tanda tangan PDF"
          format: "PDF"
          link: "/signature/nodejs-java/delete/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Hapus tanda tangan DOCX"
          format: "DOCX"
          link: "/signature/nodejs-java/delete/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Hapus tanda tangan PPTX"
          format: "PPTX"
          link: "/signature/nodejs-java/delete/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Hapus tanda tangan XLSX"
          format: "XLSX"
          link: "/signature/nodejs-java/delete/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---