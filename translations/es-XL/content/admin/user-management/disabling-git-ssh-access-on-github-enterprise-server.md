---
title: Inhabilitar el acceso SSH de Git en el servidor de GitHub Enterprise
redirect_from:
  - /enterprise/admin/hidden/disabling-ssh-access-for-a-user-account/
  - /enterprise/admin/articles/disabling-ssh-access-for-a-user-account/
  - /enterprise/admin/hidden/disabling-ssh-access-for-your-appliance/
  - /enterprise/admin/articles/disabling-ssh-access-for-your-appliance/
  - /enterprise/admin/hidden/disabling-ssh-access-for-an-organization/
  - /enterprise/admin/articles/disabling-ssh-access-for-an-organization/
  - /enterprise/admin/hidden/disabling-ssh-access-to-a-repository/
  - /enterprise/admin/articles/disabling-ssh-access-to-a-repository/
  - /enterprise/admin/guides/installation/disabling-git-ssh-access-on-github-enterprise/
  - /enterprise/admin/installation/disabling-git-ssh-access-on-github-enterprise-server
  - /enterprise/admin/user-management/disabling-git-ssh-access-on-github-enterprise-server
intro: 'Puedes evitar que las personas usen Git por SSH para determinados repositorios o para todos ellos en {{ site.data.variables.product.product_location_enterprise }}.'
versions:
  enterprise-server: '*'
---

### Inhabilitar el acceso SSH de Git para un repositorio específico

{{ site.data.reusables.enterprise_site_admin_settings.override-policy }}

{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.repository-search }}
{{ site.data.reusables.enterprise_site_admin_settings.click-repo }}
{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.admin-top-tab }}
{{ site.data.reusables.enterprise_site_admin_settings.admin-tab }}
1. En "Acceso SSH de Git", usa el menú desplegable y haz clic en **Disabled** (Inhabilitado). ![Menú desplegable del acceso SSH de Git con la opción de inhabilitación seleccionada](/assets/images/enterprise/site-admin-settings/git-ssh-access-repository-setting.png)

### Inhabilitar el acceso SSH de Git para todos los repositorios que le pertenecen a un usuario o a una organización

{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.search-user-or-org }}
{{ site.data.reusables.enterprise_site_admin_settings.click-user-or-org }}
{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.admin-top-tab }}
{{ site.data.reusables.enterprise_site_admin_settings.admin-tab }}
7. En "Acceso SSH de Git", usa el menú desplegable y haz clic en **Disabled** (Inhabilitado). Luego selecciona **Enforce on all repositories** (Aplicar en todos los repositorios). ![Menú desplegable del acceso SSH de Git con la opción de inhabilitación seleccionada](/assets/images/enterprise/site-admin-settings/git-ssh-access-organization-setting.png)

### Inhabilitar el acceso SSH de Git para todos los repositorios de un aparato

{{ site.data.reusables.enterprise_site_admin_settings.access-settings }}
{{ site.data.reusables.enterprise_site_admin_settings.business }}
{% if currentVersion ver_gt "enterprise-server@2.21" %}
{{ site.data.reusables.enterprise-accounts.policies-tab }}
{% else %}
{{ site.data.reusables.enterprise-accounts.settings-tab }}
{% endif %}
{{ site.data.reusables.enterprise-accounts.options-tab }}
7. En "Acceso SSH de Git", usa el menú desplegable y haz clic en **Disabled** (Inhabilitado). Luego selecciona **Enforce on all repositories** (Aplicar en todos los repositorios). ![Menú desplegable del acceso SSH de Git con la opción de inhabilitación seleccionada](/assets/images/enterprise/site-admin-settings/git-ssh-access-appliance-setting.png)