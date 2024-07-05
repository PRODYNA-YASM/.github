# YASM Deployment Overview

Component Status overview. Last update 2024-07-05T11:59:38Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :red_square: [9](https://github.com/prodyna-yasm/yasm-backend/compare/1.34.0..HEAD) | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.34.0 |  :red_square: 5bcdde7 |  :green_square: 1.34.0 |  :red_square: 1.32.0 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :red_square: [8](https://github.com/prodyna-yasm/yasm-frontend/compare/1.34.0..HEAD) | :yellow_square: [7](https://github.com/prodyna-yasm/yasm-frontend/pulls) | 1.34.0 |  :red_square: 2fcf5db |  :green_square: 1.34.0 |  :red_square: 1.32.0 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :green_square: 0 | :green_square: 0 | 1.37.0 |  :green_square: 1.37.0 |  :green_square: 1.37.0 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :green_square: 0 | :green_square: 0 | 1.37.0 |  :red_square: e5e8641 |  :red_square: 1.36.0 |  :red_square: 1.32.0 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :green_square: 0 | :green_square: 0 | 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 | 
| [yasm-github](https://github.com/prodyna-yasm/yasm-github) | :red_square: [6](https://github.com/prodyna-yasm/yasm-github/compare/1.5.2..HEAD) | :green_square: 0 | 1.5.2 |  :red_square: b43ab5f |  :green_square: 1.5.2 |  :green_square: 1.5.2 | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :red_square: [6](https://github.com/prodyna-yasm/yasm-geocoding/compare/1.11.0..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-geocoding/pulls) | 1.11.0 |  :red_square: 5ac2457 |  :green_square: 1.11.0 |  :green_square: 1.11.0 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :red_square: [2](https://github.com/prodyna-yasm/yasm-data/compare/1.26.0..HEAD) | :green_square: 0 | 1.26.0 |  :red_square: a59d951 |  :green_square: 1.26.0 |  :green_square: 1.26.0 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.8.0-1 |  :green_square: 8.8.0-1 |  :green_square: 8.8.0-1 |  :red_square: 8.7.0-2 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-infrastructure-staged/pulls) | 1.37.0 |  :green_square: 1.37.0 |  :green_square: 1.37.0 |  :green_square: 1.37.0 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :green_square: 0 | :yellow_square: [4](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.37.0 | 
| [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) | :green_square: 0 | :yellow_square: [3](https://github.com/prodyna-yasm/yasm-nginx/pulls) | 1.25.4-2 | 
| [yasm-test](https://github.com/prodyna-yasm/yasm-test) | :green_square: 0 | :yellow_square: [6](https://github.com/prodyna-yasm/yasm-test/pulls) | 1.30.1 | 
| [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/sales-copilot/pulls) | 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.34.0




### [Commits on main since 1.34.0](https://github.com/prodyna-yasm/yasm-backend/compare/1.34.0..HEAD) (9)

- [feat: add experience skill group to project details (#675)](https://github.com/prodyna-yasm/yasm-backend/commit/5bcdde71458ea87a8eacdae954a9df1329ffd2f8) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-07-05 07:25:49 +0000 UTC

- [build(deps): update quarkus 3.12.1 (#674)](https://github.com/prodyna-yasm/yasm-backend/commit/b5bcded6cef3f3ed753c5d1a855992d9e24afa48) by [coding4kay](https://github.com/coding4kay) on 2024-07-04 11:36:51 +0000 UTC

- [feat: search for offices in global search and add office score (#666)](https://github.com/prodyna-yasm/yasm-backend/commit/2bc5df69a407ddc66db68f1697afe32a0b248b5c) by [saemik94](https://github.com/saemik94) on 2024-07-02 07:44:07 +0000 UTC

- [fix: only return offices with at least one assigned person in the global search (#665)](https://github.com/prodyna-yasm/yasm-backend/commit/51e83d7dcf5a0aff3adc904afeef6d53506d660b) by [saemik94](https://github.com/saemik94) on 2024-07-02 06:35:10 +0000 UTC

- [fix: delete org skill audit (#669)](https://github.com/prodyna-yasm/yasm-backend/commit/e122b45a173838b19e4b73a2d8a7006c06178fed) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-28 14:08:50 +0000 UTC

- [build(deps): pipeline update build-push-action (#671)](https://github.com/prodyna-yasm/yasm-backend/commit/4cd53fb518dae4ee2c97e05ec4698c91d1100dd9) by [coding4kay](https://github.com/coding4kay) on 2024-06-28 10:53:52 +0000 UTC

- [build(deps): update quarkus (#670)](https://github.com/prodyna-yasm/yasm-backend/commit/ea01cea261c24e032f6587eb1a8a0ee7671faff3) by [coding4kay](https://github.com/coding4kay) on 2024-06-28 10:09:22 +0000 UTC

- [feat: show the number of direct and related search results (#664)](https://github.com/prodyna-yasm/yasm-backend/commit/deee49c6746fd0b03f8b5aa411ed46f6d195ba2d) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-27 12:57:52 +0000 UTC

- [feat: 15 update audit on relation change (#667)](https://github.com/prodyna-yasm/yasm-backend/commit/eb4fbe7212d9a3d4d49bc30880fc490218c6e4e4) by [coding4kay](https://github.com/coding4kay) on 2024-06-26 17:09:12 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-backend/pulls) (2)

- [refactor: change to cypher template for relation updates](https://github.com/PRODYNA-YASM/yasm-backend/pull/672)

- [Bump eclipse-temurin from 21.0.2_13-jre-ubi9-minimal to 22.0.1_8-jre-ubi9-minimal](https://github.com/PRODYNA-YASM/yasm-backend/pull/588)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  5bcdde7 |  1.34.0 |  1.32.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :red_square: | 


### Last releases

- [Added audit log, added person skill statistic endpoint, add role-check-security in BE to edit entities](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.34.0) on 2024-06-24 11:04:59 +0000 UTC

- [Improve entitiy specific search, increase payload size to 3MB and extend search metric](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.32.0) on 2024-06-18 12:16:59 +0000 UTC

- [Bookmarks and active user filter](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.29.0) on 2024-06-07 09:33:51 +0000 UTC






## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.34.0




### [Commits on main since 1.34.0](https://github.com/prodyna-yasm/yasm-frontend/compare/1.34.0..HEAD) (8)

- [fix: only display new versions on the landing page (#772)](https://github.com/prodyna-yasm/yasm-frontend/commit/2fcf5db7c917dbcc676326257d893ad2bd2a6082) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-07-05 11:55:22 +0000 UTC

- [feat: update participation detail pages (#771)](https://github.com/prodyna-yasm/yasm-frontend/commit/49fd691cebea15a069a7e59bec791b56ea53fde1) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-07-05 09:56:16 +0000 UTC

- [fix: skill sort employee project (#769)](https://github.com/prodyna-yasm/yasm-frontend/commit/69d4fce192a307d704b19c12f53fc813769e23cd) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-07-04 13:12:19 +0000 UTC

- [fix: change search organization logo placeholder label (#768)](https://github.com/prodyna-yasm/yasm-frontend/commit/0b3adde5dfda7ba8b5d716c7e55e104f2763d364) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-07-04 12:33:37 +0000 UTC

- [feat: set assignee when creating yasm-ticket type Organization (#767)](https://github.com/prodyna-yasm/yasm-frontend/commit/fd7a250f1bb5609a7295647f0cebdc07339e6246) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-07-04 12:33:16 +0000 UTC

- [chore: update api version (#766)](https://github.com/prodyna-yasm/yasm-frontend/commit/33ce466eeb6f6566b55264f14fd447e563043673) by [saemik94](https://github.com/saemik94) on 2024-07-02 07:33:27 +0000 UTC

- [feat: project participation (#765)](https://github.com/prodyna-yasm/yasm-frontend/commit/39ee8689564f5db9a7fbaa3e83b1c4536ccb00be) by [readmey](https://github.com/readmey) on 2024-07-02 07:21:42 +0000 UTC

- [feat: search and filter for offices using the global search (#764)](https://github.com/prodyna-yasm/yasm-frontend/commit/d1e511f2efe0a42b0008519b334523971a3460df) by [saemik94](https://github.com/saemik94) on 2024-07-02 07:00:14 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-frontend/pulls) (7)

- [feat: show the number of direct and related search results](https://github.com/PRODYNA-YASM/yasm-frontend/pull/770)

- [chore: bump @types/node from 20.14.0 to 20.14.9](https://github.com/PRODYNA-YASM/yasm-frontend/pull/763)

- [chore: bump @opentelemetry/instrumentation from 0.43.0 to 0.52.1](https://github.com/PRODYNA-YASM/yasm-frontend/pull/754)

- [chore: bump ws from 7.5.9 to 7.5.10](https://github.com/PRODYNA-YASM/yasm-frontend/pull/745)

- [chore: bump memfs from 3.5.3 to 4.9.3](https://github.com/PRODYNA-YASM/yasm-frontend/pull/738)

- [Bump rimraf from 4.4.1 to 5.0.7](https://github.com/PRODYNA-YASM/yasm-frontend/pull/682)

- [Bump html-loader from 1.3.2 to 5.0.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/619)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  2fcf5db |  1.34.0 |  1.32.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :red_square: | 


### Last releases

- [Improvements in yasm-test pipeline, refactor Projects-Detail-View, improved Employee-Detail-View.](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.34.0) on 2024-06-24 14:51:13 +0000 UTC

- [Sort Skills alphabetically in PdfExport, fixed skill administration bugs,  Update Employee and Organization card design, fixed user cannot delete project](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.32.0) on 2024-06-18 12:38:19 +0000 UTC

- [Synchronize Select of Skills&Methodologies, Update Project after edit (without refresh) and fixed deleting organization](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.29.1) on 2024-06-07 14:53:18 +0000 UTC






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.37.0







### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  1.37.0 |  1.37.0 | 
| Release |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: | 


### Last releases

- [Using API 1.37.0](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.37.0) on 2024-07-05 05:36:42 +0000 UTC

- [Using API 1.36.0, some components updated](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.36.0) on 2024-07-03 07:32:33 +0000 UTC

- [Using API 1.33, some components updated](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.33.0) on 2024-06-21 06:37:58 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-integration/actions?query=is%3Awaiting) (5)

- [Merge pull request #467 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9807809312) created on 2024-07-05 11:47:13 +0000 UTC

- [Merge pull request #465 from PRODYNA-YASM/464-api-136](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9774318138) created on 2024-07-03 08:18:05 +0000 UTC

- [Merge pull request #455 from PRODYNA-YASM/dependabot/docker/alpine-3.…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9611541286) created on 2024-06-21 09:35:29 +0000 UTC

- [Merge pull request #445 from PRODYNA-YASM/feature/technology-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9499658142) created on 2024-06-13 12:30:50 +0000 UTC

- [Merge pull request #437 from PRODYNA-YASM/feature/update-components](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9413568240) created on 2024-06-07 07:51:14 +0000 UTC




## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.37.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  e5e8641 |  1.36.0 |  1.32.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :red_square: |  :red_square: | 


### Last releases

- [Using API 1.37.0, Update to otelhttp](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.37.0) on 2024-07-04 22:30:37 +0000 UTC

- [Using API 1.36, some components updated](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.36.0) on 2024-07-03 08:04:35 +0000 UTC

- [Using API 1.33](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.33.0) on 2024-06-21 09:26:13 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (3)

- [Merge pull request #359 from PRODYNA-YASM/358-api-136](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9774338264) created on 2024-07-03 08:19:27 +0000 UTC

- [Merge pull request #342 from PRODYNA-YASM/341-use-api-133](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9611533495) created on 2024-06-21 09:34:55 +0000 UTC

- [Merge pull request #336 from PRODYNA-YASM/feature/fix-codeql](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9499139781) created on 2024-06-13 11:55:47 +0000 UTC




## [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) 1.16.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.16.0 |  1.16.0 |  1.16.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Technology update (chi)](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.16.0) on 2024-07-01 14:01:36 +0000 UTC

- [Technology update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.15.0) on 2024-06-21 09:32:17 +0000 UTC

- [Component update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.14.0) on 2024-06-17 15:39:02 +0000 UTC






## [yasm-github](https://github.com/prodyna-yasm/yasm-github) 1.5.2




### [Commits on main since 1.5.2](https://github.com/prodyna-yasm/yasm-github/compare/1.5.2..HEAD) (6)

- [Merge pull request #106 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlpmetric/otlpmetricgrpc-1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/b43ab5f1bd326f83c21eceab6b8135e2e6629d00) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 23:28:31 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlpmetric/otlpmetricgrpc](https://github.com/prodyna-yasm/yasm-github/commit/963df535379978b8092c3b5a98796c6fc24b411e) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 23:25:29 +0000 UTC

- [Merge pull request #107 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracegrpc-1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/2f779b04f1d199b91b63a1bc807499dcfffececf) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 23:24:19 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracegrpc](https://github.com/prodyna-yasm/yasm-github/commit/d520a75d2e44b42e9cf5cbe4944ca89b92624bc9) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 23:21:36 +0000 UTC

- [Merge pull request #108 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/contrib/instrumentation/net/http/otelhttp-0.53.0](https://github.com/prodyna-yasm/yasm-github/commit/0d6958fdfb8fd952bedc15cbc886f4be2ee1e5de) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 23:20:22 +0000 UTC

- [Bump go.opentelemetry.io/contrib/instrumentation/net/http/otelhttp](https://github.com/prodyna-yasm/yasm-github/commit/1fc07f8ae03afc9d8de5e0dcb5390f91a864e142) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 23:14:42 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  b43ab5f |  1.5.2 |  1.5.2 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [OpenTelemetry update](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.5.2) on 2024-07-03 07:03:27 +0000 UTC

- [Technology update, setting network peer for OpenTelemetry](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.5.1) on 2024-06-21 09:32:02 +0000 UTC

- [CodeQL activated](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.5.0) on 2024-06-12 07:23:18 +0000 UTC






## [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) 1.11.0




### [Commits on main since 1.11.0](https://github.com/prodyna-yasm/yasm-geocoding/compare/1.11.0..HEAD) (6)

- [Merge pull request #133 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlpmetric/otlpmetricgrpc-1.28.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/5ac24575139e65a219eebca446fc175dda36c450) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 16:28:06 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlpmetric/otlpmetricgrpc](https://github.com/prodyna-yasm/yasm-geocoding/commit/cb022de549c062d6e86718dde1f36b1e3b898a08) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 16:26:49 +0000 UTC

- [Merge pull request #129 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/sdk/metric-1.28.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/7533bc92a45fae417c298e8f9698aa20c4571b63) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 16:26:45 +0000 UTC

- [Bump go.opentelemetry.io/otel/sdk/metric from 1.27.0 to 1.28.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/b68f3ef81d0224ba20d9627aa6a5b444d12ff802) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 16:22:46 +0000 UTC

- [Merge pull request #131 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracegrpc-1.28.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/8da3b7104baf9bd4abc9822c232852960975f629) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 16:21:51 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracegrpc](https://github.com/prodyna-yasm/yasm-geocoding/commit/edb5f7bf3acd113755d85b44dcc1e7b695a42249) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 16:19:12 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-geocoding/pulls) (1)

- [Bump golang from 1.22.4 to 1.22.5](https://github.com/PRODYNA-YASM/yasm-geocoding/pull/135)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  5ac2457 |  1.11.0 |  1.11.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Component updates](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.11.0) on 2024-07-02 17:50:16 +0000 UTC

- [Component update](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.10.0) on 2024-06-20 09:47:44 +0000 UTC

- [Component update](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.13) on 2024-06-05 17:15:09 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-geocoding/actions?query=is%3Awaiting) (1)

- [Merge pull request #123 from PRODYNA-YASM/feature/update-components](https://github.com/PRODYNA-YASM/yasm-geocoding/actions/runs/9611605327) created on 2024-06-21 09:40:41 +0000 UTC




## [yasm-data](https://github.com/prodyna-yasm/yasm-data) 1.26.0




### [Commits on main since 1.26.0](https://github.com/prodyna-yasm/yasm-data/compare/1.26.0..HEAD) (2)

- [Merge pull request #117 from PRODYNA-YASM/dependabot/github_actions/docker/build-push-action-6](https://github.com/prodyna-yasm/yasm-data/commit/a59d9510b5e4aaba3ad8411f48bf9bdf310b3b5f) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 13:07:30 +0000 UTC

- [Bump docker/build-push-action from 5 to 6](https://github.com/prodyna-yasm/yasm-data/commit/9329ce3a513758a35c13ef697a89d5b0169546da) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-18 04:57:08 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  a59d951 |  1.26.0 |  1.26.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Add some roles](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.26.0) on 2024-04-29 06:13:23 +0000 UTC

- [New roles](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.2) on 2024-04-29 06:13:23 +0000 UTC

- [Main branch](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.1) on 2024-04-19 13:36:35 +0000 UTC






## [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) 8.8.0-1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  8.8.0-1 |  8.8.0-1 |  8.7.0-2 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [Gotenberg 8.8.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.8.0-1) on 2024-07-04 05:46:24 +0000 UTC

- [Build push action v6](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.7.0-2) on 2024-06-18 00:21:00 +0000 UTC

- [Gotenberg 8.7.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.7.0-1) on 2024-06-14 03:54:46 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-gotenberg/actions?query=is%3Awaiting) (2)

- [Merge pull request #47 from PRODYNA-YASM/dependabot/docker/gotenberg/…](https://github.com/PRODYNA-YASM/yasm-gotenberg/actions/runs/9807836189) created on 2024-07-05 11:49:53 +0000 UTC

- [Merge pull request #45 from PRODYNA-YASM/dependabot/docker/gotenberg/…](https://github.com/PRODYNA-YASM/yasm-gotenberg/actions/runs/9512157562) created on 2024-06-14 07:12:42 +0000 UTC




## [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) 1.37.0






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-infrastructure-staged/pulls) (2)

- [Update GitHub 6.2.2 and azurerm 3.111.0](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/pull/565)

- [Bump github from 6.2.1 to 6.2.2 in /terraform/azure](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/pull/538)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.37.0 |  1.37.0 |  1.37.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Rotate passwords for jobs, update components](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.37.0) on 2024-07-05 10:58:12 +0000 UTC

- [Updated providers](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.30.0) on 2024-06-10 23:20:11 +0000 UTC

- [DAPR 1.13.4](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.27.1) on 2024-06-02 16:10:22 +0000 UTC






## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.37.0






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-api/pulls) (4)

- [chore: bump org.openapitools:openapi-generator-maven-plugin from 7.6.0 to 7.7.0](https://github.com/PRODYNA-YASM/yasm-api/pull/212)

- [feat: #137 created skillsProfile endpoints and SkillsProfile entity](https://github.com/PRODYNA-YASM/yasm-api/pull/208)

- [chore: bump io.smallrye.reactive:mutiny from 2.6.0 to 2.6.1](https://github.com/PRODYNA-YASM/yasm-api/pull/206)

- [feat: 324-project-images](https://github.com/PRODYNA-YASM/yasm-api/pull/194)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [Add ExperienceSkill in Projects and replace Experiences with SkillGroups in ProjectParticipation](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.37.0) on 2024-07-04 11:46:47 +0000 UTC

- [Add dedicated score types](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.36.0) on 2024-07-02 07:10:02 +0000 UTC

- [Audit to Availability](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.35.0) on 2024-06-26 16:32:56 +0000 UTC






## [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) 1.25.4-2






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-nginx/pulls) (3)

- [Bump docker/build-push-action from 5 to 6](https://github.com/PRODYNA-YASM/yasm-nginx/pull/8)

- [Bump ubuntu from 22.04 to 24.04](https://github.com/PRODYNA-YASM/yasm-nginx/pull/7)

- [Bump nginx from 1.25.4 to 1.26.0](https://github.com/PRODYNA-YASM/yasm-nginx/pull/6)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [Brotli + OTEL](https://github.com/PRODYNA-YASM/yasm-nginx/releases/tag/1.25.4-2) on 2024-02-28 17:47:02 +0000 UTC

- [Brotli support](https://github.com/PRODYNA-YASM/yasm-nginx/releases/tag/1.25.4-1) on 2024-02-27 22:17:41 +0000 UTC






## [yasm-test](https://github.com/prodyna-yasm/yasm-test) 1.30.1






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-test/pulls) (6)

- [chore(deps): Bump jose from 5.4.0 to 5.6.3](https://github.com/PRODYNA-YASM/yasm-test/pull/115)

- [chore(deps): Bump cypress/included from 13.11.0 to 13.13.0](https://github.com/PRODYNA-YASM/yasm-test/pull/114)

- [chore(deps): Bump @azure/msal-node from 2.7.0 to 2.10.0](https://github.com/PRODYNA-YASM/yasm-test/pull/113)

- [chore(deps-dev): Bump cypress from 13.11.0 to 13.13.0](https://github.com/PRODYNA-YASM/yasm-test/pull/112)

- [chore(deps-dev): Bump typescript from 5.4.5 to 5.5.3](https://github.com/PRODYNA-YASM/yasm-test/pull/111)

- [chore(deps-dev): Bump @types/node from 20.14.2 to 20.14.9](https://github.com/PRODYNA-YASM/yasm-test/pull/107)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [1.30.1](https://github.com/PRODYNA-YASM/yasm-test/releases/tag/1.30.1) on 2024-06-14 13:28:41 +0000 UTC

- [1.30.0](https://github.com/PRODYNA-YASM/yasm-test/releases/tag/v1.30.0) on 2024-06-14 04:09:33 +0000 UTC

- [1.30.0](https://github.com/PRODYNA-YASM/yasm-test/releases/tag/1.30.0) on 2024-06-14 04:09:33 +0000 UTC






## [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) 1.1.0






### [Open Pull Requests](https://github.com/prodyna-yasm/sales-copilot/pulls) (2)

- [Bump docker/build-push-action from 5 to 6](https://github.com/PRODYNA-YASM/sales-copilot/pull/5)

- [fix: Handle `"location": null` in organization object](https://github.com/PRODYNA-YASM/sales-copilot/pull/4)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.1.0 |  1.1.0 |  1.1.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [QR-Code improvements](https://github.com/PRODYNA-YASM/sales-copilot/releases/tag/1.1.0) on 2024-06-06 14:06:55 +0000 UTC

- [1.0.1 Formatting and Crash Fixes](https://github.com/PRODYNA-YASM/sales-copilot/releases/tag/1.0.1) on 2024-05-24 08:34:42 +0000 UTC

- [Version 1.0.0](https://github.com/PRODYNA-YASM/sales-copilot/releases/tag/1.0.0) on 2024-05-14 11:34:42 +0000 UTC







---

Created with :heart: by the GitHub Action [deployment-overview](https://github.com/prodyna/deployment-overview) by [@dkrizic](https://github.com/dkrizic)

