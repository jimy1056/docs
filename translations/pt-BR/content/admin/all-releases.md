---
title: Versões do GitHub Enterprise Server
intro: '{% data variables.product.company_short %} lança novas versões de {% data variables.product.product_name %} regularmente. Você pode rever versões compatíveis, ver datas de obsolescência e consultar a documentação para a versão que você instalou.'
allowTitleToDifferFromFilename: true
versions:
  ghes: '*'
topics:
  - Enterprise
  - Upgrades
shortTitle: Versões
---

## Sobre as versões de {% data variables.product.product_name %}

{% data reusables.enterprise.constantly-improving %} {% data variables.product.company_short %} é compatível com as quatro versões de recurso mais recentes. Para obter mais informações, consulte[Sobre atualizações para novas versões de](/admin/overview/about-upgrades-to-new-releases)."

Você pode ver o que há de novo para cada versão nas [observações da versão](/admin/release-notes) e você pode visualizar a documentação de administrador e usuário para todas as versões aqui em {% data variables.product.prodname_docs %}. Ao ler a documentação, certifique-se de selecionar a versão que reflete o seu produto. Para obter mais informações, consulte "[Sobre as versões do {% data variables.product.prodname_docs %}](/get-started/learning-about-github/about-versions-of-github-docs)."

## Versões atualmente compatíveis

{% data variables.product.company_short %} é compatível com as seguintes versões de {% data variables.product.product_name %}. Para obter mais informações sobre a última versão, consulte o [side de {% data variables.product.prodname_enterprise %}](https://github.com/enterprise).

| Versão | Versão | Deprecation | Notas de lançamento | Documentação |
|:------ |:------ |:----------- |:------------------- |:------------ |
|        |        |             |                     |              |
{%- for version in enterpriseServerReleases.supported %}
| {{version}} | {{enterpriseServerReleases.dates[version].releaseDate}} | {{enterpriseServerReleases.dates[version].deprecationDate}} | [{{version}} observações da versão](/enterprise-server@{{version}}/admin/release-notes) | [{{version}} documentation](/enterprise-server@{{version}}) |
{%- endfor %}

## Versões obsoletas

{% data variables.product.company_short %} fornece documentação para versões obsoletas, mas não mantém ou atualiza a documentação.

| Versão | Versão | Deprecation | Notas de lançamento | Documentação |
|:------ |:------ |:----------- |:------------------- |:------------ |
|        |        |             |                     |              |
{%- for version in enterpriseServerReleases.deprecatedReleasesWithNewFormat %}
| {{version}} | {{enterpriseServerReleases.dates[version].releaseDate}} | {{enterpriseServerReleases.dates[version].deprecationDate}} | [{{version}} observações da versão](/enterprise-server@{{version}}/admin/release-notes) | [{{version}} documentation](/enterprise-server@{{version}}) |
{%- endfor %}
{%- for version in enterpriseServerReleases.deprecatedReleasesWithLegacyFormat %}
| {{version}} | {{enterpriseServerReleases.dates[version].releaseDate}} | {{enterpriseServerReleases.dates[version].deprecationDate}} | [{{version}} observações sobre a versão](https://enterprise.github.com/releases/series/{{version}}) | [{{version}} documentação](/enterprise/{{version}}) |
{%- endfor %}

### Documentação de desenvolvedor descontinuada

{% data variables.product.company_short %} hosted developer documentation for {% data variables.product.product_name %} on a separate site until the 2.17 release. {% data variables.product.company_short %} continues to provide developer documentation for version 2.16 and earlier, but does not maintain or update the documentation.

| Versão | Versão | Deprecation | Developer documentation |
|:------ |:------ |:----------- |:----------------------- |
|        |        |             |                         |
{%- for version in enterpriseServerReleases.deprecatedReleasesOnDeveloperSite %}
| {{version}} | {{enterpriseServerReleases.dates[version].releaseDate}} | {{enterpriseServerReleases.dates[version].deprecationDate}} | [{{version}} developer documentation](https://developer.github.com/enterprise/{{version}}) |
{%- endfor %}
