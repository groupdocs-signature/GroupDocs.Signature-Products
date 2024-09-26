<% configRef "..\\..\\configs\\stamp\\format_nodejs.yml" %>
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
      result_enable: true
      result_link: "/examples/signature_all.pdf"
      result_title: "<% "{common-content.format-code.result_title}" %>"
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
        const options = new signatureLib.StampSignOptions();

        // <% "{examples.comment_3}" %>
        const outerLine = new signatureLib.StampLine();
        outerLine.setText(" * The Best Company * ");
        outerLine.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        outerLine.getFont().setSize(12);
        outerLine.setHeight(22);
        outerLine.setTextBottomIntent(6);
        outerLine.setTextColor(signatureLib.Color.WHITE);
        outerLine.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine);

        // <% "{examples.comment_4}" %>
        const result = signature.sign('output.<% get "fileformat" %>', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "<% "{more_features.title}" %>"
  description: "<% "{more_features.description}" %>"
  image: "/img/signature/features_stamp.webp" # 500x500 px
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

    # feature loop
    - title: "<% "{more_features.feature_4.title}" %>"
      content: "<% "{more_features.feature_4.content}" %>"
      
  code_samples:
    # code sample loop
    - title: "<% "{code_1.title}" %>"
      content: |
        <% "{code_1.content}" %>
        {{< landing/code title="JavaScript">}}
        ```javascript {style=abap}
        const signatureLib = require('@groupdocs/groupdocs.signature')
        
        // <% "{code_1.comment_1}" %>
        const signature = new signatureLib.Signature('input.<% get "fileformat" %>');

        // <% "{code_1.comment_2}" %>
        const options = new signatureLib.StampSignOptions();

        // <% "{code_1.comment_3}" %>
        options.setHeight(300);
        options.setWidth(300);
        options.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
        options.setHorizontalAlignment(signatureLib.HorizontalAlignment.Right);
        options.setAllPages(true);

        // <% "{code_1.comment_4}" %>
        const outerLine1 = new signatureLib.StampLine();
        outerLine1.setText('* The best choice *');
        outerLine1.setTextRepeatType(signatureLib.StampTextRepeatType.FullTextRepeat);
        const signatureFont1 = new signatureLib.SignatureFont();
        signatureFont1.setSize(12);
        signatureFont1.setFamilyName('Arial');
        outerLine1.setFont(signatureFont1);
        outerLine1.setHeight(30);
        outerLine1.setTextBottomIntent(6);
        outerLine1.setTextColor(signatureLib.Color.WHITE);
        outerLine1.setBackgroundColor(signatureLib.Color.BLUE);
        options.getOuterLines().add(outerLine1);

        // <% "{code_1.comment_5}" %>
        const innerLine1 = new signatureLib.StampLine();
        innerLine1.setText('Company #1');
        innerLine1.setTextColor(signatureLib.Color.RED);
        const signFont1 = new signatureLib.SignatureFont();
        signFont1.setSize(20);
        signFont1.setBold(true);
        innerLine1.setFont(signFont1);
        innerLine1.setHeight(40);
        options.getInnerLines().add(innerLine1);
        
        // <% "{code_1.comment_6}" %>
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


############################# More Operations #####################
more_operations:
    enable: true
    title: "<% (dict "operations.title") %>"
    exclude: "<% get "OperationLow" %>"
    description: "<% (dict "operations.description") %>"
<% include "..\\..\\data\\operations_others.md" %>

############################# More Formats ########################
more_formats:
    enable: true
    title: "<% (dict "formats.title") %>"
    exclude: "<% get "FileFormatUp" %>"
    description: "<% (dict "formats.description") %>"
<% include "..\\..\\data\\format_others.md" %>

---