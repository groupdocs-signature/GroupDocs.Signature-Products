---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Signature"
product_tag: "signature"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "<% "{index-content-java.head_title}" %>"
head_description: "<% "{index-content-java.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-java.title}" %>"
description: "<% "{index-content-java.description}" %>"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
        product: "GroupDocs.Signature"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "<% "{index-content-java.submenu_overview}" %>"

            # button loop
            - link: "#features"
              text: "<% "{index-content-java.submenu_features}" %>"

            # button loop
            - link: "#support"
              text: "<% "{index-content-java.submenu_support}" %>"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "<% "{index-content-java.submenu_live_demo}" %>"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/java"
              text: "<% "{index-content-java.submenu_pricing}" %>"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      <% "{index-content-java.overview_content_1}" %>  

      <% "{index-content-java.overview_content_2}" %>  

      <% "{index-content-java.overview_content_3}" %>
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          <% "{index-content-java.overview_tab1_description}" %>
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "<% "{index-content-java.overview_tab1_left_title}" %>"
          content: |
            * <% "{index-content-java.overview_tab1_left_content_1}" %>
            * <% "{index-content-java.overview_tab1_left_content_2}" %>
            * <% "{index-content-java.overview_tab1_left_content_3}" %>
            * <% "{index-content-java.overview_tab1_left_content_4}" %>
            * <% "{index-content-java.overview_tab1_left_content_5}" %>
            * <% "{index-content-java.overview_tab1_left_content_6}" %>
            * <% "{index-content-java.overview_tab1_left_content_7}" %>
      
      ## TAB TWO ##
      tab_two:
        description: |
          <% "{index-content-java.overview_tab2_description} [{index-content.supported_formats}](https://docs.groupdocs.com/signature/java/supported-document-formats/)" %>

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF, TXT
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
                * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM

        right:
          enable: true
          table:
            # table loop
            - title: "Images & Other Formats"
              content: |
                * **<% "{index-content-java.overview_tab2_right_content_1}" %>**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **<% "{index-content-java.overview_tab2_right_content_2}" %>**: EMF, WMF, CMX
                * **<% "{index-content-java.overview_tab2_right_content_3}" %>**: PDF
                * **<% "{index-content-java.overview_tab2_right_content_4}" %>**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **<% "{index-content-java.overview_tab2_right_content_5}" %>**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          <% "{index-content-java.overview_tab3_description}" %>
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "<% "{index-content-java.overview_tab3_left_title_1}" %>"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "<% "{index-content-java.overview_tab3_left_title_2}" %>"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "<% "{index-content-java.overview_tab3_right_title_1}" %>"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "<% "{index-content-java.overview_tab3_right_title_2}" %>"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "<% "{index-content-java.features_title}" %>"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "<% "{index-content-java.features_content_1}" %>"

      # feature loop
      - icon: "fas fa-eye"
        content: "<% "{index-content-java.features_content_2}" %>"

      # feature loop
      - icon: "fas fa-bolt"
        content: "<% "{index-content-java.features_content_3}" %>"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "<% "{index-content-java.features_content_4}" %>"

      # feature loop
      - icon: "fas fa-code"
        content: "<% "{index-content-java.features_content_5}" %>"

      # feature loop
      - icon: "fas fa-cloud"
        content: "<% "{index-content-java.features_content_6}" %>"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "<% "{index-content-java.features_content_7}" %>"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "<% "{index-content-java.features_content_8}" %>"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "<% "{index-content-java.features_content_9}" %>"

      # feature loop
      - icon: "fas fa-border-all"
        content: "<% "{index-content-java.features_content_10}" %>"

      # feature loop
      - icon: "fas fa-wrench"
        content: "<% "{index-content-java.features_content_11}" %>"

      # feature loop
      - icon: "fas fa-columns"
        content: "<% "{index-content-java.features_content_12}" %>"

      # feature loop
      - icon: "fas fa-file-word"
        content: "<% "{index-content-java.features_content_13}" %>"

      # feature loop
      - icon: "fas fa-envelope"
        content: "<% "{index-content-java.features_content_14}" %>"

      # feature loop
      - icon: "fas fa-print"
        content: "<% "{index-content-java.features_content_15}" %>"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "<% "{index-content-java.features_content_16}" %>"

      # feature loop
      - icon: "fas fa-lock"
        content: "<% "{index-content-java.features_content_17}" %>"

      # feature loop
      - icon: "fas fa-file-code"
        content: "<% "{index-content-java.features_content_18}" %>"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "<% "{index-content-java.features_content_19}" %>"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "<% "{index-content-java.features_content_20}" %>"

      # feature loop
      - icon: "fas fa-heading"
        content: "<% "{index-content-java.features_content_21}" %>"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "<% "{index-content-java.features_content_22}" %>"

      # feature loop
      - icon: "fas fa-cube"
        content: "<% "{index-content-java.features_content_23}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-java.features_content_24}" %>"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-java.features_content_25}" %>"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-java.features_content_26}" %>"

       # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-java.features_content_27}" %>"

    more_feature:
      # more_feature_loop
      - title: "<% "{index-content-java.more_feature_1_title}" %>"
        content: |
          <% "{index-content-java.more_feature_1_content}" %>

          ```java
          Signature signature = new Signature("sample.pdf");

          TextSignOptions options = new TextSignOptions("John Smith");
          // <% "{index-content-java.more_feature_1_comment_1}" %>
          options.setLeft(100);
          options.setTop(100);
          
          // <% "{index-content-java.more_feature_1_comment_2}" %>
          options.setWidth(100);
          options.setHeight(30);

          // <% "{index-content-java.more_feature_1_comment_3}" %>
          options.setForeColor(Color.RED);
          SignatureFont signatureFont = new SignatureFont();
          signatureFont.setSize(12);
          signatureFont.setFamilyName("Comic Sans MS");
          options.setFont(signatureFont);
          options.setSignatureImplementation(TextSignatureImplementation.Sticker)

          // <% "{index-content-java.more_feature_1_comment_4}" %>
          signature.sign("sample_signed.pdf", options);
          ```

      # more_feature_loop
      - title: "<% "{index-content-java.more_feature_2_title}" %>"
        content: |
          <% "{index-content-java.more_feature_2_content_1}" %>

          <% "{index-content-java.more_feature_2_content_2}" %>

      # more_feature_loop
      - title: "<% "{index-content-java.more_feature_3_title}" %>"
        content: |
          <% "{index-content-java.more_feature_3_content_1}" %>  

          <% "{index-content-java.more_feature_3_content_2}" %>

      # more_feature_loop
      - title: "<% "{index-content-java.more_feature_4_title}" %>"
        content: |
          <% "{index-content-java.more_feature_4_content}" %>

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "<% "{index-content-java.solutions_title}" %>"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
          product: "GroupDocs.Signature"
          platform: ".NET"
          link: "/signature/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---