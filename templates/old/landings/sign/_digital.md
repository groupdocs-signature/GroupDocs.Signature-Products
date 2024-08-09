---
############################# Static ############################
layout: "auto-gen-signature"
date: 2022-03-01T15:12:22
draft: false
operation: <% get "Operation" %>
signaturetype: <% get "Signaturetype" %>
fileformat: <% get "Fileformat" %>
productName: <% get "ProductName" %>
lang: <% lower ( get "lang") %>
productCode: <% lower ( get "ProductCode") %>
otherformats: <% get "OtherFormats" %>
breadcrumb: Put <% get "Signaturetype" %> signature on <% get "Fileformat" %> for <% get "ProgLang" %>

############################# Head ############################
head_title: "<% "{digital-content.meta_title}" %>"
head_description: "<% "{digital-content.meta_description}" %>"

############################# Header ############################
title: "<% "{digital-content.h1}" %>"
description: "<% "{digital-content.h2}" %>"
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
    title: "<% "{digital-about.title}" %>"
    content: |
        <% "{digital-about.content}" %>
    

############################# Steps ############################
steps:
    enable: true
    title_left: "<% "{digital-steps.title}" %>"
    content_left: |
        <% "{digital-steps.content.description}" %>
        
        * <% "{digital-steps.content.step_1}" %>
        * <% "{digital-steps.content.step_2}" %>
        * <% "{digital-steps.content.step_3}" %>

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