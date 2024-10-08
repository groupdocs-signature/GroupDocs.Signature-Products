<% configRef "..\\..\\configs\\qrcode\\format_python_img.yml" %>
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
platform: "Python via .NET"
platform_tag: "python-net"

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
      platform: "python-net"
      copy_title: "<% "{common-content.format-code.copy_title}" %>"
      result_enable: true
      result_link: "/examples/signature/signature_all.pdf"
      result_title: "<% "{common-content.format-code.result_title}" %>"
      install:
        command: "pip install groupdocs-signature-net"
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
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # <% "{examples.comment_1}" %>
            with sg.Signature('input.<% get "fileformat" %>') as signature:

                # <% "{examples.comment_2}" %>
                options = sg.QrCodeSignOptions("Text Content")

                # <% "{examples.comment_3}" %>
                options.EncodeType = sg.QrCodeTypes.QR
                options.Left = 50
                options.Top = 150

                # <% "{examples.comment_4}" %>
                result = signature.Sign("output.<% get "fileformat" %>", options)
        ```                 

############################# More features ############################
more_features:
  enable: true
  title: "<% "{more_features.title}" %>"
  description: "<% "{more_features.description}" %>"
  image: "/img/signature/features_qrcode.webp" # 500x500 px
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
      
  code_samples_ext:
    # code sample ext loop
    - title: "<% "{code_1.title}" %>"
      content: |
        <% "{code_1.content}" %>
      code:
        title: "Python"
        content: |
          ```python {style=abap}
          import groupdocs.signature as sg

          def run():

              # <% "{code_1.comment_1}" %>
              with sg.Signature('input.<% get "fileformat" %>') as signature:

                    # <% "{code_1.comment_2}" %>
                    options = sg.QrCodeSignOptions("Archived on July 11, 2019")

                    # <% "{code_1.comment_3}" %>
                    options.VerticalAlignment = sg.Domain.VerticalAlignment.Top
                    options.HorizontalAlignment = sg.Domain.HorizontalAlignment.Right

                    # <% "{code_1.comment_4}" %>
                    options.Margin = sg.Padding()
                    options.Margin.Top = 20
                    options.Margin.Right = 20

                    # <% "{code_1.comment_5}" %>
                    options.ForeColor = sg.Color.Red

                    # <% "{code_1.comment_6}" %>
                    options.Font = sg.SignatureFont()
                    options.Font.Size = 12
                    options.Font.FamilyName = "Comic Sans MS"

                    # <% "{code_1.comment_7}" %>
                    options.Background = sg.Background()
                    options.Background.Color = Color.LimeGreen
                    options.Background.Transparency = 0.5
                    options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                    # <% "{code_1.comment_8}" %>
                    result = signature.Sign("output.<% get "fileformat" %>", options)
          ```
        platform: "python-net"
        copy_title: "<% "{common-content.format-code.copy_title}" %>"
        install:
          command: "pip install groupdocs-signature-net"
          copy_tip: "<% "{common-content.format-code.copy_tip}" %>"
          copy_done: "<% "{common-content.format-code.copy_done}" %>"
        top_links:
          #  loop
          - title: "<% "{common-content.format-code.result_title_bottom}" %>"
            icon: "download"
            link: "/examples/signature/formats/signature_<% get "OperationLow" %>.<% get "fileformat" %>"
        links:
          #  loop
          - title: "<% "{common-content.format-code.links.title_1}" %>"
            link: "<% get "MoreLink" %>"
          #  loop
          - title: "<% "{common-content.format-code.links.title_2}" %>"
            link: "<% get "DocsUrl" %>"
            

            


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
<% include "..\\..\\data\\operations_others_noimg.md" %>

############################# More Formats ########################
more_formats:
    enable: true
    title: "<% (dict "formats.title") %>"
    exclude: "<% get "FileFormatUp" %>"
    description: "<% (dict "formats.description") %>"
<% include "..\\..\\data\\format_others.md" %>

---