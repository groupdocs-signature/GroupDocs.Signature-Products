---
############################# Static ############################
layout: "landing"
date: 2023-09-05T16:50:31
draft: false
#operation: 
#signaturetype: 
#fileformat: 
#productName: Java
lang: hy
#productCode: java
#otherformats: 
#breadcrumb: Put  signature on  for Java
product: "Signature"
product_tag: "signature"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: ".NET, Java, Cloud API-ներ և առցանց փաստաթղթերի ստորագրման հավելվածներ"
head_description: "Ստացեք փաստաթղթի էլեկտրոնային ստորագրության ամբողջական լուծում .NET, Java և ամպի վրա հիմնված հավելվածների համար: Ստորագրեք սովորական փաստաթղթերի ձևաչափերը առցանց՝ օգտագործելով պարզ քաշել և թողնել հնարավորությունը"

############################# Header ############################
title: "{index-content.title_1}<br>{index-content-net.title_2}"
description: "Ստորագրեք թվային փաստաթղթեր և պատկերներ ցանկացած հարթակում՝ օգտագործելով մեր ճկուն API-ները և հավելվածների վրա հիմնված լուծումները ծրագրավորողների և վերջնական օգտագործողների համար:"
words:
  for: "{index-content.words_for}"

actions:
  main: "{index-content-net.actions_main}"
  main_link: "https://www.nuget.org/packages/GroupDocs.Signature"
  alt: "{index-content.actions_alt}"
  alt_link: "https://purchase.groupdocs.com/pricing/signature/net"
  title: "{index-content.actions_title}"
  description: "{index-content.actions_description}"

release:
  title: "{index-content.release_title}"
  notes: "{index-content.release_notes}"
  downloads: "{index-content.release_downloads}"

code:
  title: "{index-content-net.code_title}"
  more: "{index-content.code_more}"
  more_link: "https://github.com/groupdocs-signature/GroupDocs.Signature-for-.NET"
  install: "dotnet add package GroupDocs.Signature"
  content: |
    ```csharp {style=abap}   
    // {index-content.code_comment_1}
    using (Signature signature = new Signature("D:\\sample.pdf"))
    {
        // {index-content.code_comment_2}
        TextSignOptions options = new TextSignOptions("John Smith")
        {
            // {index-content.code_comment_3}
            ForeColor = Color.Red
        };
        // {index-content.code_comment_4}
        signature.Sign("D:\\signed.pdf", options);
     }
    ```

############################# Overview ############################
overview:
  enable: true
  title: "{index-content.overview_title}"
  description: "{index-content-net.overview_description}"
  features:
    # feature loop
    - title: "{index-content-net.overview_feature_1.title}"
      content: "{index-content-net.overview_feature_1.description}"

    # feature loop
    - title: "{index-content-net.overview_feature_2.title}"
      content: "{index-content-net.overview_feature_2.description}"

    # feature loop
    - title: "{index-content-net.overview_feature_3.title}"
      content: "{index-content-net.overview_feature_3.description}"

############################# Platforms ############################
platforms:
  enable: true
  title: "{index-content.platforms_title}"
  description: "{index-content-net.platforms_description}"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "{index-content.formats_title}"
  description: |
    {index-content-net.formats_description}
  groups:
    # group loop
    - color: "green"
      content: |
        ### {index-content.formats_groups.title_1}
        * **Word:**  DOCX, DOC, DOCM, DOT, DOTX, DOTM, RTF
        * **Excel:** XLSX, XLS, XLSM, XLSB, XLTM, XLT, XLTM, XLTX, XLAM, SXC, SpreadsheetML
        * **PowerPoint:** PPT, PPTX, PPS, PPSX, PPSM, POT, POTM, POTX, PPTM
    # group loop
    - color: "blue"
      content: |
        ### {index-content.formats_groups.title_2}
        * **{index-content.formats_groups.format_portable}:** PDF
        * **{index-content.formats_groups.format_images}:** JPG, BMP, PNG, TIFF, GIF, DCM, WEBP
        * **{index-content.formats_groups.format_other_office}:** ODT, OTT, OTS, ODS, ODP, OTP, ODG
      # group loop
    - color: "red"
      content: |
        ### {index-content.formats_groups.title_3}
        * **{index-content.formats_groups.format_web}:** HTML, MHTML
        * **{index-content.formats_groups.format_archives}:** ZIP, TAR, 7Z
        * **{index-content.formats_groups.format_certificates}:** PFX

