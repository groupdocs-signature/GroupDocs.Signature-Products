



---
############################# Static ############################
layout: "format"
date:  2024-11-19T15:16:38
draft: false
lang: id
format: Pdf
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ubah tanda tangan PDF dengan aplikasi Java"
head_description: "API pemrosesan tanda tangan Java memungkinkan Anda untuk memodifikasi tanda tangan dalam file PDF, termasuk PDF, Word, Excel, Presentasi, dan Gambar."

############################# Header ############################
title: "Modifikasi tanda tangan PDF" 
description: "Modifikasi berbagai tanda tangan elektronik menggunakan GroupDocs.Signature for Java di berbagai format seperti PDF, Word, Excel, Presentasi, dan Gambar."
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
       [GroupDocs.Signature for Java](/signature/java/) tidak hanya memungkinkan Anda untuk menandatangani dokumen tetapi juga memberikan kemampuan untuk memodifikasi tanda tangan yang sudah ada. Perbarui tanda tangan dalam format yang banyak digunakan seperti PDF, Word, Excel, dan Presentasi.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah-langkah untuk mengedit tanda tangan teks di PDF menggunakan Java"
    content: |
      [GroupDocs.Signature](/signature/java/) memungkinkan para pengembang Java untuk memperbarui konten tanda tangan teks yang sebelumnya ditambahkan ke file PDF. Tingkatkan aplikasi Java Anda dengan kemampuan yang kuat.
      
      1. Tambahkan file PDF ke instance Signature.
      2. Ambil daftar semua tanda tangan dalam dokumen.
      3. Perbarui konten tanda tangan yang teridentifikasi.
      4. Analisis hasil modifikasi.
   
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
        // Buat objek Signature dengan jalur dokumen
        Signature signature = new Signature("input.pdf");

        // Cari tanda tangan teks dalam dokumen
        TextSearchOptions options = new TextSearchOptions();
        List<TextSignature> signatures = signature.search(TextSignature.class, options);

        if (signatures.size() > 0) {
            // Ubah teks tanda tangan yang terdeteksi pertama
            TextSignature textSignature = signatures.get(0);
            textSignature.setText("New Text");
            boolean result = signature.update('output.pdf', textSignature);

            // Verifikasi hasil modifikasi
            if (result) {
                System.out.print("\nSignature was updated successfully.");
            }
        }
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Manajemen tanda tangan untuk dokumen"
  description: "GroupDocs.Signature for Java memungkinkan Anda untuk menambah, memodifikasi, mencari, memverifikasi, dan menghapus tanda tangan di semua format file industri utama."
  image: "/img/signature/features_modify.webp" # 500x500 px
  image_description: "Modifikasi tanda tangan"
  features:
    # feature loop
    - title: "Tanda tangan dokumen"
      content: "Produk kami terutama fokus pada penandatanganan dokumen dengan tanda tangan teks, gambar, barcode, atau cap. Anda dapat menempatkannya di halaman atau posisi mana pun. Tambahkan atau modifikasi metadata tersembunyi, seperti data EXIF dalam gambar, dan lindungi konten dokumen dari perubahan yang tidak sah menggunakan sertifikat digital."

    # feature loop
    - title: "Pencarian dan verifikasi tanda tangan"
      content: "Pastikan bahwa tanda tangan memenuhi persyaratan Anda dengan memverifikasi dokumen yang ditandatangani. Anda dapat mengambil daftar lengkap tanda tangan dalam dokumen melalui fungsi pencarian."

    # feature loop
    - title: "Modifikasi tanda tangan yang sudah ada"
      content: "Memodifikasi tanda tangan yang telah ditambahkan sebelumnya adalah tugas yang umum. Gunakan proses modifikasi untuk memperbarui konten, penampilan, posisi, dan properti lain dari sebuah tanda tangan."

    # feature loop
    - title: "Penghapusan tanda tangan"
      content: "Solusi kami sepenuhnya mendukung semua operasi terkait tanda tangan. Menghapus berbagai jenis tanda tangan dari dokumen adalah proses yang sederhana."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Modifikasi tanda tangan barcode"
      content: |
        Contoh ini menjelaskan proses modifikasi tanda tangan barcode dalam sebuah dokumen.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Gunakan dokumen yang berisi tanda tangan barcode
          final Signature signature = new Signature("input.pdf");

          // Cari tanda tangan barcode yang ada
          BarcodeSearchOptions options = new BarcodeSearchOptions();
          List<BarcodeSignature> signatures = signature.search(BarcodeSignature.class, options);

          if (signatures.size() > 0)
          {
              // Sesuaikan posisi barcode pertama dan simpan dokumen yang diperbarui
              BarcodeSignature barcodeSignature = signatures.get(0);
              barcodeSignature.setLeft(100);
              barcodeSignature.setTop(100);
              boolean result = signature.update("output.pdf", barcodeSignature);

              // Konfirmasikan hasil modifikasi
              if (result)
              {
                    System.out.print("\nBarcode was updated successfully.");
              }
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
    title: "Telusuri portofolio fitur kami"
    exclude: "modify"
    description: "Kami bangga mendukung berbagai format tanda tangan dan alat operasional"
    items: 
          
        # operation loop 1
        - name: "Tanda Tangan Elektronik"
          operation: "esign"
          link: "/signature/java/esign/pdf/"
          description: "Tambahkan berbagai jenis tanda tangan ke format file yang didukung"

        # operation loop 2
        - name: "Tambahkan teks ke dokumen"
          operation: "text"
          link: "/signature/java/text/pdf/"
          description: "Tingkatkan konten dokumen dengan tanda tangan teks yang dapat disesuaikan"

        # operation loop 3
        - name: "Tanda Tangan Gambar"
          operation: "image"
          link: "/signature/java/image/pdf/"
          description: "Tempatkan gambar di posisi mana pun dalam dokumen"

        # operation loop 4
        - name: "Hasilkan barcode"
          operation: "barcode"
          link: "/signature/java/barcode/pdf/"
          description: "Buat dan sisipkan berbagai barcode ke dalam dokumen yang didukung"

        # operation loop 5
        - name: "Hasilkan QR code"
          operation: "qrcode"
          link: "/signature/java/qrcode/pdf/"
          description: "Buat dan QR Code, termasuk QR code, untuk penandatanganan dokumen"
          
        # operation loop 6
        - name: "Sertifikat Digital"
          operation: "digital"
          link: "/signature/java/digital/pdf/"
          description: "Amankan bisnis dan tanda tangani dokumen dengan sertifikat digital"

        # operation loop 7
        - name: "Tanda Tangan Stempel"
          operation: "stamp"
          link: "/signature/java/stamp/pdf/"
          description: "Gunakan Konstruksi Stempel untuk membuat stempel bulat atau persegi yang kustom"
          
        # operation loop 8
        - name: "Cari tanda tangan"
          operation: "search"
          link: "/signature/java/search/pdf/"
          description: "Temukan tanda tangan yang ditambahkan sebelumnya dalam dokumen"
          
        # operation loop 9
        - name: "Verifikasi tanda tangan"
          operation: "verify"
          link: "/signature/java/verify/pdf/"
          description: "Verifikasi keaslian tanda tangan setelah diterapkan"
          
        # operation loop 10
        - name: "Modifikasi tanda tangan"
          operation: "modify"
          link: "/signature/java/modify/pdf/"
          description: "Edit berbagai tanda tangan dalam dokumen"
          
        # operation loop 11
        - name: "Hapus tanda tangan"
          operation: "delete"
          link: "/signature/java/delete/pdf/"
          description: "Hapus berbagai tanda tangan yang diterapkan sebelumnya"
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Modifikasi tanda tangan dalam berbagai format file"
    exclude: "PDF"
    description: "Format dokumen yang ditandatangani menggunakan API kami untuk Java dapat dimodifikasi. Ambil daftar tanda tangan dari dokumen dan perbarui properti yang dapat diakses."
    items: 
          
        # format loop 1
        - name: "Modifikasi tanda tangan PDF"
          format: "PDF"
          link: "/signature/java/modify/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 2
        - name: "Edit tanda tangan DOCX"
          format: "DOCX"
          link: "/signature/java/modify/docx/"
          description: "Dokumen XML Terbuka Microsoft Word"
          
        # format loop 3
        - name: "Edit tanda tangan PPTX"
          format: "PPTX"
          link: "/signature/java/modify/pptx/"
          description: "Presentasi XML Terbuka PowerPoint"
          
        # format loop 4
        - name: "Modifikasi tanda tangan XLSX"
          format: "XLSX"
          link: "/signature/java/modify/xlsx/"
          description: "Spreadsheet XML Terbuka Microsoft Excel"


          

---