---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:49
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: el
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Java Digital Signature Library - GroupDocs.Signature"
head_description: "Ενισχύστε τις εφαρμογές Java με ηλεκτρονικές υπογραφές με το GroupDocs.Signature. Υπογράψτε επαγγελματικά έγγραφα γρήγορα και χωρίς κόπο."

############################# Header ############################
title: "Υπογράψτε έγγραφα<br>μέσω Java API"
description: "Υπογράψτε ψηφιακά έγγραφα και εικόνες σε οποιαδήποτε πλατφόρμα χρησιμοποιώντας τα ευέλικτα API και τις λύσεις που βασίζονται σε εφαρμογές για προγραμματιστές και τελικούς χρήστες."
words:
  for: "Για"

actions:
  main: "Δωρεάν λήψη Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-signature/"
  alt: "Αδειοδότηση"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java"
  title: "Είστε έτοιμοι να ξεκινήσετε;"
  description: "Δοκιμάστε τις δυνατότητες GroupDocs.Signature δωρεάν ή ζητήστε άδεια"

release:
  title: "Κυκλοφόρησε η έκδοση {0}"
  notes: "Δείτε τι νέο υπάρχει"
  downloads: "Λήψεις"

code:
  title: "Υπογραφή αρχείων PDF σε Java"
  more: "Περισσότερα παραδείγματα"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Java"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-signature</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Επιλέξτε έγγραφο PDF
    Signature signature = new Signature("sample.pdf");
    
    // Δώστε κείμενο
    TextSignOptions options = 
        new TextSignOptions("John Smith");
    options.setForeColor(Color.RED);

    // Υπογράψτε το έγγραφο και αποθηκεύστε στο αρχείο
    signature.sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Επισκόπηση GroupDocs.Signature"
  description: "API για την εκτέλεση υπογραφής εγγράφων και σχετικών λειτουργιών σε εφαρμογές Java"
  features:
    # feature loop
    - title: "Βελτιωμένα επαγγελματικά έγγραφα με ψηφιακές υπογραφές σε Java"
      content: "Γρήγορη και προσαρμόσιμη υπογραφή: Το GroupDocs.Signature για Java προσφέρει ένα ευρύ φάσμα επιλογών ψηφιακής υπογραφής για αρχεία PDF, εικόνες και έγγραφα του Office. Μπορείτε να χρησιμοποιήσετε κείμενο, γραμμωτούς κώδικες, κωδικούς QR, ψηφιακά πιστοποιητικά, εικόνες ή κρυφά μεταδεδομένα. Η επεξεργασία των εγγράφων είναι γρήγορη και αποτελεσματική."

    # feature loop
    - title: "Χειρισμός υπογεγραμμένων εγγράφων"
      content: "Η προηγμένη επεξεργασία εγγράφων περιλαμβάνει ισχυρές λειτουργίες σε υπογεγραμμένα έγγραφα χρησιμοποιώντας GroupDocs.Signature για Java. Μπορείτε να αναζητήσετε και να επικυρώσετε υπογραφές που έχουν προστεθεί σε επιχειρηματικά έγγραφα χρησιμοποιώντας διάφορα χρήσιμα κριτήρια. Επιπλέον, μπορείτε να αποκτήσετε πρόσβαση σε λεπτομερείς πληροφορίες σχετικά με το έγγραφο ή να λάβετε εικόνες προεπισκόπησης των σελίδων του."

    # feature loop
    - title: "Ποικιλία επιλογών εξόδου"
      content: "Οι ισχυρές επιλογές υπογραφής σάς επιτρέπουν να προσαρμόσετε την έξοδο για έγγραφα που υπογράφονται με GroupDocs.Signature για Java. Μπορείτε να τοποθετήσετε με ακρίβεια οποιαδήποτε υπογραφή σε οποιαδήποτε σελίδα εγγράφου και να διαμορφώσετε την εμφάνισή της με διάφορους τρόπους. Το Java API υποστηρίζει την αποθήκευση υπογεγραμμένων επιχειρηματικών εγγράφων σε πολλές υποστηριζόμενες μορφές και παρέχει επιλογές για την ασφάλειά τους με κωδικούς πρόσβασης."