############################# Features ############################
features:
  enable: true
  title: "{index-content.features.title}"
  description: "{index-content.features.description}"

  items:
    # feature loop
    - icon: "merge"
      title: "{index-content.features.feature_1.title}"
      content: "{index-content.features.feature_1.content}"

    # feature loop
    - icon: "split"
      title: "{index-content.features.feature_2.title}"
      content: "{index-content.features.feature_2.content}"

    # feature loop
    - icon: "move"
      title: "{index-content.features.feature_3.title}"
      content: "{index-content.features.feature_3.content}"

    # feature loop
    - icon: "remove"
      title: "{index-content.features.feature_4.title}"
      content: "{index-content.features.feature_4.content}"

    # feature loop
    - icon: "rotate"
      title: "{index-content.features.feature_5.title}"
      content: "{index-content.features.feature_5.content}"

    # feature loop
    - icon: "swap"
      title: "{index-content.features.feature_6.title}"
      content: "{index-content.features.feature_6.content}"

    # feature loop
    - icon: "extract"
      title: "{index-content.features.feature_7.title}"
      content: "{index-content.features.feature_7.content}"

    # feature loop
    - icon: "orientation"
      title: "{index-content.features.feature_8.title}"
      content: "{index-content.features.feature_8.content}"

    # feature loop
    - icon: "preview"
      title: "{index-content.features.feature_9.title}"
      content: "{index-content.features.feature_9.content}"

############################# Code samples ############################
code_samples:
  enable: true
  title: "{index-content-net.code_samples.title}"
  description: "{index-content-net.code_samples.description}"
  items:
    # code sample loop
    - title: "{index-content-net.code_samples.sample_1.title}"
      content: |
        {index-content-net.code_samples.sample_1.content_1} {index-content-net.code_samples.sample_1.content_2}
        {{< landing/code title="{index-content-net.code_samples.sample_1.code_title}">}}
        ```csharp {style=abap}
        // {index-content-net.code_samples.sample_1.comment_1}
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // {index-content-net.code_samples.sample_1.comment_2}
            QrCodeSignOptions options = new QrCodeSignOptions("The document is approved by John Smith")
            {
                // {index-content-net.code_samples.sample_1.comment_3}
                EncodeType = QrCodeTypes.QR,
                Left = 100,
                Top = 100
            };
            // {index-content-net.code_samples.sample_1.comment_4}
            signature.Sign("file_with_QR.pdf", options);
        }
        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "{index-content-net.code_samples.sample_2.title}"
      content: |
        {index-content-net.code_samples.sample_2.content_1} {index-content-net.code_samples.sample_2.content_2}
        {{< landing/code title="{index-content-net.code_samples.sample_2.code_title}">}}
        ```csharp {style=abap}   
        // {index-content-net.code_samples.sample_2.comment_1}
        using (Signature signature = new Signature("file_to_sign.pdf"))
        {
            // {index-content-net.code_samples.sample_2.comment_2}
            DigitalSignOptions options = new DigitalSignOptions("certificate.pfx")
            {
                // {index-content-net.code_samples.sample_2.comment_3}
                Password = "1234567890"
            };
            // {index-content-net.code_samples.sample_2.comment_4}
            signature.Sign("digitally_signed.pdf", options);
        }


        ```
        {{< /landing/code >}}

############################# Reviews ############################
# reviews:
# enable: true
# title: "{reviews.title}"
# description: "{reviews.description}"

# items:
#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_1.content}"
#     author: "{reviews.review_1.author}"
#     company: "{reviews.review_1.company}"

#   # review loop
#   - title: "GroupDocs.Viewer"
#     content: "{reviews.review_2.content}"
#     author: "{reviews.review_2.author}"
#     company: "{reviews.review_2.company}"
---
