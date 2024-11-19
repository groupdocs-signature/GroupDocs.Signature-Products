



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:31
draft: false
lang: id
format: Docx
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cari tanda tangan digital di DOCX dengan Java"
head_description: "Manfaatkan API GroupDocs.Signature for Java untuk mencari tanda tangan dalam berkas DOCX. Temukan tanda tangan dalam PDF, Word, Excel, Presentasi, dan Gambar."

############################# Header ############################
title: "Cari tanda tangan digital di DOCX" 
description: "Ambil daftar lengkap e-signature yang tertanam dalam berkas PDF, Word, Excel, Presentasi, atau Gambar menggunakan GroupDocs.Signature for Java."
subtitle: "GroupDocs.Signature for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/signature/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Signature for Java"
    link: "/signature/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_signature.svg" # 480 X 400
    content: |
       [GroupDocs.Signature for Java](/signature/java/) menawarkan fitur kuat untuk menandatangani dokumen. Ini mendukung penambahan teks, gambar, kode batang, sertifikat digital, dan cap ke dalam berkas lebih dari 60 format, termasuk PDF, dokumen MS Office, Gambar, berkas ZIP, dan format bisnis umum lainnya. Selain itu, Anda dapat mencari, memverifikasi, memodifikasi, atau menghapus tanda tangan kapan saja.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk mencari tanda tangan DOCX menggunakan Java"
    content: |
      [GroupDocs.Signature](/signature/java/) menyediakan mesin yang kuat untuk mencari tanda tangan digital dalam berkas DOCX. Pengembang Java dapat memperkaya aplikasi mereka dengan solusi kami.
      
      1. Berikan jalur berkas DOCX untuk pencarian tanda tangan.
      2. Gunakan SearchOptions untuk menyaring hasil pencarian.
      3. Eksekusi metode Search untuk memperoleh hasil.
      4. Analisis daftar tanda tangan yang ditemukan.
   
    code:
      platform: "java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "Contoh tanda tangan"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-signature</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/signature/java/"
          
      content: |
        ```java {style=abap}

        // Buat instansi Signature dengan jalur dokumen
        final Signature signature = new Signature("input.docx");

        // Instantiate TextSearchOptions untuk mencakup semua halaman
        TextSearchOptions options = new TextSearchOptions();
        options.setAllPages(true);

        // Cari tanda tangan teks dalam dokumen
        List<TextSignature> signatures = signature.search(TextSignature.class, options);
        System.out.print("\nSource document contains following text signature(s).");

        // Daftar tanda tangan yang ditemukan untuk analisis lebih lanjut
        for (TextSignature textSignature : signatures) {
            System.out.print("Found Text signature at page " + textSignature.getPageNumber() 
                + " with type [" + textSignature.getSignatureImplementation() + "] and 
                text '" + textSignature.getText() + "'.");
        }
        
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Solusi tanda tangan dokumen yang komprehensif"
  description: "Kami bangga memperkenalkan solusi tanda tangan dokumen kami, yang kompatibel dengan semua format dokumen utama. Tambahkan berbagai tanda tangan untuk meningkatkan dokumen Anda atau mengamankan kontennya."
  image: "/img/signature/features_search.webp" # 500x500 px
  image_description: "Pencarian tanda tangan"
  features:
    # feature loop
    - title: "Tandatangani dokumen bisnis"
      content: "Sisipkan tanda tangan digital di mana saja pada halaman dokumen. Gunakan berbagai jenis tanda tangan, seperti teks, gambar, kode batang, metadata, cap, atau sertifikat digital."

    # feature loop
    - title: "Kelola tanda tangan"
      content: "Setelah ditandatangani, dokumen mungkin memerlukan pemrosesan lebih lanjut. Cari semua tanda tangan yang tersedia, dan perbarui atau hapus sesuai kebutuhan."

    # feature loop
    - title: "Lindungi konten dokumen"
      content: "Kelola metadata yang tersembunyi yang tertanam dalam dokumen. Tambahkan metadata baru atau hapus entri yang ada. Gunakan sertifikat digital perusahaan untuk melindungi konten dokumen dari perubahan yang tidak sah."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Cari tanda tangan gambar"
      content: |
        Contoh ini menunjukkan cara menemukan tanda tangan gambar dalam dokumen tertentu.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Lepaskan dokumen sumber sebagai parameter konstruktor
          final Signature signature = new Signature("input.docx");

          // Cari tanda tangan dengan jenis teks
          List<ImageSignature> signatures = signature.search(ImageSignature.class, SignatureType.Image);
          System.out.print("\nSource document contains following image signature(s).");

          // Tampilkan hasil beserta properti dari tanda tangan yang ditemukan
          for (ImageSignature imageSignature : signatures)
          {
              System.out.print("Image signature found at page "+imageSignature.getPageNumber()+
                    " with size "+imageSignature.getSize()+". Created "+imageSignature.getCreatedOn()+
                    ", modified "+imageSignature.getModifiedOn());
          }
          ```
        platform: "java"
        copy_title: "Salin"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-signature</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/signature/java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Signature secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan Maven"
      link: "https://releases.groupdocs.com/signature/java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/signature/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Operasi yang Didukung"
    exclude: "search"
    description: "Produk kami menawarkan API fleksibel untuk menandatangani dokumen dan mengelola tanda tangan setelah penandatanganan."
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/docx/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/docx/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/docx/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/docx/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/docx/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/docx/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/docx/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/java/search/docx/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/java/verify/docx/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/java/modify/docx/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/java/delete/docx/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari tanda tangan dalam berbagai format berkas"
    exclude: "DOCX"
    description: "API GroupDocs.Signature for Java memungkinkan Anda mengambil daftar tanda tangan dari setiap berkas yang ditandatangani. Ekstrak tanda tangan dari format berkas populer untuk pemrosesan lebih lanjut."
    items: 
          
        # format loop 1
        - name: "Cari tanda tangan dalam PDF"
          format: "PDF"
          link: "/signature/java/search/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Temukan tanda tangan dalam DOCX"
          format: "DOCX"
          link: "/signature/java/search/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Temukan tanda tangan dalam PPTX"
          format: "PPTX"
          link: "/signature/java/search/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Cari tanda tangan dalam XLSX"
          format: "XLSX"
          link: "/signature/java/search/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---