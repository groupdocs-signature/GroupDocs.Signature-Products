<% configRef "..\\configs\\sign\\config_qrcode.yml" %>
<% set "Operation" (capitalize (get "operation")) %>
<% set "Signaturetype" (capitalize (get "signaturetype")) %>
<% set "Codetype" (capitalize (get "qrcodetype")) %>
<% set "Fileformat" (capitalize (get "fileformat")) %>
<% set "CodeDetails" (dict "bar_qr_codes.{qrcodetype}.details") %>
<% set "CodeCharacterSet" (dict "bar_qr_codes.{qrcodetype}.characterset") %>
<% set "CodeTextCapacity" (dict "bar_qr_codes.{qrcodetype}.codetextcapacity") %>
<% set "CodeImage" (dict "bar_qr_code_images.{qrcodetype}") %>
<% set "ProductName" (dict "products.{product}.name") %>
<% set "ProductFullName" (dict "products.{product}.fullName") %>
<% set "ProductCode" (dict "products.{product}.code") %>
<% set "ProductUrl" (dict "products.{product}.url") %>
<% set "ProgLang" (dict "products.{product}.progLang") %>
<% set "SrcFileExt" (dict "products.{product}.srcFileExt") %>
<% set "DevEnv" (dict "products.{product}.devEnv") %>
<% set "Runtime" (dict "products.{product}.runtime") %>
<% set "RepoName" (dict "products.{product}.repoName") %>
<% set "RepoUrl" (dict "products.{product}.repoUrl") %>
<% set "OtherFormats" (dict "otherformats_sign.qrcode") %>
<% include "..\\landings\\sign\\_qrcode.md" %>