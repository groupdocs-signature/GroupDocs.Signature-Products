<% configRef "..\\..\\configs\\text\\format_nodejs.yml" %>
<% include "..\\..\\data\\format_data.md" %>

---
############################# Static ############################
layout: "format"
date:  <% date "utcnow" %>
draft: false
lang: <% lower ( get "lang") %>
format: <% get "FileformatCap" %>
product: "Signature"
product_tag: "signature"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "<% (dict "head.title") %>"
head_description: "<% (dict "head.description") %>"

############################# Header ############################
title: "<% (dict "header.title") %>" 
description: "<% (dict "header.description") %>"
subtitle: "<% (dict "header.subtitle") %>" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "<% (dict "header.action_title") %>"
      link: "<% get "ReleaseDownloads" %>"
      
############################# About ############################
about:
    enable: true
    title: "<% (dict "about.title") %>"
    link: "/signature/<% get "ProdCode" %>/"
    link_title: "<% "{common-content.texts.learn_more}" %>"
    picture: "about_signature.svg" # 480 X 400
    content: |
       <% (dict "about.content") %>

############################# Steps ############################
steps:
    enable: true
    title: "<% "{steps.title}" %>"
    content: |
      <% "{steps.content.title}" %>
      
      1. <% "{steps.content.step_1}" %>
      2. <% "{steps.content.step_2}" %>
      3. <% "{steps.content.step_3}" %>
      4. <% "{steps.content.step_4}" %>
   
    code:
      platform: "nodejs-java"
      copy_title: "<% "{common-content.format-code.copy_title}" %>"
      install:
        command: "npm i @groupdocs/groupdocs.signature"
        copy_tip: "<% "{common-content.format-code.copy_tip}" %>"
        copy_done: "<% "{common-content.format-code.copy_done}" %>"
      links:
        #  loop
        - title: "<% "{common-content.format-code.links.title_1}" %>"
          link: "<% get "MoreLink" %>"
        #  loop
        - title: "<% "{common-content.format-code.links.title_2}" %>"
          link: "<% get "DocsUrl" %>"
          
      content: |
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')

        // <% "{examples.comment_1}" %>
        const signature = new signatureLib.Signature('input.<% get "fileformat" %>');

        // <% "{examples.comment_2}" %>
        const options = new signatureLib.TextSignOptions('John Smith');

        // <% "{examples.comment_3}" %>
        options.setForeColor(new signatureLib.Color(255, 0, 0));
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);
        
        // <% "{examples.comment_4}" %>
        const result = signature.sign('output.<% get "fileformat" %>', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "<% "{more_features.title}" %>"
  description: "<% "{more_features.description}" %>"
  image: "/img/signature/features_text.webp" # 500x500 px
  image_description: "<% "{more_features.image_description}" %>"
  features:
    # feature loop
    - title: "<% "{more_features.feature_1.title}" %>"
      content: "<% "{more_features.feature_1.content}" %>"

    # feature loop
    - title: "<% "{more_features.feature_2.title}" %>"
      content: "<% "{more_features.feature_2.content}" %>"

    # feature loop
    - title: "<% "{more_features.feature_3.title}" %>"
      content: "<% "{more_features.feature_3.content}" %>"
      
  code_samples:
    # code sample loop
    - title: "<% "{more_features.code_1.title}" %>"
      content: |
        <% "{more_features.code_1.content}" %>
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // <% "{more_features.code_1.comment_1}" %>
        const signature = new signatureLib.Signature('input.<% get "fileformat" %>');

        // <% "{more_features.code_1.comment_2}" %>
        const options = new signatureLib.TextSignOptions('Rescheduled to 03/04/2025');

        // <% "{more_features.code_1.comment_3}" %>
        options.setLeft(100);
        options.setTop(100);
        options.setWidth(100);
        options.setHeight(30);

        // <% "{more_features.code_1.comment_4}" %>
        const padding = new signatureLib.Padding();
        padding.setBottom(20);
        padding.setRight(20);
        options.setMargin(padding);

        // <% "{more_features.code_1.comment_5}" %>
        options.setForeColor(signatureLib.Color.RED);
        const signatureFont = new signatureLib.SignatureFont();
        signatureFont.setSize(12);
        signatureFont.setFamilyName('Comic Sans MS');
        options.setFont(signatureFont);

        // <% "{more_features.code_1.comment_6}" %>
        const border = new signatureLib.Border();
        border.setColor(signatureLib.Color.GREEN);
        border.setDashStyle(signatureLib.DashStyle.DashLongDashDot);
        border.setTransparency(0.5);
        border.setVisible(true);
        border.setWeight(2);
        options.setBorder(border);

        // <% "{more_features.code_1.comment_7}" %>
        const background = new signatureLib.Background();
        background.setColor(signatureLib.Color.LIGHT_GRAY);
        background.setTransparency(0.5);
        const brush = new signatureLib.LinearGradientBrush
            (signatureLib.Color.GREEN, signatureLib.Color.DARK_GRAY, 0);
        background.setBrush(brush);
        options.setBackground(background);

        // <% "{more_features.code_1.comment_8}" %>
        options.setRotationAngle(45);

        // <% "{more_features.code_1.comment_9}" %>
        options.setSignatureImplementation(signatureLib.TextSignatureImplementation.Image);
        
        // <% "{more_features.code_1.comment_5}" %>
        const result = signature.sign('output.<% get "fileformat" %>', options);
        ```
        {{< /landing/code >}}


############################# Actions ############################

actions:
  enable: true
  title: "<% "{common-content.format-actions.title}" %>"
  description: "<% "{common-content.format-actions.description}" %>"
  items:
    #  loop
    - title: "<% "{common-content.format-actions.comment_1}" %>"
      link: "<% get "ReleaseDownloads" %>"
      color: "red"
        #  loop
    - title: "<% "{common-content.format-actions.comment_2}" %>"
      link: "<% get "PricesUrl" %>"
      color: "light"


############################# More Formats #####################
more_formats:
    enable: true
    title: "<% (dict "formats.title") %>"
    exclude: "<% get "FileFormatUp" %>"
    description: "<% (dict "formats.description") %>"
<% include "..\\..\\data\\format_others.md" %>

---