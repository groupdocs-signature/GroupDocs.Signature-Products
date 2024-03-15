---
############################# Static ############################
layout: "landing"
date: 2024-03-15T20:32:51
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Node.js
lang: el
#productCode: nodejs-java
#otherformats: 
#breadcrumb: Put  signature on  for JavaScript
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Digital Signature API - GroupDocs.Signature"
head_description: "Ενσωματώστε ασφαλείς ηλεκτρονικές υπογραφές στις εφαρμογές Node.js με το GroupDocs.Signature. Βελτιώστε τις ροές εργασίας της υπογραφής εγγράφων εύκολα και αποτελεσματικά."

############################# Header ############################
title: "Υπογράψτε έγγραφα<br>με το Node.js API"
description: "Υπογράψτε ψηφιακά έγγραφα και εικόνες σε οποιαδήποτε πλατφόρμα χρησιμοποιώντας τα ευέλικτα API και τις λύσεις που βασίζονται σε εφαρμογές για προγραμματιστές και τελικούς χρήστες."
words:
  for: "Για"

actions:
  main: "Λήψη από το NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.signature/"
  alt: "Αδειοδότηση"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/java/"
  title: "Είστε έτοιμοι να ξεκινήσετε;"
  description: "Δοκιμάστε τις δυνατότητες GroupDocs.Signature δωρεάν ή ζητήστε άδεια"

release:
  title: "Κυκλοφόρησε η έκδοση {0}"
  notes: "Δείτε τι νέο υπάρχει"
  downloads: "Λήψεις"

