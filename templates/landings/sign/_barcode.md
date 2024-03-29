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
head_title: "<% "{barcode-content.meta_title}" %>"
head_description: "<% "{barcode-content.meta_description}" %>"

############################# Header ############################
title: "<% "{barcode-content.h1}" %>"
description: "<% "{barcode-content.h2}" %>"
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
    title: "<% "{barcode-about.title}" %>"
    content: |
        <% "{barcode-about.content}" %>
    

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{barcode-steps.title}" %>"
    content_left: |
        <% "{barcode-steps.content.description}" %>
        
        * <% "{barcode-steps.content.step_1}" %>
        * <% "{barcode-steps.content.step_2}" %>
        * <% "{barcode-steps.content.step_3}" %>

    title_right: " <% "{system-requirements.title}" %>"
    content_right: |
        <% "{system-requirements.content.description}" %>

        * <% "{system-requirements.content.step_1}" %>
        * <% "{system-requirements.content.step_2}" %>
        * <% get "Runtime" %>
        * <% "{system-requirements.content.step_3}" %>
         
    code: |
        ```<% dict "products.{product}.syntax" %>    
        <% include "..\\..\\examples\\{operation}\\_{Signaturetype}_{product}.md" %>
        ```

############################# Demos ############################
demos:
    enable: true
    title: "<% "{demos.title}" %>"
    content: |
       <% "{demos.content}" %>

        
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
    title: "<% "{more_formats.title}" %>"
    content: |
        "<% "{more_formats.content}" %>"
    format: 
        
       
back_to_top:
    enable: true
---