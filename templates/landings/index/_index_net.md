---
############################# Static ############################
layout: "product"
date: 2022-03-01T15:12:22
draft: false
#operation: <% get "Operation" %>
#signaturetype: <% get "Signaturetype" %>
#fileformat: <% get "Fileformat" %>
#productName: <% get "ProductName" %>
lang: <% lower ( get "lang") %>
#productCode: <% lower ( get "ProductCode") %>
#otherformats: <% get "OtherFormats" %>
#breadcrumb: Put <% get "Signaturetype" %> signature on <% get "Fileformat" %> for <% get "ProgLang" %>
product: "Signature"
product_tag: "signature"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "<% "{index-content-net.head_title}" %>"
head_description: "<% "{index-content-net.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-net.title}" %>"
description: "<% "{index-content-net.description}" %>"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Signature for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-net.png"
        product: "GroupDocs.Signature"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "<% "{index-content-net.submenu_overview}" %>"

            # button loop
            - link: "#features"
              text: "<% "{index-content-net.submenu_features}" %>"

            # button loop
            - link: "#support"
              text: "<% "{index-content-net.submenu_support}" %>"

            # button loop
            - link: "https://products.groupdocs.app/signature"
              text: "<% "{index-content-net.submenu_live_demo}" %>"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/signature/net"
              text: "<% "{index-content-net.submenu_pricing}" %>"

    right:
        link_download: "https://downloads.groupdocs.com/signature"
        link_learn: "https://docs.groupdocs.com/signature/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      <% "{index-content-net.overview_content_1}" %>  

      <% "{index-content-net.overview_content_2}" %>  

      <% "{index-content-net.overview_content_3}" %>
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          <% "{index-content-net.overview_tab1_description}" %>
      
        left:
          enable: true
          icon: "fab fa-html5"
          title: "<% "{index-content-net.overview_tab1_left_title}" %>"
          content: |
            * <% "{index-content-net.overview_tab1_left_content_1}" %>
            * <% "{index-content-net.overview_tab1_left_content_2}" %>
            * <% "{index-content-net.overview_tab1_left_content_3}" %>
            * <% "{index-content-net.overview_tab1_left_content_4}" %>
            * <% "{index-content-net.overview_tab1_left_content_5}" %>
            * <% "{index-content-net.overview_tab1_left_content_6}" %>
            * <% "{index-content-net.overview_tab1_left_content_7}" %>
      
      ## TAB TWO ##
      tab_two:
        description: |
          <% "{index-content-net.overview_tab2_description} [{index-content.supported_formats}](https://docs.groupdocs.com/signature/net/supported-document-formats/)" %>

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
                * **<% "{index-content-net.overview_tab2_right_content_1}" %>**: JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
                * **OpenDocument**: ODT, OTT, OTS, ODS, ODP, OTP, ODG
                * **Jpeg2000**: JP2, JPF, JPX, J2K, J2C, JPM
                * **<% "{index-content-net.overview_tab2_right_content_2}" %>**: EMF, WMF, CMX
                * **<% "{index-content-net.overview_tab2_right_content_3}" %>**: PDF
                * **<% "{index-content-net.overview_tab2_right_content_4}" %>**: CDR, SVG
                * **Adobe Photoshop**: PSD
                * **<% "{index-content-net.overview_tab2_right_content_5}" %>**: DJVU

      ## TAB THREE ##
      tab_three:
        description: |
          <% "{index-content-net.overview_tab3_description}" %>
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "<% "{index-content-net.overview_tab3_left_title_1}" %>"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "<% "{index-content-net.overview_tab3_left_title_2}" %>"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "<% "{index-content-net.overview_tab3_right_title_1}" %>"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "<% "{index-content-net.overview_tab3_right_title_2}" %>"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "<% "{index-content-net.features_title}" %>"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "<% "{index-content-net.features_content_1}" %>"

      # feature loop
      - icon: "fas fa-eye"
        content: "<% "{index-content-net.features_content_2}" %>"

      # feature loop
      - icon: "fas fa-bolt"
        content: "<% "{index-content-net.features_content_3}" %>"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "<% "{index-content-net.features_content_4}" %>"

      # feature loop
      - icon: "fas fa-code"
        content: "<% "{index-content-net.features_content_5}" %>"

      # feature loop
      - icon: "fas fa-cloud"
        content: "<% "{index-content-net.features_content_6}" %>"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "<% "{index-content-net.features_content_7}" %>"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "<% "{index-content-net.features_content_8}" %>"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "<% "{index-content-net.features_content_9}" %>"

      # feature loop
      - icon: "fas fa-border-all"
        content: "<% "{index-content-net.features_content_10}" %>"

      # feature loop
      - icon: "fas fa-wrench"
        content: "<% "{index-content-net.features_content_11}" %>"

      # feature loop
      - icon: "fas fa-columns"
        content: "<% "{index-content-net.features_content_12}" %>"

      # feature loop
      - icon: "fas fa-file-word"
        content: "<% "{index-content-net.features_content_13}" %>"

      # feature loop
      - icon: "fas fa-envelope"
        content: "<% "{index-content-net.features_content_14}" %>"

      # feature loop
      - icon: "fas fa-print"
        content: "<% "{index-content-net.features_content_15}" %>"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "<% "{index-content-net.features_content_16}" %>"

      # feature loop
      - icon: "fas fa-lock"
        content: "<% "{index-content-net.features_content_17}" %>"

      # feature loop
      - icon: "fas fa-file-code"
        content: "<% "{index-content-net.features_content_18}" %>"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "<% "{index-content-net.features_content_19}" %>"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "<% "{index-content-net.features_content_20}" %>"

      # feature loop
      - icon: "fas fa-heading"
        content: "<% "{index-content-net.features_content_21}" %>"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "<% "{index-content-net.features_content_22}" %>"

      # feature loop
      - icon: "fas fa-cube"
        content: "<% "{index-content-net.features_content_23}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_24}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_25}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_26}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_27}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_28}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_29}" %>"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "<% "{index-content-net.features_content_30}" %>"

    more_feature:
      # more_feature_loop
      - title: "<% "{index-content-net.more_feature_1_title}" %>"
        content: |
          <% "{index-content-net.more_feature_1_content}" %>

          ```cs
          using (Signature signature = new Signature("D:\\sample.pdf"))
          {
          TextSignOptions options = new TextSignOptions("John Smith")
          {
          // <% "{index-content-net.more_feature_1_comment_1}" %>
          ForeColor = Color.Red
          };
          // <% "{index-content-net.more_feature_1_comment_2}" %>
          signature.Sign("D:\\signed.pdf", options);
          }
          ```

      # more_feature_loop
      - title: "<% "{index-content-net.more_feature_2_title}" %>"
        content: |
          <% "{index-content-net.more_feature_2_content}" %>

      # more_feature_loop
      - title: "<% "{index-content-net.more_feature_3_title}" %>"
        content: |
          <% "{index-content-net.more_feature_3_content_1}" %>  

          <% "{index-content-net.more_feature_3_content_2}" %>

      # more_feature_loop
      - title: "<% "{index-content-net.more_feature_4_title}" %>"
        content: |
          <% "{index-content-net.more_feature_4_content}" %>

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "<% "{index-content-net.solutions_title}" %>"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Signature for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-signature-java.png"
          product: "GroupDocs.Signature"
          platform: "Java"
          link: "/signature/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---