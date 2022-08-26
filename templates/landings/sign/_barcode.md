---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: <% get "Operation" %>
signaturetype: <% get "Signaturetype" %>
codetype: <% get "Codetype" %>
fileformat: <% get "Fileformat" %>
productName: <% get "ProductName" %>
lang: <% lower ( get "lang") %>
productCode: <% lower ( get "ProductCode") %>
otherformats: <% get "OtherFormats" %>
breadcrumb: Put <% get "Barcodetype" %> <% get "Signaturetype" %> signature on <% get "Fileformat" %> for <% get "ProgLang" %>

############################# Head ############################
head_title: "<% "{barcode-content-sign.meta_title}" %>"
head_description: "<% "{barcode-content-sign.meta_description}" %>"

############################# Header ############################
title: "<% "{barcode-content-sign.h1}" %>"
description: "<% "{barcode-content-sign.h2}" %>"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "<% get "ProductFullName" %>"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-signature-<% get "ProductCode" %>.png"
        product: "GroupDocs.Signature"
        platform: "<% get "ProductName" %>"



############################# About ############################
about:
    enable: true
    title: "<% "{about-sign.title}" %>"
    content: |
        <% "{about-sign.barcode-content}" %>
    

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{steps-sign.title_left}" %>"
    content_left: |
        <% "{steps-sign.content_left.description}" %>
        
        * <% "{steps-sign.content_left.step_1}" %>
        * <% "{steps-sign.content_left.step_2}" %>
        * <% "{steps-sign.content_left.step_3}" %>

    title_right: "System Requirements"
    content_right: |
        <% "{steps-sign.content_right.description}" %>

        * <% "{steps-sign.content_right.step_1}" %>
        * <% "{steps-sign.content_right.step_2}" %>
        * <% get "Runtime" %>
        * <% "{steps-sign.content_right.step_3}" %>
         
    code: |
        ```<% dict "products.{product}.syntax" %>    
        <% include "..\\..\\examples\\{operation}\\_{Signaturetype}_{product}.md" %>
        ```

############################# Demos ############################
demos:
    enable: true
    title: "<% "{demos-sign.title}" %>"
    content: |
       <% "{demos-sign.content}" %>

        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "fas fa-barcode"
          title: "About <% get "Codetype" %> Barcode"
          content: |
            <% get "CodeDetails" %>
          characterset: |
             <% get "CodeCharacterSet" %>
          textcapacity: |
             <% get "CodeTextCapacity" %>
          image: |
             <% get "CodeImage" %>

          link: ""

############################# More Formats ############################
more_formats:
    enable: true
    title: "Signing Other Document Formats with <% get "Codetype" %> <% get "Signaturetype" %> using <% get "ProgLang" %>"
    content: |
        <% get "ProductName" %> <% get "Codetype" %> <% get "Signaturetype" %> signatures management API for documents and images. Add <% get "Codetype" %> <% get "Signaturetype" %> signatures to some of the popular file formats as stated below.
    format: 
           
       
back_to_top:
    enable: true
---