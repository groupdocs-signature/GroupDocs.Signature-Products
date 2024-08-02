<% configRef "..\\configs\\delete\\format_nodejs.yml" %>
<% include "..\\data\\format_data.md" %>

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
      platform: "net"
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

        // <% "{more_features.code_1.comment_2}" %>
        const options = new signatureLib.TextSearchOptions();
        const signatures = signature.search(signatureLib.TextSignature.class, options);

        // <% "{examples.comment_3}" %>
        if(signatures.size() > 0)
        {
            const textSignature = signatures[0];
            const result = signature.delete('output.<% get "fileformat" %>', textSignature);

            // <% "{examples.comment_4}" %>
            if(result)
            {
                console.log(`\nSignature was deleted successfully`);
            }
        }

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "<% "{more_features.title}" %>"
  description: "<% "{more_features.description}" %>"
  image: "/img/signature/features_delete.webp" # 500x500 px
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
        const result = await signature.delete('output.<% get "fileformat" %>', signatureLib.SignatureType.QrCode);
        if (result.getSucceeded().size() > 0) {

            // <% "{more_features.code_1.comment_3}" %>
            console.log('Following QR-Code signatures were deleted:');
            let number = 1;
            result.getSucceeded().toArray().forEach((o) => {
                const temp = o;
                console.log(`Signature #${number++}: Type: ${temp.getSignatureType()}, 
                Id: ${temp.getSignatureId()}, Text: ${temp.getText()}`);
            });
        }
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
<% include "..\\data\\format_others.md" %>

---