code:
  title: "Υπογραφή αρχείων PDF από το Node.js"
  more: "Περισσότερα παραδείγματα"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.signature"
  content: |
    ```javascript {style=abap}   
    // Επιλέξτε έγγραφο PDF
    let signature = new Signature("sample.pdf");
    
    // Δώστε κείμενο
    let options = new TextSignOptions("John Smith");
    
    // Σετ χρώματος
    options.ForeColor = Color.Red;
    
    // Υπογράψτε το έγγραφο και αποθηκεύστε στο αρχείο
    signature.Sign("signed.pdf", options);
    
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Επισκόπηση GroupDocs.Signature"
  description: "Βιβλιοθήκη υπογραφής εγγράφων που είναι έτοιμη για χρήση σε εφαρμογές Node.js"
  features:
    # feature loop
    - title: "Λύση Ψηφιακών Υπογραφών για Επιχειρηματικά Έγγραφα με το Node.js"
      content: "Το GroupDocs.Signature for Node.js via Java προσφέρει ένα ολοκληρωμένο σύνολο επιλογών ψηφιακής υπογραφής για PDF, έγγραφα του Office και εικόνες. Διατίθενται κείμενο, γραμμικοί κώδικες, εικόνες, ψηφιακά πιστοποιητικά και μεταδεδομένα. Η απλοποιημένη επεξεργασία εγγράφων εξασφαλίζει αποτελεσματικότητα."

    # feature loop
    - title: "Προηγμένος χειρισμός υπογεγραμμένων εγγράφων"
      content: "Το GroupDocs.Signature σάς δίνει τη δυνατότητα να επεξεργάζεστε υπογεγραμμένα έγγραφα. Αναζήτηση και επικύρωση υπογραφών χρησιμοποιώντας διάφορα κριτήρια. Επιπλέον, εξάγετε λεπτομερείς πληροφορίες εγγράφων ή δημιουργήστε εικόνες προεπισκόπησης σελίδων."

    # feature loop
    - title: "Διαφορετικές μορφές εξόδου"
      content: "Η λύση μας παρέχει εκτεταμένο έλεγχο στη μορφή εξόδου των υπογεγραμμένων εγγράφων. Τοποθετήστε με ακρίβεια τις υπογραφές σε οποιαδήποτε σελίδα και προσαρμόστε την εμφάνισή τους. Αποθηκεύστε υπογεγραμμένα έγγραφα σε πολλές υποστηριζόμενες μορφές και προαιρετικά ασφαλίστε τα με κωδικούς πρόσβασης."

############################# Platforms ############################
platforms:
  enable: true
  title: "Ανεξαρτησία πλατφόρμας"
  description: "Το GroupDocs.Signature for Node.js via Java εκτελεί επεξεργασία εγγράφων με διάφορα λειτουργικά συστήματα"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Υποστηριζόμενες μορφές αρχείων"
  description: |
    Το GroupDocs.Signature for Node.js via Java διευκολύνει τις λειτουργίες για τις [δημοφιλείς μορφές αρχείων](https://docs.groupdocs.com/signature/java/supported-document-formats/).
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
  title: "Χαρακτηριστικά του GroupDocs.Signature"
  description: "Υπογράψτε αρχεία PDF, έγγραφα του Office και εικόνες με ψηφιακές υπογραφές"

  items:
    # feature loop
    - icon: "sign"
      title: "Επιχειρηματικές υπογραφές"
      content: "Χρησιμοποιήστε διάφορους τύπους υπογραφών για την υπογραφή εγγράφων. Τοποθετήστε ψηφιακές υπογραφές με ακρίβεια σε οποιαδήποτε θέση σελίδας."

    # feature loop
    - icon: "custom"
      title: "Προσαρμογή της εμφάνισης υπογραφής"
      content: "Προσαρμόστε τις οπτικές πτυχές των υπογραφών προσαρμόζοντας το χρώμα, τη γραμματοσειρά, τα περιγράμματα, την περιστροφή και πολλά άλλα για να επιτύχετε το επιθυμητό αποτέλεσμα."

    # feature loop
    - icon: "password"
      title: "Έγγραφα που προστατεύονται με κωδικό πρόσβασης"
      content: "Για πολλές υποστηριζόμενες μορφές εγγράφων, προστατέψτε τα υπογεγραμμένα έγγραφα με κωδικό πρόσβασης για πρόσθετη ασφάλεια."

    # feature loop
    - icon: "protect"
      title: "Αποτροπή μη εξουσιοδοτημένων τροποποιήσεων"
      content: "Προστατέψτε τα κρίσιμα επιχειρηματικά έγγραφα που υπογράφονται με ψηφιακά πιστοποιητικά από μη εξουσιοδοτημένες τροποποιήσεις."

    # feature loop
    - icon: "convert"
      title: "Επιθυμητές μορφές εξόδου"
      content: "Λάβετε αβίαστα υπογεγραμμένα έγγραφα σε οποιαδήποτε υποστηριζόμενη μορφή. Μετατρέψτε έγγραφα MS Word σε μορφή PDF με ευκολία."

    # feature loop
    - icon: "preview"
      title: "Προεπισκόπηση εγγράφων"
      content: "Αποθηκεύστε μεμονωμένες σελίδες εγγράφων ως εικόνες για μελλοντικές ανάγκες."

    # feature loop
    - icon: "search"
      title: "Αναζήτηση υπογραφών"
      content: "Ανακτήστε πληροφορίες σχετικά με υπογραφές που έχετε προσθέσει προηγουμένως στα έγγραφά σας."

    # feature loop
    - icon: "validate"
      title: "Επικύρωση εγγράφου"
      content: "Επαληθεύστε τη γνησιότητα των υπογραφών που παρουσιάζονται σε οποιοδήποτε έγγραφο."

    # feature loop
    - icon: "update"
      title: "Διαχείριση υπογραφών"
      content: "Διαγράψτε, μεταφέρετε ή τροποποιήστε τυχόν υπογραφές που έχουν τοποθετηθεί σε οποιαδήποτε σελίδα εγγράφου."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Δείγματα κωδικών"
  description: "Ενδεικτικά παραδείγματα που παρουσιάζουν τυπικές λειτουργίες GroupDocs.Signature for Node.js via Java"
  items:
    # code sample loop
    - title: "Επισημάνετε το PDF με κωδικούς QR"
      content: |
        Η ενσωμάτωση [barcodes](https://docs.groupdocs.com/signature/java/esign-document-with-qr-code-signature/) σε συγκεκριμένες σελίδες εγγράφων PDF μπορεί να βελτιώσει τις επιχειρηματικές διαδικασίες. Αυτή η ενότητα παρέχει ένα παράδειγμα προσθήκης κωδικού QR χρησιμοποιώντας το GroupDocs.Signature for Node.js via Java.
        {{< landing/code title="Πώς να τοποθετήσετε τον κωδικό QR σε PDF.">}}
        ```javascript {style=abap}
        // Φορτώστε το έγγραφο για υπογραφή
        let signature = new Signature("file_to_sign.pdf");
        
        // Δημιουργήστε επιλογές κωδικού QR με προκαθορισμένο κείμενο
        let options = new QrCodeSignOptions("The document is approved by John Smith");
        
        // Διαμορφώστε τον τύπο και τη θέση κωδικοποίησης κώδικα QR στη σελίδα
        options.EncodeType = QrCodeTypes.QR;
        options.Left = 100;
        options.Top = 100;
            
        // Υπογράψτε το έγγραφο και αποθηκεύστε το ως αρχείο αποτελεσμάτων
        signature.Sign("file_with_QR.pdf", options);
        
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Προστασία ενός DOCX με ψηφιακή υπογραφή"
      content: |
        [Προστατέψτε τα έγγραφά σας](https://docs.groupdocs.com/signature/java/esign-document-with-digital-signature/) με υπογραφές που βασίζονται σε ψηφιακά πιστοποιητικά. Η ψηφιακή υπογραφή προστατεύει τα έγγραφα της επιχείρησής σας από την αλλαγή περιεχομένου.
        {{< landing/code title="Ακολουθεί ο τρόπος διασφάλισης της ακεραιότητας του εγγράφου.">}}
        ```javascript {style=abap}   
        // Φορτώστε το έγγραφο που πρόκειται να υπογραφεί ψηφιακά
        let signature = new Signature("file_to_sign.docx");
        
        // Καθορίστε τις επιλογές ψηφιακής υπογραφής και δώστε τη διαδρομή προς το αρχείο πιστοποιητικού
        let options = new DigitalSignOptions("certificate.pfx");

        // Ορίστε τον κωδικό πρόσβασης του πιστοποιητικού
        options.Password = "1234567890";

        // Υπογράψτε το έγγραφο και αποθηκεύστε το στην επιθυμητή διαδρομή
        signature.Sign("digitally_signed.docx", options);

        ```
        {{< /landing/code >}}

---
