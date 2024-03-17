# YASM Deployment Overview

Component Status overview. Last update 2024-03-17T20:50:44Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :green_square: 0 | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.16.1 |  :green_square: 1.16.1 |  :green_square: 1.16.1 |  :red_square: 1.13.1 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :green_square: 0 | :green_square: 0 | 1.16.3 |  :green_square: 1.16.3 |  :green_square: 1.16.3 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :green_square: 0 | :green_square: 0 | 1.16.0 |  :green_square: 1.16.0 |  :green_square: 1.16.0 |  :red_square: 1.15.1 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :green_square: 0 | :green_square: 0 | 1.11.0 |  :green_square: 1.11.0 |  :green_square: 1.11.0 |  :green_square: 1.11.0 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :green_square: 0 | :green_square: 0 | 1.15.0 |  :green_square: 1.15.0 |  :green_square: 1.15.0 | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :green_square: 0 | :green_square: 0 | 1.4.0 |  :green_square: 1.4.0 |  :green_square: 1.4.0 |  :green_square: 1.4.0 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :green_square: 0 | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-data/pulls) | 1.9.0 |  :green_square: 1.9.0 |  :green_square: 1.9.0 |  :green_square: 1.9.0 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.2.1-1 |  :green_square: 8.2.1-1 |  :green_square: 8.2.1-1 |  :green_square: 8.2.1-1 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :green_square: 0 | :green_square: 0 | 1.15.1 |  :green_square: 1.15.1 |  :green_square: 1.15.1 |  :green_square: 1.15.1 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :green_square: 0 | :yellow_square: [3](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.16.1 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.16.1






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-backend/pulls) (1)

- [Bump jackson.version from 2.16.1 to 2.17.0](https://github.com/PRODYNA-YASM/yasm-backend/pull/538)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.16.1 |  1.16.1 |  1.13.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [Fix explodes in openapi schema](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.16.1) on 2024-03-15 18:21:03 +0000 UTC

- [Sort person skills by experience, json logging](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.15.0) on 2024-03-15 12:06:51 +0000 UTC

- [1.13.1](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.13.1) on 2024-03-01 12:34:19 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-backend/actions?query=is%3Awaiting) (2)

- [do not run tests on tag or pr merge on master (#545)](https://github.com/PRODYNA-YASM/yasm-backend/actions/runs/8300711918) created on 2024-03-15 18:23:49 +0000 UTC

- [update quarkus (#541)](https://github.com/PRODYNA-YASM/yasm-backend/actions/runs/8296018731) created on 2024-03-15 12:15:58 +0000 UTC




## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.16.3







### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  1.16.3 |  1.16.3 | 
| Release |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: | 


### Last releases

- [Set SALES_COPILOT URL on prod to empty](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.16.3) on 2024-03-15 22:31:06 +0000 UTC

- [Initialize COPILOT_PROJECTS_URL in base webpack config](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.16.2) on 2024-03-15 19:27:59 +0000 UTC

- [Update API to 1.16.1 and removed hacky copilot link check in prod](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.16.1) on 2024-03-15 18:48:26 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-frontend/actions?query=is%3Awaiting) (1)

- [Merge pull request #538 from PRODYNA-YASM/feature/537-copilot-url-on-…](https://github.com/PRODYNA-YASM/yasm-frontend/actions/runs/8306005512) created on 2024-03-16 06:41:01 +0000 UTC




## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.16.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.16.0 |  1.16.0 |  1.15.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [API 1.16.0](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.16.0) on 2024-03-15 22:43:28 +0000 UTC

- [Auto update deployments](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.15.1) on 2024-03-15 15:25:19 +0000 UTC

- [API 1.5, overview integration](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.15.0) on 2024-03-15 14:46:34 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (3)

- [Merge pull request #286 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8303151124) created on 2024-03-15 22:44:18 +0000 UTC

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






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.15.0







### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  1.15.0 |  1.15.0 | 
| Release |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: | 


### Last releases

- [API 1.15, Go updates](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.15.0) on 2024-03-15 10:19:32 +0000 UTC

- [Current libs for MS Graph and Helm deployment](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.13.5) on 2024-03-01 09:52:21 +0000 UTC

- [Virtual nodes, libs updated](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.13.4) on 2024-02-26 15:32:38 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-integration/actions?query=is%3Awaiting) (1)

- [Merge pull request #378 from PRODYNA-YASM/feature/377-api-115](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/8294756781) created on 2024-03-15 10:25:54 +0000 UTC




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






## [yasm-data](https://github.com/prodyna-yasm/yasm-data) 1.9.0






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-data/pulls) (1)

- [Remove organizations, change address of PRODYNA HQ to Neo-Isenburg](https://github.com/PRODYNA-YASM/yasm-data/pull/114)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.9.0 |  1.9.0 |  1.9.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [1.9.0](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.9.0) on 2024-03-01 13:51:07 +0000 UTC

- [International office names](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.8.0) on 2023-12-14 13:10:13 +0000 UTC

- [Dusseldorf synonym für Düsseldorf](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.6.1) on 2023-11-30 18:39:48 +0000 UTC






## [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) 8.2.1-1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  8.2.1-1 |  8.2.1-1 |  8.2.1-1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Gotenberg 8.2.1](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.2.1-1) on 2024-03-11 06:18:26 +0000 UTC

- [8.2.0-4](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.2.0-4) on 2024-03-04 01:27:19 +0000 UTC

- [Update actions](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.2.0-3) on 2024-02-27 02:00:10 +0000 UTC






## [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) 1.15.1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.15.1 |  1.15.1 |  1.15.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Deactivate GeoIP, some components updates](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.15.1) on 2024-03-15 12:56:06 +0000 UTC

- [Ingress-Nginx 1.10, new Grafana, custom error page](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.15.0) on 2024-03-14 10:44:54 +0000 UTC

- [Remove CosmosDB](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.14.0) on 2024-03-08 17:13:16 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-infrastructure-staged/actions?query=is%3Awaiting) (2)

- [Merge pull request #449 from PRODYNA-YASM/feature/445-enable-geoip-mo…](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/actions/runs/8294687130) created on 2024-03-15 10:20:35 +0000 UTC

- [Merge pull request #443 from PRODYNA-YASM/feature/remove-cosmos](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/actions/runs/8208199950) created on 2024-03-08 19:39:55 +0000 UTC




## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.16.1






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

