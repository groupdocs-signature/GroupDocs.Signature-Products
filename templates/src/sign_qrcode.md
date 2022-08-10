<% configRef "..\\configs\\config_sign_qrcode.yml" %>
<% set "SIGNATURETYPE" (upper (get "signaturetype")) %>
<% set "BARCODETYPE" (upper (get "barcodetype")) %>
<% set "FILEFORMAT" (upper (get "fileformat")) %>
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
<% set "OtherFormats" (dict "otherformats.{from}") %>
<% include "..\\landings\\_sign_qrcode.md" %>