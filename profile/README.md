# YASM Deployment Overview

Component Status overview. Last update 2024-03-20T12:14:34Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :red_square: [3](https://github.com/prodyna-yasm/yasm-backend/compare/1.16.1..HEAD) | :yellow_square: [4](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.16.1 |  :red_square: 9a75967 |  :green_square: 1.16.1 |  :green_square: 1.16.1 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :red_square: [6](https://github.com/prodyna-yasm/yasm-frontend/compare/1.16.4..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-frontend/pulls) | 1.16.4 |  :red_square: 2c765ef |  :green_square: 1.16.4 |  :green_square: 1.16.4 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :green_square: 0 | :green_square: 0 | 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :green_square: 0 | :green_square: 0 | 1.11.0 |  :green_square: 1.11.0 |  :green_square: 1.11.0 |  :green_square: 1.11.0 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :green_square: 0 | :green_square: 0 | 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 | 
| [yasm-github](https://github.com/prodyna-yasm/yasm-github) | :red_square: [15](https://github.com/prodyna-yasm/yasm-github/compare/..HEAD) | :green_square: 0 |  |  :red_square: 210ac0d | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :green_square: 0 | :green_square: 0 | 1.4.0 |  :green_square: 1.4.0 |  :green_square: 1.4.0 |  :green_square: 1.4.0 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :green_square: 0 | :green_square: 0 | 1.10.0 |  :green_square: 1.10.0 |  :green_square: 1.10.0 |  :red_square: 1.9.0 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.2.2-2 |  :green_square: 8.2.2-2 |  :green_square: 8.2.2-2 |  :green_square: 8.2.2-2 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :green_square: 0 | :green_square: 0 | 1.16.2 |  :green_square: 1.16.2 |  :green_square: 1.16.2 |  :red_square: 1.16.1 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :red_square: [4](https://github.com/prodyna-yasm/yasm-api/compare/1.16.1..HEAD) | :yellow_square: [3](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.16.1 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.16.1




### [Commits on master since 1.16.1](https://github.com/prodyna-yasm/yasm-backend/compare/1.16.1..HEAD) (3)

- [Merge pull request #549 from PRODYNA-YASM/feature/548-create-a-new-prodyna-pat-to-use-when-creating-ticket-issue-over-yasm-ui-github-api](https://github.com/prodyna-yasm/yasm-backend/commit/9a759679e93e8b0475e12fcaf9b3ae14933709e9) by [dkrizic](https://github.com/dkrizic) on 2024-03-19 09:55:40 +0000 UTC

- [Take PAT from Action secrets and forward to Helm](https://github.com/prodyna-yasm/yasm-backend/commit/6ab898d671d9b9a7efe20b7b3ca846c12ec14723) by [dkrizic](https://github.com/dkrizic) on 2024-03-19 09:37:27 +0000 UTC

- [Add "PAT_ISSUE" to helm chart](https://github.com/prodyna-yasm/yasm-backend/commit/dd06a32aaaae961651d755abb26003fd68853d29) by [dkrizic](https://github.com/dkrizic) on 2024-03-19 09:35:29 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-backend/pulls) (4)

- [Bump quarkus.platform.version from 3.8.2 to 3.8.3](https://github.com/PRODYNA-YASM/yasm-backend/pull/550)

- [Bump org.apache.maven.plugins:maven-compiler-plugin from 3.12.1 to 3.13.0](https://github.com/PRODYNA-YASM/yasm-backend/pull/547)

- [Bump io.quarkiverse.neo4j:quarkus-neo4j from 3.8.0 to 3.8.1](https://github.com/PRODYNA-YASM/yasm-backend/pull/546)

- [Bump jackson.version from 2.16.1 to 2.17.0](https://github.com/PRODYNA-YASM/yasm-backend/pull/538)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  9a75967 |  1.16.1 |  1.16.1 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Fix explodes in openapi schema](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.16.1) on 2024-03-15 18:21:03 +0000 UTC

- [Sort person skills by experience, json logging](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.15.0) on 2024-03-15 12:06:51 +0000 UTC

- [1.13.1](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.13.1) on 2024-03-01 12:34:19 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-backend/actions?query=is%3Awaiting) (1)

- [update quarkus (#541)](https://github.com/PRODYNA-YASM/yasm-backend/actions/runs/8296018731) created on 2024-03-15 12:15:58 +0000 UTC




## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.16.4




### [Commits on master since 1.16.4](https://github.com/prodyna-yasm/yasm-frontend/compare/1.16.4..HEAD) (6)

- [Merge pull request #543 from PRODYNA-YASM/dependabot/github_actions/actions/add-to-project-0.6.1](https://github.com/prodyna-yasm/yasm-frontend/commit/2c765ef2212c7e21247acd50c7e005cfc4d8a35f) by [dkrizic](https://github.com/dkrizic) on 2024-03-20 08:03:20 +0000 UTC

- [Bump actions/add-to-project from 0.6.0 to 0.6.1](https://github.com/prodyna-yasm/yasm-frontend/commit/f2091a2307513f980bc84494af5e0c6bdc1f2822) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-03-20 04:48:35 +0000 UTC

- [Merge pull request #540 from PRODYNA-YASM/feature/293-increase-the-amount-of-focus-skills-to-20-for-export](https://github.com/prodyna-yasm/yasm-frontend/commit/00d8d9bacc0ca29f6c35c5ebc5b8ce20f5a48ff4) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-03-19 09:43:24 +0000 UTC

- [delete variable](https://github.com/prodyna-yasm/yasm-frontend/commit/87eaffc09ff1fd64df350c153f76975ed75d3d99) by [TimSFunk](https://github.com/TimSFunk) on 2024-03-19 09:20:59 +0000 UTC

- [Delete Changes in ExportUserPofile and Modal index.tsx](https://github.com/prodyna-yasm/yasm-frontend/commit/64fb82248beb12f5a24062d02443ac7b8764ccf3) by [TimSFunk](https://github.com/TimSFunk) on 2024-03-19 09:13:17 +0000 UTC

- [Modal height increase for better view](https://github.com/prodyna-yasm/yasm-frontend/commit/3405f0f743a212f07933a905ece63aca5b40ab08) by [TimSFunk](https://github.com/TimSFunk) on 2024-03-18 16:28:39 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-frontend/pulls) (1)

- [Enable depandabot](https://github.com/PRODYNA-YASM/yasm-frontend/pull/542)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  2c765ef |  1.16.4 |  1.16.4 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Fix modal logo search Organization by setting overflowY to visible](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.16.4) on 2024-03-18 11:34:25 +0000 UTC

- [Set SALES_COPILOT URL on prod to empty](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.16.3) on 2024-03-15 22:31:06 +0000 UTC

- [Initialize COPILOT_PROJECTS_URL in base webpack config](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.16.2) on 2024-03-15 19:27:59 +0000 UTC






## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.16.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.16.0 |  1.16.0 |  1.16.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [API 1.16.0](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.16.0) on 2024-03-15 22:43:28 +0000 UTC

- [Auto update deployments](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.15.1) on 2024-03-15 15:25:19 +0000 UTC

- [API 1.5, overview integration](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.15.0) on 2024-03-15 14:46:34 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (2)

- [Merge pull request #284 from PRODYNA-YASM/feature/281-auto-update-aft…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8298432302) created on 2024-03-15 15:15:33 +0000 UTC

- [Merge pull request #273 from PRODYNA-YASM/feature/api-1.4.0](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8164164282) created on 2024-03-05 22:59:56 +0000 UTC




## [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) 1.11.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.11.0 |  1.11.0 |  1.11.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Technical updates](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.0) on 2024-03-15 10:28:15 +0000 UTC

- [Libs updated](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.10.0) on 2024-02-26 13:21:22 +0000 UTC

- [Create virtual node in Service Graph](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.9.0) on 2024-02-24 22:44:44 +0000 UTC






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.16.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.16.0 |  1.16.0 |  1.16.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [API 1.16.1](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.16.0) on 2024-03-18 06:03:04 +0000 UTC

- [API 1.15, Go updates](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.15.0) on 2024-03-15 10:19:32 +0000 UTC

- [Current libs for MS Graph and Helm deployment](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.13.5) on 2024-03-01 09:52:21 +0000 UTC






## [yasm-github](https://github.com/prodyna-yasm/yasm-github) 


> [!WARNING]
> GET https://api.github.com/repos/prodyna-yasm/yasm-github/releases/latest: 404 Not Found []


## [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) 1.4.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.4.0 |  1.4.0 |  1.4.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Go updates](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.4.0) on 2024-03-06 17:05:01 +0000 UTC

- [1.3.0](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.3.0) on 2024-02-29 16:32:20 +0000 UTC

- [OpenTelemetry 1.24.0](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.2.0) on 2024-02-26 16:44:36 +0000 UTC






## [yasm-data](https://github.com/prodyna-yasm/yasm-data) 1.10.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.10.0 |  1.10.0 |  1.9.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [No more certifications](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.0) on 2024-03-18 13:47:12 +0000 UTC

- [1.9.0](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.9.0) on 2024-03-01 13:51:07 +0000 UTC

- [International office names](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.8.0) on 2023-12-14 13:10:13 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-data/actions?query=is%3Awaiting) (1)

- [Merge pull request #114 from PRODYNA-YASM/feature112-prevent-legacy-d…](https://github.com/PRODYNA-YASM/yasm-data/actions/runs/8327746582) created on 2024-03-18 13:50:59 +0000 UTC




## [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) 8.2.2-2







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  8.2.2-2 |  8.2.2-2 |  8.2.2-2 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Gotenberg 8.2.2](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.2.2-2) on 2024-03-18 06:03:48 +0000 UTC

- [Gotenberg 8.2.1](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.2.1-1) on 2024-03-11 06:18:26 +0000 UTC

- [8.2.0-4](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.2.0-4) on 2024-03-04 01:27:19 +0000 UTC






## [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) 1.16.2







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.16.2 |  1.16.2 |  1.16.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [YASM-Github added](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.16.2) on 2024-03-20 10:51:36 +0000 UTC

- [1.16.1](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.16.1) on 2024-03-19 13:04:16 +0000 UTC

- [New version of Grafana stack](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/v1.16.0) on 2024-03-19 13:04:16 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-infrastructure-staged/actions?query=is%3Awaiting) (3)

- [Merge pull request #454 from PRODYNA-YASM/feature/add-yasm-github](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/actions/runs/8357746758) created on 2024-03-20 10:57:27 +0000 UTC

- [Merge pull request #449 from PRODYNA-YASM/feature/445-enable-geoip-mo…](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/actions/runs/8294687130) created on 2024-03-15 10:20:35 +0000 UTC

- [Merge pull request #443 from PRODYNA-YASM/feature/remove-cosmos](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/actions/runs/8208199950) created on 2024-03-08 19:39:55 +0000 UTC




## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.16.1




### [Commits on master since 1.16.1](https://github.com/prodyna-yasm/yasm-api/compare/1.16.1..HEAD) (4)

- [Merge pull request #165 from PRODYNA-YASM/dependabot/maven/org.apache.maven.plugins-maven-compiler-plugin-3.13.0](https://github.com/prodyna-yasm/yasm-api/commit/7278702de748fb2d7063b4f1c3f0101d99358560) by [dkrizic](https://github.com/dkrizic) on 2024-03-19 06:46:15 +0000 UTC

- [Merge pull request #166 from PRODYNA-YASM/dependabot/maven/io.smallrye.reactive-mutiny-2.6.0](https://github.com/prodyna-yasm/yasm-api/commit/552f9a3d1c7be3eb63d2d37fd4d88e3c99b81242) by [dkrizic](https://github.com/dkrizic) on 2024-03-19 06:45:59 +0000 UTC

- [Bump io.smallrye.reactive:mutiny from 2.5.8 to 2.6.0](https://github.com/prodyna-yasm/yasm-api/commit/5b71a0db5f5f161f3b260b3a42e4b459459c33cf) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-03-19 00:54:19 +0000 UTC

- [Bump org.apache.maven.plugins:maven-compiler-plugin](https://github.com/prodyna-yasm/yasm-api/commit/a765114216b0ef761a162169ca1262f528331959) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-03-19 00:54:12 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-api/pulls) (3)

- [Bump com.fasterxml.jackson.core:jackson-databind from 2.16.2 to 2.17.0](https://github.com/PRODYNA-YASM/yasm-api/pull/161)

- [Bump org.openapitools:openapi-generator-maven-plugin from 7.3.0 to 7.4.0](https://github.com/PRODYNA-YASM/yasm-api/pull/160)

- [Draft: Skill kind giver refactoring](https://github.com/PRODYNA-YASM/yasm-api/pull/105)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [Explode query param arrays to false](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.16.1) on 2024-03-15 17:34:56 +0000 UTC

- [change explode in array query params](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.16.0) on 2024-03-15 16:57:58 +0000 UTC

- [1.15.0](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.15.0) on 2024-03-15 09:31:07 +0000 UTC







---

Created with :heart: by the GitHub Action [deployment-overview](https://github.com/prodyna/deployment-overview) by [@dkrizic](https://github.com/dkrizic)

