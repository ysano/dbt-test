# dbt test repo

## インストール作業

### Install dbt

- python -m venv .venv
- source .venv/bin/activate
- pip install dbt-bigquery

### OAuth

- gcloud auth application-default loginによって認証する
- https://docs.getdbt.com/docs/core/connect-data-platform/bigquery-setup#local-oauth-gcloud-setup

### dbt project

- dbt init
- $HOME/.dbt/profiles.yml に接続情報を保持


### move project files to repo root

- mv dbt_test/* .
- rmdir dbt_test

## Using the starter project

Try running the following commands:
- dbt run
- dbt test

### Documentation

- dbt docs serve

### persist_docs

- dbt runで生成されたドキュメントを永続化するための設定
- https://docs.getdbt.com/reference/resource-configs/persist_docs

### dbt-osmosis

- pip install dbt-osmosis
- dbt-osmosis yaml refactor

### dbt-coverage

- pip install dbt-coverage
- dbt docs generate

### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
