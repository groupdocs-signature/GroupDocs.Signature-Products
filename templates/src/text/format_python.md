<% configRef "..\\..\\configs\\text\\format_python.yml" %>
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
      result_link: "/examples/signature_all.pdf"
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
                options = sg.TextSignOptions("John Smith")

                # <% "{examples.comment_3}" %>
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 14
                options.Font.FamilyName = "Comic Sans MS"

                # <% "{examples.comment_4}" %>
                result = signature.Sign("output.<% get "fileformat" %>", options)
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

    # feature loop
    - title: "<% "{more_features.feature_4.title}" %>"
      content: "<% "{more_features.feature_4.content}" %>"
      
  code_samples:
    # code sample loop
    - title: "<% "{code_1.title}" %>"
      content: |
        <% "{code_1.content}" %>
        {{< landing/code title="C#">}}
        ```python {style=abap}
        import groupdocs.signature as sg

        def run():

            # <% "{code_1.comment_1}" %>
            with sg.Signature('input.<% get "fileformat" %>') as signature:

                # <% "{code_1.comment_2}" %>
                options = sg.TextSignOptions("Rescheduled to 03/04/2025")

                # <% "{code_1.comment_3}" %>
                options.Left = 100
                options.Top = 100
                options.Width = 100
                options.Height = 30

                # <% "{code_1.comment_4}" %>
                options.Margin = sg.Padding()
                options.Margin.Top = 20
                options.Margin.Right = 20

                # <% "{code_1.comment_5}" %>
                options.ForeColor = sg.Color.Red
                options.Font = sg.SignatureFont()
                options.Font.Size = 12
                options.Font.FamilyName = "Comic Sans MS"

                # <% "{code_1.comment_6}" %>
                options.Border = sg.Border()
                options.Border.Color = sg.Color.IndianRed
                options.Border.DashStyle = sg.DashStyle.DashLongDashDot
                options.Border.Transparency = 0.5
                options.Border.Visible = True
                options.Border.Weight = 2

                # <% "{code_1.comment_7}" %>
                options.Background = sg.Background()
                options.Background.Color = sg.Color.LimeGreen
                options.Background.Transparency = 0.5
                options.Background.Brush = sg.LinearGradientBrush(sg.Color.LimeGreen, sg.Color.DarkGreen)

                # <% "{code_1.comment_8}" %>
                options.RotationAngle = 45

                # <% "{code_1.comment_9}" %>
                options.SignatureImplementation = sg.TextSignatureImplementation.Image

                # <% "{code_1.comment_10}" %>
                result = signature.Sign("output.<% get "fileformat" %>", options)
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