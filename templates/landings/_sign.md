---
############################# Static ############################
layout: "auto-gen"
date: 2022-03-01T15:12:22
draft: false
otherformats: <% get "OtherFormats" %>
breadcrumb: Create <% get "SIGNATURETYPE" %> signature on <% get "FILEFORMAT" %> for <% get "ProgLang" %>

############################# Head ############################
head_title: "<% "{content-sign.meta_title}" %>"
head_description: "<% "{content-sign.meta_description}" %>"

############################# Header ############################
title: "<% "{content-sign.h1}" %>"
description: "<% "{content-sign.h2}" %>"
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
        <% "{about-sign.content}" %>
    

overview:
    enable: true
    title: "<% "{overview-sign.title}" %>"
    content: |
        <% "{overview-sign.description1}" %>
        <% "{overview-sign.description2}" %> 
        
        <% "{overview-sign.sign_options_desc}" %>

        * <% "{overview-sign.sign_options_item_1}" %>;
        * <% "{overview-sign.sign_options_item_2}" %>;
        * <% "{overview-sign.sign_options_item_3}" %>.
        
        <% "{overview-sign.sign_saving_desc}" %>

        * <% "{overview-sign.sign_saving_item_1}" %>;
        * <% "{overview-sign.sign_saving_item_2}" %>.

        <% "{overview-sign.summary}" %>


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
        <% include "..\\examples\\_sign_{SIGNATURETYPE}_{product}.md" %>
        ```

demos:
    enable: true
    title: "<% "{demos-sign.title}" %>"
    content: |
       <% "{demos-sign.content}" %>
          

more_formats:
    enable: true
    title: "<% "{more_formats.title}" %>"
    content: "<% "{more_formats.content}" %>"
       
       
back_to_top:
    enable: true
---