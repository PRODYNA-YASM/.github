# YASM Deployment Overview

Component Status overview. Last update 2024-07-03T07:32:13Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :red_square: [7](https://github.com/prodyna-yasm/yasm-backend/compare/1.34.0..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.34.0 |  :red_square: 2bc5df6 |  :green_square: 1.34.0 |  :red_square: 1.32.0 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :red_square: [3](https://github.com/prodyna-yasm/yasm-frontend/compare/1.34.0..HEAD) | :yellow_square: [6](https://github.com/prodyna-yasm/yasm-frontend/pulls) | 1.34.0 |  :red_square: 33ce466 |  :green_square: 1.34.0 |  :red_square: 1.32.0 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :red_square: [10](https://github.com/prodyna-yasm/yasm-integration/compare/1.33.0..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-integration/pulls) | 1.33.0 |  :red_square: f5cf679 |  :green_square: 1.33.0 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :red_square: [18](https://github.com/prodyna-yasm/yasmctl/compare/1.33.0..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasmctl/pulls) | 1.33.0 |  :red_square: 941c10b |  :green_square: 1.33.0 |  :red_square: 1.32.0 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :red_square: [4](https://github.com/prodyna-yasm/yasm-proxy-odbc/compare/1.15.0..HEAD) | :green_square: 0 | 1.15.0 |  :red_square: a213f25 |  :green_square: 1.15.0 |  :green_square: 1.15.0 | 
| [yasm-github](https://github.com/prodyna-yasm/yasm-github) | :red_square: [10](https://github.com/prodyna-yasm/yasm-github/compare/1.5.1..HEAD) | :green_square: 0 | 1.5.1 |  :red_square: 28a065b |  :green_square: 1.5.1 |  :green_square: 1.5.1 | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :red_square: [8](https://github.com/prodyna-yasm/yasm-geocoding/compare/1.10.0..HEAD) | :green_square: 0 | 1.10.0 |  :red_square: c0384fa |  :green_square: 1.10.0 |  :red_square: 1.9.13 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :red_square: [2](https://github.com/prodyna-yasm/yasm-data/compare/1.26.0..HEAD) | :green_square: 0 | 1.26.0 |  :red_square: a59d951 |  :green_square: 1.26.0 |  :green_square: 1.26.0 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.7.0-2 |  :green_square: 8.7.0-2 |  :green_square: 8.7.0-2 |  :green_square: 8.7.0-2 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :red_square: [20](https://github.com/prodyna-yasm/yasm-infrastructure-staged/compare/1.30.0..HEAD) | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-infrastructure-staged/pulls) | 1.30.0 |  :red_square: e7460a0 |  :green_square: 1.30.0 |  :green_square: 1.30.0 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :green_square: 0 | :yellow_square: [4](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.36.0 | 
| [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) | :green_square: 0 | :yellow_square: [3](https://github.com/prodyna-yasm/yasm-nginx/pulls) | 1.25.4-2 | 
| [yasm-test](https://github.com/prodyna-yasm/yasm-test) | :green_square: 0 | :yellow_square: [6](https://github.com/prodyna-yasm/yasm-test/pulls) | 1.30.1 | 
| [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/sales-copilot/pulls) | 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.34.0




### [Commits on main since 1.34.0](https://github.com/prodyna-yasm/yasm-backend/compare/1.34.0..HEAD) (7)

- [feat: search for offices in global search and add office score (#666)](https://github.com/prodyna-yasm/yasm-backend/commit/2bc5df69a407ddc66db68f1697afe32a0b248b5c) by [saemik94](https://github.com/saemik94) on 2024-07-02 07:44:07 +0000 UTC

- [fix: only return offices with at least one assigned person in the global search (#665)](https://github.com/prodyna-yasm/yasm-backend/commit/51e83d7dcf5a0aff3adc904afeef6d53506d660b) by [saemik94](https://github.com/saemik94) on 2024-07-02 06:35:10 +0000 UTC

- [fix: delete org skill audit (#669)](https://github.com/prodyna-yasm/yasm-backend/commit/e122b45a173838b19e4b73a2d8a7006c06178fed) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-28 14:08:50 +0000 UTC

- [build(deps): pipeline update build-push-action (#671)](https://github.com/prodyna-yasm/yasm-backend/commit/4cd53fb518dae4ee2c97e05ec4698c91d1100dd9) by [coding4kay](https://github.com/coding4kay) on 2024-06-28 10:53:52 +0000 UTC

- [build(deps): update quarkus (#670)](https://github.com/prodyna-yasm/yasm-backend/commit/ea01cea261c24e032f6587eb1a8a0ee7671faff3) by [coding4kay](https://github.com/coding4kay) on 2024-06-28 10:09:22 +0000 UTC

- [feat: show the number of direct and related search results (#664)](https://github.com/prodyna-yasm/yasm-backend/commit/deee49c6746fd0b03f8b5aa411ed46f6d195ba2d) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-27 12:57:52 +0000 UTC

- [feat: 15 update audit on relation change (#667)](https://github.com/prodyna-yasm/yasm-backend/commit/eb4fbe7212d9a3d4d49bc30880fc490218c6e4e4) by [coding4kay](https://github.com/coding4kay) on 2024-06-26 17:09:12 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-backend/pulls) (1)

- [Bump eclipse-temurin from 21.0.2_13-jre-ubi9-minimal to 22.0.1_8-jre-ubi9-minimal](https://github.com/PRODYNA-YASM/yasm-backend/pull/588)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  2bc5df6 |  1.34.0 |  1.32.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :red_square: | 


### Last releases

- [Added audit log, added person skill statistic endpoint, add role-check-security in BE to edit entities](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.34.0) on 2024-06-24 11:04:59 +0000 UTC

- [Improve entitiy specific search, increase payload size to 3MB and extend search metric](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.32.0) on 2024-06-18 12:16:59 +0000 UTC

- [Bookmarks and active user filter](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.29.0) on 2024-06-07 09:33:51 +0000 UTC






## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.34.0




### [Commits on main since 1.34.0](https://github.com/prodyna-yasm/yasm-frontend/compare/1.34.0..HEAD) (3)

- [chore: update api version (#766)](https://github.com/prodyna-yasm/yasm-frontend/commit/33ce466eeb6f6566b55264f14fd447e563043673) by [saemik94](https://github.com/saemik94) on 2024-07-02 07:33:27 +0000 UTC

- [feat: project participation (#765)](https://github.com/prodyna-yasm/yasm-frontend/commit/39ee8689564f5db9a7fbaa3e83b1c4536ccb00be) by [readmey](https://github.com/readmey) on 2024-07-02 07:21:42 +0000 UTC

- [feat: search and filter for offices using the global search (#764)](https://github.com/prodyna-yasm/yasm-frontend/commit/d1e511f2efe0a42b0008519b334523971a3460df) by [saemik94](https://github.com/saemik94) on 2024-07-02 07:00:14 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-frontend/pulls) (6)

- [chore: bump @types/node from 20.14.0 to 20.14.9](https://github.com/PRODYNA-YASM/yasm-frontend/pull/763)

- [chore: bump @opentelemetry/instrumentation from 0.43.0 to 0.52.1](https://github.com/PRODYNA-YASM/yasm-frontend/pull/754)

- [chore: bump ws from 7.5.9 to 7.5.10](https://github.com/PRODYNA-YASM/yasm-frontend/pull/745)

- [chore: bump memfs from 3.5.3 to 4.9.3](https://github.com/PRODYNA-YASM/yasm-frontend/pull/738)

- [Bump rimraf from 4.4.1 to 5.0.7](https://github.com/PRODYNA-YASM/yasm-frontend/pull/682)

- [Bump html-loader from 1.3.2 to 5.0.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/619)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  33ce466 |  1.34.0 |  1.32.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :red_square: | 


### Last releases

- [Improvements in yasm-test pipeline, refactor Projects-Detail-View, improved Employee-Detail-View.](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.34.0) on 2024-06-24 14:51:13 +0000 UTC

- [Sort Skills alphabetically in PdfExport, fixed skill administration bugs,  Update Employee and Organization card design, fixed user cannot delete project](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.32.0) on 2024-06-18 12:38:19 +0000 UTC

- [Synchronize Select of Skills&Methodologies, Update Project after edit (without refresh) and fixed deleting organization](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.29.1) on 2024-06-07 14:53:18 +0000 UTC






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.33.0




### [Commits on main since 1.33.0](https://github.com/prodyna-yasm/yasm-integration/compare/1.33.0..HEAD) (10)

- [Merge pull request #460 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/sdk/metric-1.28.0](https://github.com/prodyna-yasm/yasm-integration/commit/f5cf679ff223875f2251cb0e5411114d5e27fa96) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 07:06:46 +0000 UTC

- [Merge pull request #461 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlpmetric/otlpmetricgrpc-1.28.0](https://github.com/prodyna-yasm/yasm-integration/commit/77943c250a41fa07010a29abfa9d80981057d320) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 07:06:38 +0000 UTC

- [Bump go.opentelemetry.io/otel/sdk/metric from 1.27.0 to 1.28.0](https://github.com/prodyna-yasm/yasm-integration/commit/313f94ff6165856a6555debb00131a9a661363ee) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 05:05:15 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlpmetric/otlpmetricgrpc](https://github.com/prodyna-yasm/yasm-integration/commit/62e8181481913e02fe1b0dec107f198b00cd6992) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 05:05:12 +0000 UTC

- [Merge pull request #463 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracegrpc-1.28.0](https://github.com/prodyna-yasm/yasm-integration/commit/7b33ad7975f6bcc2adb47aa01ed74d9bcbbb2870) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 05:04:26 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracegrpc](https://github.com/prodyna-yasm/yasm-integration/commit/d6e4d9911f0b41990ecfc6905d5c6934f44d9f46) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 01:22:57 +0000 UTC

- [Merge pull request #458 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.35.0](https://github.com/prodyna-yasm/yasm-integration/commit/d4a3b734efee42f56a3ee89c940ff86e35491a04) by [dkrizic](https://github.com/dkrizic) on 2024-06-27 04:05:34 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.34.0 to 1.35.0](https://github.com/prodyna-yasm/yasm-integration/commit/61c40bc6378d1cef0a242af3b39aac4c15642acd) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-27 01:24:52 +0000 UTC

- [Merge pull request #457 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.34.0](https://github.com/prodyna-yasm/yasm-integration/commit/fc8813dca30abcfb5afbfcd7dbde2ef2dfd2a2c7) by [dkrizic](https://github.com/dkrizic) on 2024-06-24 03:52:32 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.32.0 to 1.34.0](https://github.com/prodyna-yasm/yasm-integration/commit/a1f8580936c213d1b7d71de9864e9816a0e08cf9) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-24 02:00:12 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-integration/pulls) (1)

- [API 1.36.0 and other dependencies](https://github.com/PRODYNA-YASM/yasm-integration/pull/465)



### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  f5cf679 |  1.33.0 | 
| Release |  :red_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: | 


### Last releases

- [Using API 1.33, some components updated](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.33.0) on 2024-06-21 06:37:58 +0000 UTC

- [Fix bug when an office has no Geolocation](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.32.1) on 2024-06-19 11:26:46 +0000 UTC

- [API 1.32](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.32.0) on 2024-06-18 13:18:23 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-integration/actions?query=is%3Awaiting) (3)

- [Merge pull request #455 from PRODYNA-YASM/dependabot/docker/alpine-3.…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9611541286) created on 2024-06-21 09:35:29 +0000 UTC

- [Merge pull request #445 from PRODYNA-YASM/feature/technology-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9499658142) created on 2024-06-13 12:30:50 +0000 UTC

- [Merge pull request #437 from PRODYNA-YASM/feature/update-components](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9413568240) created on 2024-06-07 07:51:14 +0000 UTC




## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.33.0




### [Commits on main since 1.33.0](https://github.com/prodyna-yasm/yasmctl/compare/1.33.0..HEAD) (18)

- [Merge pull request #355 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.36.0](https://github.com/prodyna-yasm/yasmctl/commit/941c10b88925b11ad15ee22439263aa0654b6e12) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 05:08:08 +0000 UTC

- [Merge pull request #356 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracehttp-1.28.0](https://github.com/prodyna-yasm/yasmctl/commit/ff4ac5f7c7e0f2a928dfebefdf9ae1c94553bcd9) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 05:07:57 +0000 UTC

- [Bump go.opentelemetry.io/otel/exporters/otlp/otlptrace/otlptracehttp](https://github.com/prodyna-yasm/yasmctl/commit/2a66ccc72dbdb251fa8c53bfdbd39d89d3014ee6) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-02 21:28:35 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.35.0 to 1.36.0](https://github.com/prodyna-yasm/yasmctl/commit/b08e326d5a6d1dcc412a5d7ab29e6904f262636b) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-02 21:28:27 +0000 UTC

- [Merge pull request #352 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.35.0](https://github.com/prodyna-yasm/yasmctl/commit/c0ea5827e21cfc76c3302c3fa67133601dced874) by [dkrizic](https://github.com/dkrizic) on 2024-06-26 22:03:28 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.34.0 to 1.35.0](https://github.com/prodyna-yasm/yasmctl/commit/4954966554ed2727b3bbadabd71fba852d6dc094) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-26 21:19:17 +0000 UTC

- [Merge pull request #351 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.34.0](https://github.com/prodyna-yasm/yasmctl/commit/ef2ff8cc154d5e5bab70e129538d42d8434f0929) by [dkrizic](https://github.com/dkrizic) on 2024-06-24 21:41:35 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.33.0 to 1.34.0](https://github.com/prodyna-yasm/yasmctl/commit/437b5920a945442b1848b1942f713dff67d514b6) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-24 21:22:08 +0000 UTC

- [Merge pull request #350 from PRODYNA-YASM/346-dummy-else](https://github.com/prodyna-yasm/yasmctl/commit/ea0df991dd583e2a9fac9d7478c8ab9f0e75c6c6) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:19:06 +0000 UTC

- [Merge pull request #347 from PRODYNA-YASM/343-dummy-feature-enhancement](https://github.com/prodyna-yasm/yasmctl/commit/8726b45e147a78126bff5ab7e0e3c5dd1b159302) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:18:09 +0000 UTC

- [Merge pull request #348 from PRODYNA-YASM/345-dummy-dependency](https://github.com/prodyna-yasm/yasmctl/commit/e44f625f9c227a6e91aea7c62fa544f835764df6) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:18:00 +0000 UTC

- [Merge pull request #349 from PRODYNA-YASM/344-dummy-bugfix](https://github.com/prodyna-yasm/yasmctl/commit/423ac13f1e2dcd19f79a012fe126f060ec477a79) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:17:48 +0000 UTC

- [Remove license file](https://github.com/prodyna-yasm/yasmctl/commit/c0a9b1a324dcdad77f147fb7abaf5109d98edf4e) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:16:45 +0000 UTC

- [Dummy bugfix](https://github.com/prodyna-yasm/yasmctl/commit/c41203a81d66a911b0b47e4bcb4dd0a39ab0af80) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:15:00 +0000 UTC

- [Dummy feature](https://github.com/prodyna-yasm/yasmctl/commit/bbd1101cc1a1c36189e01f002bcf05e6269d9e6e) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:12:47 +0000 UTC

- [Dummy dependency](https://github.com/prodyna-yasm/yasmctl/commit/b148463b2e7357de91c8932448ef11a3031ba9c9) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:11:55 +0000 UTC

- [Add dummy feature](https://github.com/prodyna-yasm/yasmctl/commit/324f5221ed38f82508023cc2f805dae0a8b0aa91) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:09:33 +0000 UTC

- [Update release.yaml configuration](https://github.com/prodyna-yasm/yasmctl/commit/53b250b847d246e322a0a675b2d8363f69219b5a) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 10:08:59 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasmctl/pulls) (1)

- [Using API 1.36.0 and other component updates](https://github.com/PRODYNA-YASM/yasmctl/pull/359)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  941c10b |  1.33.0 |  1.32.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :red_square: | 


### Last releases

- [Using API 1.33](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.33.0) on 2024-06-21 09:26:13 +0000 UTC

- [1.32.0Using API 1.32 and some dependencies](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.32.0) on 2024-06-18 15:17:33 +0000 UTC

- [Using API 1.30.0](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.30.0) on 2024-06-12 07:13:55 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (2)

- [Merge pull request #342 from PRODYNA-YASM/341-use-api-133](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9611533495) created on 2024-06-21 09:34:55 +0000 UTC

- [Merge pull request #336 from PRODYNA-YASM/feature/fix-codeql](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9499139781) created on 2024-06-13 11:55:47 +0000 UTC




## [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) 1.15.0




### [Commits on main since 1.15.0](https://github.com/prodyna-yasm/yasm-proxy-odbc/compare/1.15.0..HEAD) (4)

- [Merge pull request #208 from PRODYNA-YASM/dependabot/go_modules/github.com/go-chi/chi/v5-5.1.0](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/a213f257c745bf6b3961a74259b4c9426be07f43) by [dkrizic](https://github.com/dkrizic) on 2024-07-01 14:01:36 +0000 UTC

- [Bump github.com/go-chi/chi/v5 from 5.0.14 to 5.1.0](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/f01400a7b9dedcde19ad4a2a46a686e2462b59a8) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-01 13:58:24 +0000 UTC

- [Merge pull request #207 from PRODYNA-YASM/dependabot/go_modules/github.com/go-chi/chi/v5-5.0.14](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/6239c25b09b57958c99ccc87d719597287b6e6ce) by [dkrizic](https://github.com/dkrizic) on 2024-06-24 17:19:32 +0000 UTC

- [Bump github.com/go-chi/chi/v5 from 5.0.13 to 5.0.14](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/a6a842b9b07f3844c04742dd248073d95e08c056) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-24 13:17:41 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  a213f25 |  1.15.0 |  1.15.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Technology update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.15.0) on 2024-06-21 09:32:17 +0000 UTC

- [Component update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.14.0) on 2024-06-17 15:39:02 +0000 UTC

- [Components update, CodeQL activated](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.13.0) on 2024-06-12 07:20:24 +0000 UTC






## [yasm-github](https://github.com/prodyna-yasm/yasm-github) 1.5.1




### [Commits on main since 1.5.1](https://github.com/prodyna-yasm/yasm-github/compare/1.5.1..HEAD) (10)

- [Merge pull request #101 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/sdk/metric-1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/28a065bbf8b6572635ddb39f7800984be8d7e583) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 07:03:27 +0000 UTC

- [Bump go.opentelemetry.io/otel/sdk/metric from 1.27.0 to 1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/1a24ba34f39952cddec521e671d5be72c614d28f) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 06:23:25 +0000 UTC

- [Merge pull request #103 from PRODYNA-YASM/dependabot/go_modules/google.golang.org/grpc-1.65.0](https://github.com/prodyna-yasm/yasm-github/commit/b2d1ea921ce1e25ae2506f75ac74f9e6463fa09b) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 06:22:09 +0000 UTC

- [Merge pull request #104 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/sdk-1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/3d2cb00169f89d11852d1e1e9568d2a2f410866e) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 06:19:03 +0000 UTC

- [Bump google.golang.org/grpc from 1.64.0 to 1.65.0](https://github.com/prodyna-yasm/yasm-github/commit/1481efe0e49b3cc8edc3aa24d3597e006b1dbda4) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 05:07:06 +0000 UTC

- [Bump go.opentelemetry.io/otel/sdk from 1.27.0 to 1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/ed2b5a7592d729790749bddb12d9ee4336585fc3) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 05:07:01 +0000 UTC

- [Merge pull request #102 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel/trace-1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/cb4fed0c1e0cc48a4f19433ba2fd22b1a1cae0df) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 05:06:13 +0000 UTC

- [Merge pull request #105 from PRODYNA-YASM/dependabot/go_modules/go.opentelemetry.io/otel-1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/d639ab2dc1f470e12358009f63eaf55ee0f3e78b) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 05:05:41 +0000 UTC

- [Bump go.opentelemetry.io/otel from 1.27.0 to 1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/051c3301f996b95bdb9fd17568b636b4157237e9) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 00:04:08 +0000 UTC

- [Bump go.opentelemetry.io/otel/trace from 1.27.0 to 1.28.0](https://github.com/prodyna-yasm/yasm-github/commit/d60d7077988524f2ee2b7bf92e1b3c8ceb5e5334) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-03 00:03:59 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  28a065b |  1.5.1 |  1.5.1 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Technology update, setting network peer for OpenTelemetry](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.5.1) on 2024-06-21 09:32:02 +0000 UTC

- [CodeQL activated](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.5.0) on 2024-06-12 07:23:18 +0000 UTC

- [Component update](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.9) on 2024-06-05 13:22:56 +0000 UTC






## [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) 1.10.0




### [Commits on main since 1.10.0](https://github.com/prodyna-yasm/yasm-geocoding/compare/1.10.0..HEAD) (8)

- [Merge pull request #127 from PRODYNA-YASM/dependabot/go_modules/google.golang.org/grpc-1.65.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/c0384fa3601b3085f0f8dba4acbe9d12bbbfbb91) by [dkrizic](https://github.com/dkrizic) on 2024-07-02 17:50:16 +0000 UTC

- [Bump google.golang.org/grpc from 1.64.0 to 1.65.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/23e7d0dd4966f33353db54448b9866df97005776) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-07-02 16:50:43 +0000 UTC

- [Merge pull request #126 from PRODYNA-YASM/dependabot/go_modules/github.com/go-chi/chi/v5-5.1.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/b7167de434bdc7bd73bce1344cd4c9327c321b7f) by [dkrizic](https://github.com/dkrizic) on 2024-06-28 17:20:00 +0000 UTC

- [Bump github.com/go-chi/chi/v5 from 5.0.14 to 5.1.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/77ce4d92f442f3160b79073fdf658298633dc0c8) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-28 16:54:38 +0000 UTC

- [Merge pull request #125 from PRODYNA-YASM/dependabot/go_modules/github.com/go-chi/chi/v5-5.0.14](https://github.com/prodyna-yasm/yasm-geocoding/commit/223bc3f6641d7fb80248852f41e9b8b638951374) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 18:50:58 +0000 UTC

- [Bump github.com/go-chi/chi/v5 from 5.0.13 to 5.0.14](https://github.com/prodyna-yasm/yasm-geocoding/commit/497c17ee4f2dc0e741d1785f2eef8016cc0b06eb) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-21 16:55:04 +0000 UTC

- [Merge pull request #124 from PRODYNA-YASM/dependabot/docker/alpine-3.20.1](https://github.com/prodyna-yasm/yasm-geocoding/commit/74b3a8ad843621188fae31a0a0235e555ebcf0eb) by [dkrizic](https://github.com/dkrizic) on 2024-06-21 16:18:06 +0000 UTC

- [Bump alpine from 3.20.0 to 3.20.1](https://github.com/prodyna-yasm/yasm-geocoding/commit/12a3fab41cbcb14e937581b6fe218201af160b60) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-21 16:08:54 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  c0384fa |  1.10.0 |  1.9.13 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :red_square: | 


### Last releases

- [Component update](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.10.0) on 2024-06-20 09:47:44 +0000 UTC

- [Component update](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.13) on 2024-06-05 17:15:09 +0000 UTC

- [Alpine 3.20](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.12) on 2024-05-23 17:16:53 +0000 UTC




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






## [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) 8.7.0-2







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  8.7.0-2 |  8.7.0-2 |  8.7.0-2 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Build push action v6](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.7.0-2) on 2024-06-18 00:21:00 +0000 UTC

- [Gotenberg 8.7.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.7.0-1) on 2024-06-14 03:54:46 +0000 UTC

- [Gotenberg 8.6.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.6.0-1) on 2024-06-07 07:43:03 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-gotenberg/actions?query=is%3Awaiting) (1)

- [Merge pull request #45 from PRODYNA-YASM/dependabot/docker/gotenberg/…](https://github.com/PRODYNA-YASM/yasm-gotenberg/actions/runs/9512157562) created on 2024-06-14 07:12:42 +0000 UTC




## [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) 1.30.0




### [Commits on main since 1.30.0](https://github.com/prodyna-yasm/yasm-infrastructure-staged/compare/1.30.0..HEAD) (20)

- [Merge pull request #555 from PRODYNA-YASM/554-update-components](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/e7460a01ae66b40615f21ef89c0a24d34543ac9c) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 07:11:27 +0000 UTC

- [GitHub 6.2.2 not available yet](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/79bbcd6c1099beb0c34135fbc27372c0c859863d) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 07:08:16 +0000 UTC

- [Update versions of providers](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/8489d3ce80f67baa8a9549a0a396d0e7eb8b4874) by [dkrizic](https://github.com/dkrizic) on 2024-07-03 07:05:40 +0000 UTC

- [Merge pull request #549 from PRODYNA-YASM/545-opentelemetry-collector-0933](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/ce06eab1d074333b0b3a7fe1d6267fcb36cc6224) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 09:23:51 +0000 UTC

- [Fix names of environment variables](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/61053255af75fa36b89029dd8a22d2b474f37170) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 09:17:56 +0000 UTC

- [Merge pull request #548 from PRODYNA-YASM/545-opentelemetry-collector-0933](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/24d3b0c2311f41140bb8f4efdc92c118d8f164ad) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 09:07:52 +0000 UTC

- [Use connection string](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/04a398687be4046ed8c32ab1034b1709208f2c86) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 09:03:58 +0000 UTC

- [Merge pull request #547 from PRODYNA-YASM/545-opentelemetry-collector-0933](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/bfa3f457b06c4b6dd6ec8b2dd7bed5a512ef309f) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 07:06:51 +0000 UTC

- [Merge pull request #546 from PRODYNA-YASM/542-grafana-802](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/ac0523532e83a60031303a30c9f979ff9b5dbdec) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 06:59:09 +0000 UTC

- [Grafana 8.0.2](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/1d612e2af99ff838434253702a75ea1551ea298c) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 06:56:48 +0000 UTC

- [Update OpenTelemetry Collector](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/96149debbdc2ac4f7a2108b1d26e461833f59997) by [dkrizic](https://github.com/dkrizic) on 2024-06-20 06:55:13 +0000 UTC

- [Merge pull request #541 from PRODYNA-YASM/539-feat-enable-datadog-temporarily](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/94b2a02c97970612400797f754d463189b07abda) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 10:40:10 +0000 UTC

- [Only use exporter for Datadog](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/1236b6ccbe8b62a0cf087146563b776115b81864) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 10:32:11 +0000 UTC

- [Merge pull request #540 from PRODYNA-YASM/539-feat-enable-datadog-temporarily](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/89484ba0603ab9c96106be6ef0ddebae83f675dd) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 10:11:41 +0000 UTC

- [Back to GitHub 6.2.1](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/66f606738d1ce8e6584117c87bde018f420514b9) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 10:07:46 +0000 UTC

- [Update provider](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/9c5294dbebf894b539002c8884c4212ea18c6641) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 09:57:38 +0000 UTC

- [Enable datadog for now](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/e7648182fb4b79bd71d5893d4d87e28a275a14c8) by [dkrizic](https://github.com/dkrizic) on 2024-06-18 09:19:24 +0000 UTC

- [Merge pull request #537 from PRODYNA-YASM/536-fix-pod-association](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/bba65e9ca3b922696c36d3051e6df29f74601234) by [dkrizic](https://github.com/dkrizic) on 2024-06-17 09:09:41 +0000 UTC

- [Fix pod association, chore, some update](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/ca48392d1100e9cb04732fb935c1894b4970f0e3) by [dkrizic](https://github.com/dkrizic) on 2024-06-17 08:45:34 +0000 UTC

- [Try to match the pod metadata](https://github.com/prodyna-yasm/yasm-infrastructure-staged/commit/d964e55857592dd826fea07e2430268c6e41100e) by [dkrizic](https://github.com/dkrizic) on 2024-06-14 10:27:48 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-infrastructure-staged/pulls) (2)

- [Update Cert-Manager to 1.15.1](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/pull/556)

- [Bump github from 6.2.1 to 6.2.2 in /terraform/azure](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/pull/538)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  e7460a0 |  1.30.0 |  1.30.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Updated providers](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.30.0) on 2024-06-10 23:20:11 +0000 UTC

- [DAPR 1.13.4](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.27.1) on 2024-06-02 16:10:22 +0000 UTC

- [Kubernetes 1.29.4 and some other updates](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.27.0) on 2024-06-01 10:32:03 +0000 UTC






## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.36.0






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

- [Add dedicated score types](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.36.0) on 2024-07-02 07:10:02 +0000 UTC

- [Audit to Availability](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.35.0) on 2024-06-26 16:32:56 +0000 UTC

- [Audit](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.34.0) on 2024-06-22 00:02:25 +0000 UTC






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

- [chore(deps): Bump @azure/msal-node from 2.7.0 to 2.10.0](https://github.com/PRODYNA-YASM/yasm-test/pull/113)

- [chore(deps-dev): Bump cypress from 13.11.0 to 13.13.0](https://github.com/PRODYNA-YASM/yasm-test/pull/112)

- [chore(deps-dev): Bump typescript from 5.4.5 to 5.5.3](https://github.com/PRODYNA-YASM/yasm-test/pull/111)

- [chore(deps): Bump jose from 5.4.0 to 5.6.2](https://github.com/PRODYNA-YASM/yasm-test/pull/110)

- [chore(deps-dev): Bump @types/node from 20.14.2 to 20.14.9](https://github.com/PRODYNA-YASM/yasm-test/pull/107)

- [chore(deps): Bump cypress/included from 13.11.0 to 13.12.0](https://github.com/PRODYNA-YASM/yasm-test/pull/102)



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