############################# Platforms ############################
platforms:
  enable: true
  title: "Ανεξαρτησία πλατφόρμας"
  description: "Το GroupDocs.Signature για Java υποστηρίζει τα ακόλουθα λειτουργικά συστήματα, πλαίσια και διαχειριστές πακέτων"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Υποστηριζόμενες μορφές αρχείων"
  description: |
    Το GroupDocs.Signature για Java υποστηρίζει λειτουργίες με τις ακόλουθες [μορφές αρχείων](https://docs.groupdocs.com/signature/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Μορφές Microsoft Office
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### Εικόνες & Άλλες Μορφές
        * **Φορητός:** PDF
        * **εικόνες:** JPG, BMP, PNG, TIFF, GIF, DICOM, WEBP
        * **Άλλες μορφές γραφείου:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### Άλλες μορφές
        * **Ιστός:** HTML, MHTML
        * **Αρχεία:** ZIP, TAR, 7Z
        * **Πιστοποιητικά:** PFX

############################# Features ############################
features:
  enable: true
  title: "Λειτουργίες GroupDocs.Signature"
  description: "Υπογραφή αρχείων PDF, εγγράφων γραφείου και εικόνων με ψηφιακές υπογραφές"

  items:
    # feature loop
    - icon: "sign"
      title: "Προσθήκη υπογραφών"
      content: "Υπογράψτε ένα έγγραφο χρησιμοποιώντας διάφορους υποστηριζόμενους τύπους υπογραφής τοποθετώντας μια ψηφιακή υπογραφή ακριβώς σε οποιαδήποτε θέση σε οποιαδήποτε σελίδα."

    # feature loop
    - icon: "custom"
      title: "Προσαρμογή αποτελεσμάτων"
      content: "Προσαρμόστε την εμφάνιση της υπογραφής προσαρμόζοντας το χρώμα, τη γραμματοσειρά, το περίγραμμα, την περιστροφή και άλλες λειτουργίες για να επιτύχετε το επιθυμητό αποτέλεσμα."

    # feature loop
    - icon: "password"
      title: "Προστασία εγγράφων με κωδικό πρόσβασης"
      content: "Για πολλούς υποστηριζόμενους τύπους εγγράφων, μπορείτε να προστατεύσετε το υπογεγραμμένο έγγραφο με κωδικό πρόσβασης."

    # feature loop
    - icon: "protect"
      title: "Αποτροπή μη εξουσιοδοτημένων αλλαγών"
      content: "Προστατέψτε σημαντικά επιχειρηματικά έγγραφα που υπογράφονται με ψηφιακό πιστοποιητικό από μη εξουσιοδοτημένες τροποποιήσεις."

    # feature loop
    - icon: "convert"
      title: "Λήψη αποτελεσμάτων σε επιθυμητές μορφές"
      content: "Αποκτήστε εύκολα υπογεγραμμένα αρχεία αποτελεσμάτων σε οποιαδήποτε υποστηριζόμενη μορφή. Μπορείτε επίσης να μετατρέψετε έγγραφα MS Word σε PDF χωρίς κόπο."

    # feature loop
    - icon: "preview"
      title: "Προεπισκόπηση εγγράφου"
      content: "Αποθηκεύστε οποιαδήποτε σελίδα ενός εγγράφου ως εικόνα για μελλοντική επεξεργασία."

    # feature loop
    - icon: "search"
      title: "Ψάχνοντας για υπογραφές"
      content: "Είναι δυνατό να λάβετε πληροφορίες σχετικά με υπογραφές που έχουν προστεθεί προηγουμένως σε συγκεκριμένα έγγραφα."

    # feature loop
    - icon: "validate"
      title: "Επικύρωση εγγράφων"
      content: "Επικυρώστε την ορθότητα των υπογραφών σε οποιοδήποτε υπογεγραμμένο έγγραφο."

    # feature loop
    - icon: "update"
      title: "Διαχείριση υπογραφών"
      content: "Μόλις τοποθετηθεί μια υπογραφή σε μια σελίδα εγγράφου, μπορεί να διαγραφεί, να μετακινηθεί ή να ενημερωθεί ανάλογα με τις ανάγκες."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Δείγματα κωδικών"
  description: "Ορισμένοι χρησιμοποιούν περιπτώσεις τυπικών GroupDocs.Signature για λειτουργίες Java"
  items:
    # code sample loop
    - title: "Βελτιώστε το έγγραφο PDF με κωδικό QR"
      content: |
        Η βελτίωση των επιχειρηματικών διαδικασιών με την προσθήκη [QR-codes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) σε συγκεκριμένες σελίδες εγγράφων PDF μπορεί να είναι πολύτιμη. Υπάρχει ένα παράδειγμα για το πώς μπορείτε να προσθέσετε έναν κωδικό QR χρησιμοποιώντας το GroupDocs.Signature για Java.
        {{< landing/code title="Βελτιώστε το έγγραφο PDF με κωδικό QR">}}
        ```java {style=abap}
        // Φορτώστε το έγγραφο για υπογραφή
        Signature signature = new Signature("file_to_sign.pdf");
        
        // Δημιουργήστε επιλογές κωδικού QR με προκαθορισμένο κείμενο
        QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Διαμορφώστε τον τύπο και τη θέση κωδικοποίησης κώδικα QR στη σελίδα
        options.setEncodeType(QrCodeTypes.QR);
        options.setLeft(100);
        options.setTop(100);

        // Υπογράψτε το έγγραφο και αποθηκεύστε το ως αρχείο αποτελεσμάτων
        signature.sign("file_with_QR.pdf", options);
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Χρησιμοποιήστε ψηφιακή υπογραφή για την προστασία ενός DOCX"
      content: |
        Μπορείτε να [Διασφαλίστε ένα έγγραφο](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) χρησιμοποιώντας προσωπικές ή εταιρικές υπογραφές που είναι αποθηκευμένες ως ψηφιακά πιστοποιητικά. Τα έγγραφα που είναι ασφαλισμένα με πιστοποιητικό δεν μπορούν να τροποποιηθούν χωρίς να ακυρωθεί η υπογραφή.
        {{< landing/code title="Χρησιμοποιήστε ψηφιακή υπογραφή για την προστασία ενός DOCX">}}
        ```java {style=abap}   
        // Φορτώστε το έγγραφο που πρόκειται να υπογραφεί ψηφιακά
        Signature signature = new Signature("file_to_sign.docx");
        
        // Καθορίστε τις επιλογές ψηφιακής υπογραφής και δώστε τη διαδρομή προς το αρχείο πιστοποιητικού
        DigitalSignOptions options = new DigitalSignOptions("certificate.pfx");

        // Ορίστε τον κωδικό πρόσβασης του πιστοποιητικού
        options.setPassword("1234567890");

        // Υπογράψτε το έγγραφο και αποθηκεύστε το στην επιθυμητή διαδρομή
        signature.sign("digitally_signed.docx", options);
        ```
        {{< /landing/code >}}

---
