---
title: Managing repository access for your organization's codespaces
shortTitle: Repository access
intro: '{% data variables.product.prodname_github_codespaces %} がアクセスできる Organization 内のリポジトリを管理できます。'
product: '{% data reusables.gated-features.codespaces %}'
permissions: 'To manage access and security for {% data variables.product.prodname_github_codespaces %} for an organization, you must be an organization owner.'
versions:
  fpt: '*'
  ghec: '*'
type: how_to
topics:
  - Codespaces
  - Security
  - Administrator
redirect_from:
  - /codespaces/managing-codespaces-for-your-organization/managing-access-and-security-for-your-organizations-codespaces
  - /github/developing-online-with-codespaces/managing-access-and-security-for-codespaces
  - /codespaces/working-with-your-codespace/managing-access-and-security-for-codespaces
---

{% warning %}

**Deprecation note**: The access and security setting described below is now deprecated and is documented here for reference only. To enable expanded access to other repositories, add the requested permissions to your dev container definition. For more information, see "[Managing access to other repositories within your codespace](/codespaces/managing-your-codespaces/managing-repository-access-for-your-codespaces)."

{% endwarning %}

デフォルト設定では、Codespace は作成されたリポジトリにのみアクセスできます。 When you enable access and security for a repository owned by your organization, any codespaces that are created for that repository will also have read permissions to all other repositories the organization owns and the codespace creator has permissions to access. If you want to restrict the repositories a codespace can access, you can limit it to either the repository where the codespace was created, or to specific repositories. 信頼するリポジトリに対してのみ、アクセスとセキュリティを有効にしてください。

To manage which users in your organization can use {% data variables.product.prodname_github_codespaces %}, see "[Enabling GitHub Codespaces for your organization](/codespaces/managing-codespaces-for-your-organization/enabling-github-codespaces-for-your-organization#enable-codespaces-for-users-in-your-organization)."

{% data reusables.profile.access_org %}
{% data reusables.profile.org_settings %}
{% data reusables.organizations.click-codespaces %}
1. [Access and security] で、あなたの Organization の設定を選択します。 ![信頼するリポジトリを管理するラジオボタン](/assets/images/help/settings/codespaces-org-access-and-security-radio-buttons.png)
1. [Selected repositories] を選択した場合、ドロップダウンメニューを選択してから、あなたの Organization が所有するその他のリポジトリにアクセスを許可する、リポジトリのコードスペースをクリックします。 その他のリポジトリにコードスペースによるアクセスを許可したい、すべてのリポジトリについて同じ手順を繰り返します。 ![[Selected repositories]ドロップダウンメニュー](/assets/images/help/settings/codespaces-access-and-security-repository-drop-down.png)

## 参考リンク

- "[Managing repository access for your codespaces](/codespaces/managing-your-codespaces/managing-repository-access-for-your-codespaces)"
