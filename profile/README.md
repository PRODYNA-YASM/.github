# YASM Deployment Overview

Component Status overview. Last update 2024-06-07T10:11:32Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :red_square: [14](https://github.com/prodyna-yasm/yasm-backend/compare/1.27.0..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.27.0 |  :red_square: afb5211 |  :green_square: 1.27.0 |  :green_square: 1.27.0 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :red_square: [30](https://github.com/prodyna-yasm/yasm-frontend/compare/1.27.1..HEAD) | :yellow_square: [5](https://github.com/prodyna-yasm/yasm-frontend/pulls) | 1.27.1 |  :red_square: 4b83736 |  :green_square: 1.27.1 |  :green_square: 1.27.1 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :green_square: 0 | :green_square: 0 | 1.29.0 |  :green_square: 1.29.0 |  :green_square: 1.29.0 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :green_square: 0 | :green_square: 0 | 1.29.0 |  :green_square: 1.29.0 |  :green_square: 1.29.0 |  :red_square: 1.27.0 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :green_square: 0 | :green_square: 0 | 1.12.1 |  :green_square: 1.12.1 |  :green_square: 1.12.1 |  :green_square: 1.12.1 | 
| [yasm-github](https://github.com/prodyna-yasm/yasm-github) | :green_square: 0 | :green_square: 0 | 1.4.9 |  :green_square: 1.4.9 |  :green_square: 1.4.9 |  :green_square: 1.4.9 | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :green_square: 0 | :green_square: 0 | 1.9.13 |  :green_square: 1.9.13 |  :green_square: 1.9.13 |  :green_square: 1.9.13 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :green_square: 0 | :green_square: 0 | 1.26.0 |  :green_square: 1.26.0 |  :green_square: 1.26.0 |  :green_square: 1.26.0 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.6.0-1 |  :green_square: 8.6.0-1 |  :green_square: 8.6.0-1 |  :green_square: 8.6.0-1 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :green_square: 0 | :green_square: 0 | 1.27.1 |  :green_square: 1.27.1 |  :green_square: 1.27.1 |  :green_square: 1.27.1 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :green_square: 0 | :yellow_square: [3](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.29.0 | 
| [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-nginx/pulls) | 1.25.4-2 | 
| [yasm-test](https://github.com/prodyna-yasm/yasm-test) | :red_square: [16](https://github.com/prodyna-yasm/yasm-test/compare/1.27.0..HEAD) | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-test/pulls) | 1.27.0 | 
| [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) | :green_square: 0 | :green_square: 0 | 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.27.0




### [Commits on main since 1.27.0](https://github.com/prodyna-yasm/yasm-backend/compare/1.27.0..HEAD) (14)

- [fix random person order (#639)](https://github.com/prodyna-yasm/yasm-backend/commit/afb5211cf226a04ae6ac3f8ca30b8fa6f2916949) by [coding4kay](https://github.com/coding4kay) on 2024-06-07 09:33:51 +0000 UTC

- [Merge pull request #638 from PRODYNA-YASM/feature/431-anonymize-export](https://github.com/prodyna-yasm/yasm-backend/commit/96922c1b2dac0346311137eb82c85332b692e5ed) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 09:00:34 +0000 UTC

- [removed unused/old classes and tests](https://github.com/prodyna-yasm/yasm-backend/commit/67e208ff5b1e99bb9bbdf64d8571e8bd17e98f0c) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 08:52:42 +0000 UTC

- [431: add anonymize flag to hide picture in pdfExport, removed githubUser and removed old pdf-profile endpoint](https://github.com/prodyna-yasm/yasm-backend/commit/c5ab005f91357d1434a60df86b5a15d73e51bf62) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-06 15:03:03 +0000 UTC

- [exclude inactive persons from showing up global search (#637)](https://github.com/prodyna-yasm/yasm-backend/commit/d2b26f1b48c83f9a76d8dcdc81fc6ba3d14ebd97) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-06 12:52:14 +0000 UTC

- [update quarkus 3.11.1 (#636)](https://github.com/prodyna-yasm/yasm-backend/commit/5ce9a1e839b5082ede63577f62e6592dd4812177) by [coding4kay](https://github.com/coding4kay) on 2024-06-06 11:34:08 +0000 UTC

- [remove unused fields inside logging (#635)](https://github.com/prodyna-yasm/yasm-backend/commit/1ed4ac546b24564076cb7781c771a31e8c65b338) by [coding4kay](https://github.com/coding4kay) on 2024-06-06 11:06:59 +0000 UTC

- [GeoBuilder return null if no values exist, not an empty object (#633)](https://github.com/prodyna-yasm/yasm-backend/commit/9a6908e6b782be63f006408cd6515517c85e4cf0) by [coding4kay](https://github.com/coding4kay) on 2024-06-05 16:05:46 +0000 UTC

- [add team members to person detail (#632)](https://github.com/prodyna-yasm/yasm-backend/commit/9042645dbb68cd6ce995ed990687edb519a481f5) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-05 11:48:57 +0000 UTC

- [add inactive filter (#631)](https://github.com/prodyna-yasm/yasm-backend/commit/d6a33d37bf42d99506a0ead7d0529c16d63833b6) by [coding4kay](https://github.com/coding4kay) on 2024-06-05 08:53:31 +0000 UTC

- [Fix: Line separator issue on Windows systems (#629)](https://github.com/prodyna-yasm/yasm-backend/commit/5ab0f8d683c313d13a309f6e7e1708c3968f61ea) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-05 07:12:35 +0000 UTC

- [addk enduser.id and enduser.role (#628)](https://github.com/prodyna-yasm/yasm-backend/commit/c694dc3eda2957eb1b56ea63d47fc6b84940865f) by [coding4kay](https://github.com/coding4kay) on 2024-06-04 10:51:58 +0000 UTC

- [add new pdf profile endpoint (#627)](https://github.com/prodyna-yasm/yasm-backend/commit/c1459156ea13ba03195c877a58f2e454f924576c) by [coding4kay](https://github.com/coding4kay) on 2024-06-03 16:47:08 +0000 UTC

- [improve test performance by using oidc mock service (#625)](https://github.com/prodyna-yasm/yasm-backend/commit/59d3e0055c5586d62d1fbd42e14e66ddc618391f) by [coding4kay](https://github.com/coding4kay) on 2024-05-31 13:16:26 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-backend/pulls) (1)

- [Bump eclipse-temurin from 21.0.2_13-jre-ubi9-minimal to 22.0.1_8-jre-ubi9-minimal](https://github.com/PRODYNA-YASM/yasm-backend/pull/588)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  afb5211 |  1.27.0 |  1.27.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Skill importance and extended metrics](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.27.0) on 2024-05-31 12:24:13 +0000 UTC

- [Improve cypher performance and update quarkus](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.2) on 2024-05-24 21:43:36 +0000 UTC

- [Fix skill linking relevant for kindgiver](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.1) on 2024-05-24 09:04:38 +0000 UTC






## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.27.1




### [Commits on main since 1.27.1](https://github.com/prodyna-yasm/yasm-frontend/compare/1.27.1..HEAD) (30)

- [Merge pull request #713 from PRODYNA-YASM/feature/431-anonymize-export](https://github.com/prodyna-yasm/yasm-frontend/commit/4b837365c8f8c08d49fbbbff2f5b08cd2e9c12af) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 09:45:18 +0000 UTC

- [merge main and fixed conflicts](https://github.com/prodyna-yasm/yasm-frontend/commit/5b414e775f8b3a45404e62e25f7367ad3d3a6fa5) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 09:43:18 +0000 UTC

- [update api to 1.29.0](https://github.com/prodyna-yasm/yasm-frontend/commit/8a7d7102f2364869687e2d347a8c50aa0aaabc13) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 09:30:52 +0000 UTC

- [Merge pull request #712 from PRODYNA-YASM/fix/maintainer-can-not-add-organization](https://github.com/prodyna-yasm/yasm-frontend/commit/4963f68afcb3ccab7f920c011ed608984a850a5b) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 07:42:50 +0000 UTC

- [Merge pull request #709 from PRODYNA-YASM/feature/509-link-to-github](https://github.com/prodyna-yasm/yasm-frontend/commit/14eba36a81a15648bfd4c0adc5754c85891d189b) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 07:38:26 +0000 UTC

- [Merge pull request #701 from PRODYNA-YASM/feature/fix-parent-skill-tree](https://github.com/prodyna-yasm/yasm-frontend/commit/7bdde8fb0be85bbb27e4eb5fabda22fdff0c2625) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 07:35:05 +0000 UTC

- [enable Maintainers to CRUD Organization](https://github.com/prodyna-yasm/yasm-frontend/commit/89bd4395edd7ebf838451629f9c64f95995afd54) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-07 07:27:31 +0000 UTC

- [Merge pull request #710 from PRODYNA-YASM/319-feature-requestmore-descriptive-page-titles-for-bookmarking](https://github.com/prodyna-yasm/yasm-frontend/commit/8a2f6de3a95c79047da1b110c0028e735695f37d) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-06 16:05:01 +0000 UTC

- [overwrite document title for bookmarks](https://github.com/prodyna-yasm/yasm-frontend/commit/5178bcf057426943f3dbd1762f8ea67c020d7941) by [coding4kay](https://github.com/coding4kay) on 2024-06-06 16:00:56 +0000 UTC

- [509: added helperContext and add a link to githubProfile in Contact Details](https://github.com/prodyna-yasm/yasm-frontend/commit/eacca30e3b3da8505d910b6b7a4c237b10197f26) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-06 15:32:13 +0000 UTC

- [431: build TemplateObject in FE, enable anonymization and override of Person object for pdf-export](https://github.com/prodyna-yasm/yasm-frontend/commit/6cc150124b5a49141383ba614c7c7c06fb88e7e0) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-06 15:01:27 +0000 UTC

- [Merge pull request #708 from PRODYNA-YASM/707-activate-copilot-for-staging-and-prod-again](https://github.com/prodyna-yasm/yasm-frontend/commit/0ca5ab7096a8143e96ceb56993051179dcfca630) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 14:26:44 +0000 UTC

- [Activate copilot link on production again](https://github.com/prodyna-yasm/yasm-frontend/commit/cf23fc4797e93045a1119aa95b2b8c1616ec140d) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 14:24:56 +0000 UTC

- [change yellow to green xD](https://github.com/prodyna-yasm/yasm-frontend/commit/1e5ea870842e77ee1999dcbb394118a37ddf404b) by [](https://github.com/) on 2024-06-06 13:22:42 +0000 UTC

- [Feature: Exclude inactive persons from showing up global search (#706)](https://github.com/prodyna-yasm/yasm-frontend/commit/604eb930560ef9bfafd0cc17784d34c77bc48231) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-06 13:20:07 +0000 UTC

- [Merge pull request #705 from PRODYNA-YASM/feature/team_member_overview_in_user_profile](https://github.com/prodyna-yasm/yasm-frontend/commit/21403b0971d6595540ce60b4067fc64fbe44d841) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-06 13:08:41 +0000 UTC

- [remove duplicate entries](https://github.com/prodyna-yasm/yasm-frontend/commit/8fbd766eb840bca442d11207e9d1210745454f92) by [saemik94](https://github.com/saemik94) on 2024-06-06 08:25:28 +0000 UTC

- [sort alphabetically](https://github.com/prodyna-yasm/yasm-frontend/commit/3334b3d577adf1e692604baa547b3a116341de53) by [saemik94](https://github.com/saemik94) on 2024-06-06 08:23:59 +0000 UTC

- [refactor code](https://github.com/prodyna-yasm/yasm-frontend/commit/c2d6566b4bd590e4073cc553137612357c69d14a) by [saemik94](https://github.com/saemik94) on 2024-06-06 06:44:43 +0000 UTC

- [fix: flatten svg icon](https://github.com/prodyna-yasm/yasm-frontend/commit/786873d83a6360d4c9672834d85cc0701ffdf124) by [saemik94](https://github.com/saemik94) on 2024-06-06 06:31:39 +0000 UTC

- [wip code refactor](https://github.com/prodyna-yasm/yasm-frontend/commit/689155a6a0a3777351f939ae46e6eb9fd5f5c967) by [saemik94](https://github.com/saemik94) on 2024-06-05 15:50:11 +0000 UTC

- [refactor code](https://github.com/prodyna-yasm/yasm-frontend/commit/9c97fd09bb9966bc39cae5c03f2a256040c3a45f) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-05 14:26:18 +0000 UTC

- [adjust person manager style](https://github.com/prodyna-yasm/yasm-frontend/commit/77424b46717d4e460b3604382cdd7a237c55a5eb) by [saemik94](https://github.com/saemik94) on 2024-06-05 13:59:00 +0000 UTC

- [initial team members implementation](https://github.com/prodyna-yasm/yasm-frontend/commit/44c167a892bb5110284e8db7cdeaab1765ccf4aa) by [mayer-prodyna](https://github.com/mayer-prodyna) on 2024-06-05 13:42:48 +0000 UTC

- [Merge pull request #702 from PRODYNA-YASM/feature/109-charts](https://github.com/prodyna-yasm/yasm-frontend/commit/931fb49a41f5a2dc1e29432b05ab9282529ec43c) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-05 13:11:40 +0000 UTC

- [109: removed warnings and add cursor pointer to BarChart](https://github.com/prodyna-yasm/yasm-frontend/commit/3898483bbc6b234cc05d53bbade6a359112f609e) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-06-05 13:08:27 +0000 UTC

- [add selectable barItems](https://github.com/prodyna-yasm/yasm-frontend/commit/796d6eb8af76e36f519c069d762b9685b75e6f56) by [](https://github.com/) on 2024-06-05 12:50:50 +0000 UTC

- [fix pieChart width](https://github.com/prodyna-yasm/yasm-frontend/commit/6e02349d3b5f79f8ac0cc9cf0c642bcd69fc5ef3) by [](https://github.com/) on 2024-06-05 12:24:45 +0000 UTC

- [remove decimal](https://github.com/prodyna-yasm/yasm-frontend/commit/aa7e503c922decfe069c6eb1e257d11ef4623816) by [](https://github.com/) on 2024-06-05 12:23:58 +0000 UTC

- [fix availability infos](https://github.com/prodyna-yasm/yasm-frontend/commit/af03563b642dcaf9a603e852dcc31c58878e2733) by [](https://github.com/) on 2024-06-05 12:20:08 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-frontend/pulls) (5)

- [Bump @mui/x-date-pickers from 6.20.0 to 7.6.2](https://github.com/PRODYNA-YASM/yasm-frontend/pull/711)

- [Bump chalk from 3.0.0 to 5.3.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/704)

- [Bump rimraf from 4.4.1 to 5.0.7](https://github.com/PRODYNA-YASM/yasm-frontend/pull/682)

- [Bump memfs from 3.5.3 to 4.9.2](https://github.com/PRODYNA-YASM/yasm-frontend/pull/672)

- [Bump html-loader from 1.3.2 to 5.0.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/619)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  4b83736 |  1.27.1 |  1.27.1 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Fixed update OrganizationForm in Project-View](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.27.1) on 2024-06-04 08:00:16 +0000 UTC

- [Added Skill Importance and added title in Changelog](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.27.0) on 2024-05-31 12:43:30 +0000 UTC

- [Added changelog and upgrade dependencies](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.26.2) on 2024-05-29 08:23:30 +0000 UTC






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.29.0







### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  1.29.0 |  1.29.0 | 
| Release |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: | 


### Last releases

- [API 1.29 (making it compatible again)](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.29.0) on 2024-06-07 09:59:15 +0000 UTC

- [API 1.28, component update](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.28.0) on 2024-06-07 07:39:20 +0000 UTC

- [Start date for main projects 2022-07-01](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.27.1) on 2024-06-01 09:58:01 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-integration/actions?query=is%3Awaiting) (7)

- [Merge pull request #438 from PRODYNA-YASM/feature/api-1.29](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9415273300) created on 2024-06-07 10:05:14 +0000 UTC

- [Merge pull request #437 from PRODYNA-YASM/feature/update-components](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9413568240) created on 2024-06-07 07:51:14 +0000 UTC

- [Merge pull request #427 from PRODYNA-YASM/dependabot/docker/alpine-3.…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9207758718) created on 2024-05-23 12:14:09 +0000 UTC

- [Merge pull request #426 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9189201188) created on 2024-05-22 09:56:06 +0000 UTC

- [Merge pull request #421 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9177468495) created on 2024-05-21 15:44:35 +0000 UTC

- [Merge pull request #419 from PRODYNA-YASM/dependabot/go_modules/googl…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9108351279) created on 2024-05-16 07:35:56 +0000 UTC

- [Merge pull request #418 from PRODYNA-YASM/technology-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9077209401) created on 2024-05-14 09:42:04 +0000 UTC




## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.29.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.29.0 |  1.29.0 |  1.27.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [API 1.29](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.29.0) on 2024-06-07 09:57:51 +0000 UTC

- [API 1.28 and Go 1.22.4](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.28.0) on 2024-06-05 13:22:38 +0000 UTC

- [Using API 1.27.0](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.27.0) on 2024-05-31 21:43:46 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (5)

- [Merge pull request #332 from PRODYNA-YASM/feature/api-1.29](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9415201339) created on 2024-06-07 10:00:15 +0000 UTC

- [Merge pull request #331 from PRODYNA-YASM/feature/go-1.22.4](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9413322430) created on 2024-06-07 07:29:11 +0000 UTC

- [Merge pull request #324 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9182087461) created on 2024-05-21 22:05:09 +0000 UTC

- [Merge pull request #320 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9177461182) created on 2024-05-21 15:43:57 +0000 UTC

- [Merge pull request #319 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9077198208) created on 2024-05-14 09:41:06 +0000 UTC




## [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) 1.12.1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.12.1 |  1.12.1 |  1.12.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Technology update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.12.1) on 2024-06-07 07:26:38 +0000 UTC

- [Technology update, start date for main projects back to 2023-07-01](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.12.0) on 2024-05-31 14:42:58 +0000 UTC

- [OpenTelemetry 1.27.0](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.9) on 2024-05-27 14:14:44 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-proxy-odbc/actions?query=is%3Awaiting) (1)

- [Merge pull request #188 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/actions/runs/9177465100) created on 2024-05-21 15:44:16 +0000 UTC




## [yasm-github](https://github.com/prodyna-yasm/yasm-github) 1.4.9







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.4.9 |  1.4.9 |  1.4.9 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Component update](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.9) on 2024-06-05 13:22:56 +0000 UTC

- [Improved error handling](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.8) on 2024-05-28 14:28:02 +0000 UTC

- [OpenTelemetry 1.27](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.7) on 2024-05-22 09:50:59 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-github/actions?query=is%3Awaiting) (1)

- [Merge pull request #82 from PRODYNA-YASM/81-dummy-issue](https://github.com/PRODYNA-YASM/yasm-github/actions/runs/9173421502) created on 2024-05-21 10:50:14 +0000 UTC




## [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) 1.9.13







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.9.13 |  1.9.13 |  1.9.13 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Component update](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.13) on 2024-06-05 17:15:09 +0000 UTC

- [Alpine 3.20](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.12) on 2024-05-23 17:16:53 +0000 UTC

- [OpenTelemetry 1.27](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.11) on 2024-05-22 18:13:49 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-geocoding/actions?query=is%3Awaiting) (1)

- [Merge pull request #112 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasm-geocoding/actions/runs/9207766232) created on 2024-05-23 12:14:39 +0000 UTC




## [yasm-data](https://github.com/prodyna-yasm/yasm-data) 1.26.0







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.26.0 |  1.26.0 |  1.26.0 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Add some roles](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.26.0) on 2024-04-29 06:13:23 +0000 UTC

- [New roles](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.2) on 2024-04-29 06:13:23 +0000 UTC

- [Main branch](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.1) on 2024-04-19 13:36:35 +0000 UTC






## [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) 8.6.0-1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  8.6.0-1 |  8.6.0-1 |  8.6.0-1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Gotenberg 8.6.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.6.0-1) on 2024-06-07 07:43:03 +0000 UTC

- [Gotenberg 8.5.1](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.5.1-1) on 2024-05-27 05:13:43 +0000 UTC

- [Gotenberg 8.5.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.5.0-1) on 2024-04-29 06:09:42 +0000 UTC






## [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) 1.27.1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.27.1 |  1.27.1 |  1.27.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [DAPR 1.13.4](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.27.1) on 2024-06-02 16:10:22 +0000 UTC

- [Kubernetes 1.29.4 and some other updates](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.27.0) on 2024-06-01 10:32:03 +0000 UTC

- [Otel Collector 0.92](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.26.2) on 2024-05-22 11:53:37 +0000 UTC






## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.29.0






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-api/pulls) (3)

- [Feature/324-project-images](https://github.com/PRODYNA-YASM/yasm-api/pull/194)

- [Bump jakarta.ws.rs:jakarta.ws.rs-api from 3.1.0 to 4.0.0](https://github.com/PRODYNA-YASM/yasm-api/pull/180)

- [Draft: Skill kind giver refactoring](https://github.com/PRODYNA-YASM/yasm-api/pull/105)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [Add anonymize flag in pdfProfile, removed GitHubUser and removed old PDFExport endpoint](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.29.0) on 2024-06-07 08:39:04 +0000 UTC

- [Team member in person detail](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.28.0) on 2024-06-05 08:26:56 +0000 UTC

- [Fix Naming](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.27.2) on 2024-06-03 16:33:43 +0000 UTC






## [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) 1.25.4-2






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-nginx/pulls) (2)

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






## [yasm-test](https://github.com/prodyna-yasm/yasm-test) 1.27.0




### [Commits on main since 1.27.0](https://github.com/prodyna-yasm/yasm-test/compare/1.27.0..HEAD) (16)

- [Merge pull request #94 from PRODYNA-YASM/feature/update-components](https://github.com/prodyna-yasm/yasm-test/commit/c29a46b065f1690748c34033b553ced864346c59) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:44:13 +0000 UTC

- [Update all components](https://github.com/prodyna-yasm/yasm-test/commit/78c3aa013ca30191983466c86f58ca04ea205573) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:37:39 +0000 UTC

- [Merge pull request #91 from PRODYNA-YASM/90-check-the-test-first-before-building-the-container](https://github.com/prodyna-yasm/yasm-test/commit/66fa49ec3d4cb424c36db75925eb5629d362185a) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:35:21 +0000 UTC

- [Merge branch 'main' into 90-check-the-test-first-before-building-the-container](https://github.com/prodyna-yasm/yasm-test/commit/6cfc8dd7b77d4b2cbb9100454041f7cc6b03b546) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:29:54 +0000 UTC

- [Merge pull request #93 from PRODYNA-YASM/92-generate-md-file-inside-the-container-and-put-all-artefacts-into-a-mountable-directory](https://github.com/prodyna-yasm/yasm-test/commit/40155bf3ca90ba2b9ea6095a1ebf6d8cae864111) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:29:33 +0000 UTC

- [Merge branch 'main' into 92-generate-md-file-inside-the-container-and-put-all-artefacts-into-a-mountable-directory](https://github.com/prodyna-yasm/yasm-test/commit/b8412aa47232f9a388d04d7422029d0dc66fc20c) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:26:20 +0000 UTC

- [Update all components](https://github.com/prodyna-yasm/yasm-test/commit/0f7b7d192c53b3d01baab53503eb914dac27ea95) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:24:42 +0000 UTC

- [Use Cypress 13.11.0](https://github.com/prodyna-yasm/yasm-test/commit/0c0ca725f3046e6997d27343c35ee101b54ca94f) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:21:13 +0000 UTC

- [Copy results to /github/workspace](https://github.com/prodyna-yasm/yasm-test/commit/a5bc49b224404c8da04c6e51a96b2f38664075a6) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 11:20:17 +0000 UTC

- [Fixed starting the own shell script](https://github.com/prodyna-yasm/yasm-test/commit/14604eee7fa475f7d5939962776e1150da84c5ec) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 10:55:20 +0000 UTC

- [Run own script and write all to /reports](https://github.com/prodyna-yasm/yasm-test/commit/dcb78ac6ec5a131e297caf13b63d6844a0a61010) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 10:11:41 +0000 UTC

- [Merge pull request #60 from PRODYNA-YASM/dependabot/npm_and_yarn/auth0-js-9.26.1](https://github.com/prodyna-yasm/yasm-test/commit/1d14a72d369b101dee838517ddac73eabd1ca9de) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 08:33:15 +0000 UTC

- [First run the tests and only then build the image](https://github.com/prodyna-yasm/yasm-test/commit/d9e32bd0c2e139b3862527049014ffb8d7d7cd22) by [dkrizic](https://github.com/dkrizic) on 2024-06-06 08:30:51 +0000 UTC

- [Fix reference to image](https://github.com/prodyna-yasm/yasm-test/commit/c538f921393cf280a3443e4f768e036c89bf2ec6) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 08:35:59 +0000 UTC

- [Merge branch 'main' of github.com:PRODYNA-YASM/yasm-test](https://github.com/prodyna-yasm/yasm-test/commit/328e986514e5f663059bebf273e5ffa0758488cc) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 08:26:02 +0000 UTC

- [fix pipeline to use version without v in the tag name](https://github.com/prodyna-yasm/yasm-test/commit/47743be07ceecb26a024331474d630a8a865f430) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 08:25:28 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-test/pulls) (2)

- [chore(deps): Bump @azure/msal-node from 2.7.0 to 2.9.1](https://github.com/PRODYNA-YASM/yasm-test/pull/95)

- [Fix/adding and verifying project startdate](https://github.com/PRODYNA-YASM/yasm-test/pull/89)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [Compatible to YASM 1.27](https://github.com/PRODYNA-YASM/yasm-test/releases/tag/1.27.0) on 2024-06-05 08:35:59 +0000 UTC

- [v1.1.4](https://github.com/PRODYNA-YASM/yasm-test/releases/tag/v1.1.4) on 2024-05-31 16:54:48 +0000 UTC

- [v1.1.2](https://github.com/PRODYNA-YASM/yasm-test/releases/tag/v1.1.2) on 2024-05-31 16:20:16 +0000 UTC






## [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) 1.1.0







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




### [Workflows requiring approval](https://github.com/prodyna-yasm/sales-copilot/actions?query=is%3Awaiting) (1)

- [Adjust volume estimation guesstimate!](https://github.com/PRODYNA-YASM/sales-copilot/actions/runs/9003211686) created on 2024-05-08 14:04:41 +0000 UTC





---

Created with :heart: by the GitHub Action [deployment-overview](https://github.com/prodyna/deployment-overview) by [@dkrizic](https://github.com/dkrizic)

