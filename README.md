# OpenSearch-Dashboard Community Translations

pt-BR translations for OpenSearch-Dashboard.

Tested on OpenSearch-Dashboard version 1.2.0

## How to use it

### Installation

```bash
git clone --depth 1 --branch 1.2.0 https://github.com/opensearch-project/OpenSearch-Dashboards
cd OpenSearch-Dashboards/plugins/ 

git clone https://github.com/schleuss/opensearch-dashboard-i18n-ptbr
cd ../

# Fix error - directory not exist 
mkdir -p src/legacy/core_plugins/management/translations/

yarn osd bootstrap

node scripts/i18n_integrate --source plugins/opensearch-dashboards-translations/translations/pt-BR.json

```
### Configuration

Change / Add the parameter ``i18n.locale`` in the config file of OpenSearch-Dashboard (config/opensearch_dashboards.yml). The value of this parameter is the locale id that you can found in the list of available languages below.

For example, if you want use the french translation, add the following line in your OpenSearch-Dashboard config file:

```yaml
i18n.locale: "pt-BR"
```
