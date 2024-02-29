<% configRef "..\\configs\\index\\index_nodejs.yml" %>
<% set "ProductName" (dict "products.{product}.name") %>
<% set "ProdShortName" (dict "products.productShortName") %>
<% set "ProductFullName" (dict "products.{product}.fullName") %>
<% set "ProductCode" (dict "products.{product}.code") %>
<% set "ProductUrl" (dict "products.{product}.url") %>
<% set "ProgLang" (dict "products.{product}.progLang") %>
<% set "SrcFileExt" (dict "products.{product}.srcFileExt") %>
<% set "DevEnv" (dict "products.{product}.devEnv") %>
<% set "Runtime" (dict "products.{product}.runtime") %>
<% set "RepoName" (dict "products.{product}.repoName") %>
<% set "RepoUrl" (dict "products.{product}.repoUrl") %>
<% set "SupportedFormatsUrl" (dict "products.{product}.supportedFormatsUrl") %>
<% set "Sample1Url" (dict "products.{product}.sample1Url") %>
<% set "Sample2Url" (dict "products.{product}.sample2Url") %>
<% include "..\\landings\\index\\_index_nodejs.md" %>