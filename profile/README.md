# YASM Deployment Overview

Component Status overview. Last update 2024-06-06T15:28:22Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :red_square: [10](https://github.com/prodyna-yasm/yasm-backend/compare/1.27.0..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.27.0 |  :red_square: d2b26f1 |  :green_square: 1.27.0 |  :green_square: 1.27.0 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :red_square: [23](https://github.com/prodyna-yasm/yasm-frontend/compare/1.27.1..HEAD) | :yellow_square: [6](https://github.com/prodyna-yasm/yasm-frontend/pulls) | 1.27.1 |  :red_square: 0ca5ab7 |  :green_square: 1.27.1 |  :green_square: 1.27.1 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :red_square: [8](https://github.com/prodyna-yasm/yasm-integration/compare/1.27.1..HEAD) | :green_square: 0 | 1.27.1 |  :red_square: c0c2f15 |  :green_square: 1.27.1 |  :green_square: 1.27.1 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :red_square: [8](https://github.com/prodyna-yasm/yasmctl/compare/1.27.0..HEAD) | :green_square: 0 | 1.27.0 |  :red_square: 1d87661 |  :green_square: 1.27.0 |  :green_square: 1.27.0 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :red_square: [3](https://github.com/prodyna-yasm/yasm-proxy-odbc/compare/1.12.0..HEAD) | :green_square: 0 | 1.12.0 |  :red_square: fdcbfe7 |  :green_square: 1.12.0 |  :green_square: 1.12.0 | 
| [yasm-github](https://github.com/prodyna-yasm/yasm-github) | :red_square: [6](https://github.com/prodyna-yasm/yasm-github/compare/1.4.8..HEAD) | :green_square: 0 | 1.4.8 |  :red_square: 2cf207e |  :green_square: 1.4.8 |  :green_square: 1.4.8 | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :red_square: [4](https://github.com/prodyna-yasm/yasm-geocoding/compare/1.9.12..HEAD) | :green_square: 0 | 1.9.12 |  :red_square: 1eed23f |  :green_square: 1.9.12 |  :green_square: 1.9.12 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :green_square: 0 | :green_square: 0 | 1.26.0 |  :green_square: 1.26.0 |  :green_square: 1.26.0 |  :green_square: 1.26.0 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.5.1-1 |  :green_square: 8.5.1-1 |  :green_square: 8.5.1-1 |  :green_square: 8.5.1-1 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :green_square: 0 | :green_square: 0 | 1.27.1 |  :green_square: 1.27.1 |  :green_square: 1.27.1 |  :green_square: 1.27.1 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :green_square: 0 | :yellow_square: [4](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.28.0 | 
| [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-nginx/pulls) | 1.25.4-2 | 
| [yasm-test](https://github.com/prodyna-yasm/yasm-test) | :red_square: [16](https://github.com/prodyna-yasm/yasm-test/compare/1.27.0..HEAD) | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-test/pulls) | 1.27.0 | 
| [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) | :green_square: 0 | :green_square: 0 | 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 |  :green_square: 1.1.0 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.27.0




### [Commits on main since 1.27.0](https://github.com/prodyna-yasm/yasm-backend/compare/1.27.0..HEAD) (10)

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
| Version |  d2b26f1 |  1.27.0 |  1.27.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Skill importance and extended metrics](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.27.0) on 2024-05-31 12:24:13 +0000 UTC

- [Improve cypher performance and update quarkus](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.2) on 2024-05-24 21:43:36 +0000 UTC

- [Fix skill linking relevant for kindgiver](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.1) on 2024-05-24 09:04:38 +0000 UTC






## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.27.1




### [Commits on main since 1.27.1](https://github.com/prodyna-yasm/yasm-frontend/compare/1.27.1..HEAD) (23)

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

- [Merge pull request #697 from PRODYNA-YASM/dependabot/npm_and_yarn/pmmmwh/react-refresh-webpack-plugin-0.5.15](https://github.com/prodyna-yasm/yasm-frontend/commit/b39ed7fe2bb281e242dedbe33fdea2403332b9ae) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 11:31:25 +0000 UTC

- [Merge pull request #700 from PRODYNA-YASM/699-use-tests-1270](https://github.com/prodyna-yasm/yasm-frontend/commit/3970acd442322309383af85c7ed6f47c91e7a171) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 08:31:04 +0000 UTC

- [Use current tests](https://github.com/prodyna-yasm/yasm-frontend/commit/697ebc3388b105baa6cb81eb6c252b8f031a5af2) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 08:25:08 +0000 UTC

- [refactoring, add charts to employee detail page](https://github.com/prodyna-yasm/yasm-frontend/commit/4fa2235c6c4cbdbbe50826ed641c6fbea1871864) by [](https://github.com/) on 2024-06-04 13:48:54 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-frontend/pulls) (6)

- [Bump chalk from 3.0.0 to 5.3.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/704)

- [added skill tree for parent path](https://github.com/PRODYNA-YASM/yasm-frontend/pull/701)

- [Bump @mui/x-date-pickers from 6.20.0 to 7.6.1](https://github.com/PRODYNA-YASM/yasm-frontend/pull/696)

- [Bump rimraf from 4.4.1 to 5.0.7](https://github.com/PRODYNA-YASM/yasm-frontend/pull/682)

- [Bump memfs from 3.5.3 to 4.9.2](https://github.com/PRODYNA-YASM/yasm-frontend/pull/672)

- [Bump html-loader from 1.3.2 to 5.0.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/619)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  0ca5ab7 |  1.27.1 |  1.27.1 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Fixed update OrganizationForm in Project-View](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.27.1) on 2024-06-04 08:00:16 +0000 UTC

- [Added Skill Importance and added title in Changelog](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.27.0) on 2024-05-31 12:43:30 +0000 UTC

- [Added changelog and upgrade dependencies](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.26.2) on 2024-05-29 08:23:30 +0000 UTC






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.27.1




### [Commits on main since 1.27.1](https://github.com/prodyna-yasm/yasm-integration/compare/1.27.1..HEAD) (8)

- [Merge pull request #436 from PRODYNA-YASM/feature/go-1.22.4](https://github.com/prodyna-yasm/yasm-integration/commit/c0c2f15c264c1877e6a8a1d9886f30535f632b4a) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 13:25:00 +0000 UTC

- [Go 1.22.4](https://github.com/prodyna-yasm/yasm-integration/commit/a2f1dd03ec128fd9a1ffdb8a693dca9de4509edd) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 13:19:09 +0000 UTC

- [Merge pull request #435 from PRODYNA-YASM/feature/yasm-api-1.28](https://github.com/prodyna-yasm/yasm-integration/commit/83349890849c96175286084bb342d4b3934a95b4) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 11:33:56 +0000 UTC

- [Using API 1.28 and some updates](https://github.com/prodyna-yasm/yasm-integration/commit/9ca9208f64b96a06e9d7f72fe384d8f9e764918f) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 11:28:27 +0000 UTC

- [Merge pull request #433 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.27.2](https://github.com/prodyna-yasm/yasm-integration/commit/eb893f20eae8be658ec58863610d48e01019e1bf) by [dkrizic](https://github.com/dkrizic) on 2024-06-04 05:31:47 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.27.0 to 1.27.2](https://github.com/prodyna-yasm/yasm-integration/commit/d7b7045260e6bab40b3fb1ef51da373d5709b95d) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-04 01:11:51 +0000 UTC

- [Merge pull request #432 from PRODYNA-YASM/dependabot/go_modules/github.com/spf13/viper-1.19.0](https://github.com/prodyna-yasm/yasm-integration/commit/a65fcd8b7fa4b5ac6cb1abbb3cac7e7f5e3a97e3) by [dkrizic](https://github.com/dkrizic) on 2024-06-03 07:03:48 +0000 UTC

- [Bump github.com/spf13/viper from 1.18.2 to 1.19.0](https://github.com/prodyna-yasm/yasm-integration/commit/8dcbec8390d8e4f571b92a9a81f72952fbc6c552) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-03 01:28:06 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  c0c2f15 |  1.27.1 |  1.27.1 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Start date for main projects 2022-07-01](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.27.1) on 2024-06-01 09:58:01 +0000 UTC

- [Using API 1.27.0](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.27.0) on 2024-05-31 05:07:45 +0000 UTC

- [Update alpine image](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.26.4) on 2024-05-23 05:35:03 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-integration/actions?query=is%3Awaiting) (6)

- [Merge pull request #427 from PRODYNA-YASM/dependabot/docker/alpine-3.…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9207758718) created on 2024-05-23 12:14:09 +0000 UTC

- [Merge pull request #426 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9189201188) created on 2024-05-22 09:56:06 +0000 UTC

- [Merge pull request #421 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9177468495) created on 2024-05-21 15:44:35 +0000 UTC

- [Merge pull request #419 from PRODYNA-YASM/dependabot/go_modules/googl…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9108351279) created on 2024-05-16 07:35:56 +0000 UTC

- [Merge pull request #418 from PRODYNA-YASM/technology-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9077209401) created on 2024-05-14 09:42:04 +0000 UTC

- [Merge pull request #415 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/8998943989) created on 2024-05-08 08:45:36 +0000 UTC




## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.27.0




### [Commits on main since 1.27.0](https://github.com/prodyna-yasm/yasmctl/compare/1.27.0..HEAD) (8)

- [Merge pull request #331 from PRODYNA-YASM/feature/go-1.22.4](https://github.com/prodyna-yasm/yasmctl/commit/1d876614ff67ff70096df37e422bc7972377ae9f) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 13:22:38 +0000 UTC

- [Go 1.22.4](https://github.com/prodyna-yasm/yasmctl/commit/3bb7aee1d12d020312e551be668fe58a08dbf885) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 13:11:33 +0000 UTC

- [Merge pull request #330 from PRODYNA-YASM/feature/yasm-api-1.28](https://github.com/prodyna-yasm/yasmctl/commit/2a7ba8b7dbf3229f0d0353167207a32c1e06a268) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 11:30:54 +0000 UTC

- [API 1.28, some updates](https://github.com/prodyna-yasm/yasmctl/commit/21132f40142110c414434a17d519d05515c735de) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 11:29:15 +0000 UTC

- [Merge pull request #328 from PRODYNA-YASM/dependabot/go_modules/github.com/spf13/viper-1.19.0](https://github.com/prodyna-yasm/yasmctl/commit/d3972edfaa41af15fc858517310d6116afbc2e7f) by [dkrizic](https://github.com/dkrizic) on 2024-06-03 21:59:44 +0000 UTC

- [Merge pull request #329 from PRODYNA-YASM/dependabot/go_modules/github.com/prodyna-yasm/yasm-api-go-1.27.2](https://github.com/prodyna-yasm/yasmctl/commit/7969d4078e88641d7e7c74e045599e595996c41b) by [dkrizic](https://github.com/dkrizic) on 2024-06-03 21:59:28 +0000 UTC

- [Bump github.com/prodyna-yasm/yasm-api-go from 1.27.0 to 1.27.2](https://github.com/prodyna-yasm/yasmctl/commit/cad978e09b9c2f524b87ec835cd113dc71a766ea) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-03 21:53:51 +0000 UTC

- [Bump github.com/spf13/viper from 1.18.2 to 1.19.0](https://github.com/prodyna-yasm/yasmctl/commit/b5372c962b468eb5224fe9db00a78cdd35df051d) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-03 21:53:46 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1d87661 |  1.27.0 |  1.27.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Using API 1.27.0](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.27.0) on 2024-05-31 21:43:46 +0000 UTC

- [New libraries](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.26.2) on 2024-05-21 22:00:27 +0000 UTC

- [1.26.1](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.26.1) on 2024-05-21 15:41:38 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (4)

- [Merge pull request #324 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9182087461) created on 2024-05-21 22:05:09 +0000 UTC

- [Merge pull request #320 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9177461182) created on 2024-05-21 15:43:57 +0000 UTC

- [Merge pull request #319 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9077198208) created on 2024-05-14 09:41:06 +0000 UTC

- [Merge pull request #318 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8998896608) created on 2024-05-08 08:41:31 +0000 UTC




## [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) 1.12.0




### [Commits on main since 1.12.0](https://github.com/prodyna-yasm/yasm-proxy-odbc/compare/1.12.0..HEAD) (3)

- [Merge pull request #196 from PRODYNA-YASM/feature/default-date-2023-07-01](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/fdcbfe7b67e16b302deb1bc761983cb81d30111b) by [dkrizic](https://github.com/dkrizic) on 2024-06-03 16:38:05 +0000 UTC

- [Merge pull request #197 from PRODYNA-YASM/dependabot/go_modules/github.com/spf13/viper-1.19.0](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/7fa7257212693deda5e089901d2a2b5d7c462e2f) by [dkrizic](https://github.com/dkrizic) on 2024-06-03 13:20:15 +0000 UTC

- [Bump github.com/spf13/viper from 1.18.2 to 1.19.0](https://github.com/prodyna-yasm/yasm-proxy-odbc/commit/741c5f28c1ac374c53c3de29ceb755e228d37125) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-03 13:15:08 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  fdcbfe7 |  1.12.0 |  1.12.0 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Technology update, start date for main projects back to 2023-07-01](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.12.0) on 2024-05-31 14:42:58 +0000 UTC

- [OpenTelemetry 1.27.0](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.9) on 2024-05-27 14:14:44 +0000 UTC

- [1.11.8](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.8) on 2024-05-21 15:38:12 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-proxy-odbc/actions?query=is%3Awaiting) (1)

- [Merge pull request #188 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/actions/runs/9177465100) created on 2024-05-21 15:44:16 +0000 UTC




## [yasm-github](https://github.com/prodyna-yasm/yasm-github) 1.4.8




### [Commits on main since 1.4.8](https://github.com/prodyna-yasm/yasm-github/compare/1.4.8..HEAD) (6)

- [Merge pull request #94 from PRODYNA-YASM/feature/technolgy-update](https://github.com/prodyna-yasm/yasm-github/commit/2cf207ed338a5a4cbc10a4fc192bd09b70db6d99) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 13:22:56 +0000 UTC

- [Current components](https://github.com/prodyna-yasm/yasm-github/commit/5661f816e83bd56ef3edd9344ab947614075eb69) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 13:08:40 +0000 UTC

- [Merge pull request #93 from PRODYNA-YASM/dependabot/docker/golang-1.22.4-alpine3.19](https://github.com/prodyna-yasm/yasm-github/commit/f29a32a9a0d3737b121fd18f15c7004147b4da9c) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 06:34:55 +0000 UTC

- [Bump golang from 1.22.3-alpine3.19 to 1.22.4-alpine3.19](https://github.com/prodyna-yasm/yasm-github/commit/f8cda83b7b6f342e1e1954b2c0600cd63811a25a) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-04 23:49:49 +0000 UTC

- [Merge pull request #92 from PRODYNA-YASM/dependabot/go_modules/golang.org/x/oauth2-0.21.0](https://github.com/prodyna-yasm/yasm-github/commit/3400c31aeb34a98a9c236980021209f529e67efa) by [dkrizic](https://github.com/dkrizic) on 2024-06-04 23:20:36 +0000 UTC

- [Bump golang.org/x/oauth2 from 0.20.0 to 0.21.0](https://github.com/prodyna-yasm/yasm-github/commit/380da8c4f22d9f6efa7fa5862a26cfdf5ddd2723) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-04 23:09:33 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  2cf207e |  1.4.8 |  1.4.8 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Improved error handling](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.8) on 2024-05-28 14:28:02 +0000 UTC

- [OpenTelemetry 1.27](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.7) on 2024-05-22 09:50:59 +0000 UTC

- [1.4.6](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.6) on 2024-05-21 15:39:11 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-github/actions?query=is%3Awaiting) (1)

- [Merge pull request #82 from PRODYNA-YASM/81-dummy-issue](https://github.com/PRODYNA-YASM/yasm-github/actions/runs/9173421502) created on 2024-05-21 10:50:14 +0000 UTC




## [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) 1.9.12




### [Commits on main since 1.9.12](https://github.com/prodyna-yasm/yasm-geocoding/compare/1.9.12..HEAD) (4)

- [Merge pull request #119 from PRODYNA-YASM/dependabot/docker/golang-1.22.4](https://github.com/prodyna-yasm/yasm-geocoding/commit/1eed23f09186e89d0ca0a5a72dcf1672fda609aa) by [dkrizic](https://github.com/dkrizic) on 2024-06-05 17:15:09 +0000 UTC

- [Bump golang from 1.22.3 to 1.22.4](https://github.com/prodyna-yasm/yasm-geocoding/commit/5b3c27b9405978e38de4cceffcc5bf8b013a11b0) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-05 16:50:07 +0000 UTC

- [Merge pull request #118 from PRODYNA-YASM/dependabot/go_modules/github.com/spf13/viper-1.19.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/eca159d4fc174920e8f292f6140cf4c3dba0e01b) by [dkrizic](https://github.com/dkrizic) on 2024-06-03 16:32:24 +0000 UTC

- [Bump github.com/spf13/viper from 1.18.2 to 1.19.0](https://github.com/prodyna-yasm/yasm-geocoding/commit/335a3c68976447b979ed1ccfc25d1b74ee0c7d6c) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-06-03 16:26:38 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1eed23f |  1.9.12 |  1.9.12 | 
| Release |  :red_square: |  :green_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: |  :green_square: | 


### Last releases

- [Alpine 3.20](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.12) on 2024-05-23 17:16:53 +0000 UTC

- [OpenTelemetry 1.27](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.9.11) on 2024-05-22 18:13:49 +0000 UTC

- [1.6.10](https://github.com/PRODYNA-YASM/yasm-geocoding/releases/tag/1.6.10) on 2024-05-21 15:39:34 +0000 UTC




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






## [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) 8.5.1-1







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  8.5.1-1 |  8.5.1-1 |  8.5.1-1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Gotenberg 8.5.1](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.5.1-1) on 2024-05-27 05:13:43 +0000 UTC

- [Gotenberg 8.5.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.5.0-1) on 2024-04-29 06:09:42 +0000 UTC

- [Gotenberg 8.4.0](https://github.com/PRODYNA-YASM/yasm-gotenberg/releases/tag/8.4.0-1) on 2024-04-15 05:40:41 +0000 UTC






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






## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.28.0






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-api/pulls) (4)

- [add anonymize flag in pdf-profile, removed githubUser and  removed ol…](https://github.com/PRODYNA-YASM/yasm-api/pull/201)

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

- [Team member in person detail](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.28.0) on 2024-06-05 08:26:56 +0000 UTC

- [Fix Naming](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.27.2) on 2024-06-03 16:33:43 +0000 UTC

- [New PdfProfile Endpoint](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.27.1) on 2024-06-03 16:23:51 +0000 UTC






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

