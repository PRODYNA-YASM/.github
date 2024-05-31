# YASM Deployment Overview

Component Status overview. Last update 2024-05-31T11:12:12Z

| Repository | Commits | PRs | Latest Release |  [dev](https://dev-yasm.prodyna.com) |  [staging](https://staging-yasm.prodyna.com) |  [prod](https://yasm.prodyna.com) | 
| --- | --- | --- | -- |  --- |  --- |  --- | 
| [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) | :red_square: [6](https://github.com/prodyna-yasm/yasm-backend/compare/1.26.2..HEAD) | :yellow_square: [1](https://github.com/prodyna-yasm/yasm-backend/pulls) | 1.26.2 |  :red_square: 0c7b316 |  :green_square: 1.26.2 | 
| [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) | :red_square: [9](https://github.com/prodyna-yasm/yasm-frontend/compare/1.26.2..HEAD) | :yellow_square: [8](https://github.com/prodyna-yasm/yasm-frontend/pulls) | 1.26.2 |  :red_square: 9230ff8 |  :green_square: 1.26.2 | 
| [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) | :red_square: [2](https://github.com/prodyna-yasm/yasm-integration/compare/1.26.4..HEAD) | :green_square: 0 | 1.26.4 |  :red_square: 0420dce |  :green_square: 1.26.4 | 
| [yasmctl](https://github.com/prodyna-yasm/yasmctl) | :green_square: 0 | :green_square: 0 | 1.26.2 |  :green_square: 1.26.2 |  :green_square: 1.26.2 |  :red_square: 1.19.6 | 
| [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) | :green_square: 0 | :green_square: 0 | 1.11.9 |  :green_square: 1.11.9 |  :green_square: 1.11.9 |  :green_square: 1.11.9 | 
| [yasm-github](https://github.com/prodyna-yasm/yasm-github) | :green_square: 0 | :green_square: 0 | 1.4.8 |  :green_square: 1.4.8 |  :green_square: 1.4.8 |  :red_square: 1.4.7 | 
| [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) | :green_square: 0 | :green_square: 0 | 1.9.12 |  :green_square: 1.9.12 |  :green_square: 1.9.12 |  :green_square: 1.9.12 | 
| [yasm-data](https://github.com/prodyna-yasm/yasm-data) | :green_square: 0 | :green_square: 0 | 1.26.0 |  :green_square: 1.26.0 |  :green_square: 1.26.0 |  :red_square: 1.10.2 | 
| [yasm-gotenberg](https://github.com/prodyna-yasm/yasm-gotenberg) | :green_square: 0 | :green_square: 0 | 8.5.1-1 |  :green_square: 8.5.1-1 |  :green_square: 8.5.1-1 |  :green_square: 8.5.1-1 | 
| [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-infrastructure-staged/pulls) | 1.26.2 |  :green_square: 1.26.2 |  :green_square: 1.26.2 |  :green_square: 1.26.2 | 
| [yasm-api](https://github.com/prodyna-yasm/yasm-api) | :green_square: 0 | :yellow_square: [7](https://github.com/prodyna-yasm/yasm-api/pulls) | 1.26.0 | 
| [yasm-nginx](https://github.com/prodyna-yasm/yasm-nginx) | :green_square: 0 | :yellow_square: [2](https://github.com/prodyna-yasm/yasm-nginx/pulls) | 1.25.4-2 | 
| [yasm-test](https://github.com/prodyna-yasm/yasm-test) | :red_square: [30](https://github.com/prodyna-yasm/yasm-test/compare/..HEAD) | :yellow_square: [6](https://github.com/prodyna-yasm/yasm-test/pulls) |  | 
| [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) | :red_square: [1](https://github.com/prodyna-yasm/sales-copilot/compare/1.0.1..HEAD) | :green_square: 0 | 1.0.1 |  :green_square: 1.0.1 |  :green_square: 1.0.1 |  :green_square: 1.0.1 | 



## [yasm-backend](https://github.com/prodyna-yasm/yasm-backend) 1.26.2




### [Commits on main since 1.26.2](https://github.com/prodyna-yasm/yasm-backend/compare/1.26.2..HEAD) (6)

- [Merge pull request #623 from PRODYNA-YASM/622-maxunavailable=1](https://github.com/prodyna-yasm/yasm-backend/commit/0c7b316afb8d040c81d3aef6029f9442311cb6d8) by [dkrizic](https://github.com/dkrizic) on 2024-05-31 09:36:18 +0000 UTC

- [maxUnavailable and maxSurge=1](https://github.com/prodyna-yasm/yasm-backend/commit/112e3313395cefdcad2d83d42323ca710b511535) by [dkrizic](https://github.com/dkrizic) on 2024-05-31 09:27:01 +0000 UTC

- [update quarkus (#621)](https://github.com/prodyna-yasm/yasm-backend/commit/e26f0fca2529477e41ed607302d7e3f4d4c6564e) by [coding4kay](https://github.com/coding4kay) on 2024-05-31 09:24:47 +0000 UTC

- [fix: preventing errors when creating metrics (#619)](https://github.com/prodyna-yasm/yasm-backend/commit/f4bb34c4b8fac9b4b42858712815a162e2644944) by [saemik94](https://github.com/saemik94) on 2024-05-30 13:37:03 +0000 UTC

- [fix: adjust skill search metric (#618)](https://github.com/prodyna-yasm/yasm-backend/commit/82694901efa8615f845ae2b9fc2a96fa182f6221) by [saemik94](https://github.com/saemik94) on 2024-05-30 12:31:12 +0000 UTC

- [feat: extend search metrics (#616)](https://github.com/prodyna-yasm/yasm-backend/commit/fc240ec01b1bf9c1cd4ac8b3e1a5f7e5dae9fa9d) by [saemik94](https://github.com/saemik94) on 2024-05-30 08:30:20 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-backend/pulls) (1)

- [Bump eclipse-temurin from 21.0.2_13-jre-ubi9-minimal to 22.0.1_8-jre-ubi9-minimal](https://github.com/PRODYNA-YASM/yasm-backend/pull/588)



### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  0c7b316 |  1.26.2 | 
| Release |  :red_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: | 


### Last releases

- [Improve cypher performance and update quarkus](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.2) on 2024-05-24 21:43:36 +0000 UTC

- [Fix skill linking relevant for kindgiver](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.1) on 2024-05-24 09:04:38 +0000 UTC

- [Sort people avatar in project, clean skill api and add search metrics](https://github.com/PRODYNA-YASM/yasm-backend/releases/tag/1.26.0) on 2024-05-14 12:53:08 +0000 UTC






## [yasm-frontend](https://github.com/prodyna-yasm/yasm-frontend) 1.26.2




### [Commits on main since 1.26.2](https://github.com/prodyna-yasm/yasm-frontend/compare/1.26.2..HEAD) (9)

- [Merge pull request #690 from PRODYNA-YASM/688-maxsurge-and-maxunavailable-=-1](https://github.com/prodyna-yasm/yasm-frontend/commit/9230ff82df673787c70c91aa91c5baa84a348306) by [dkrizic](https://github.com/dkrizic) on 2024-05-31 09:32:39 +0000 UTC

- [maxSurge = 1, maxUnavailable = 1](https://github.com/prodyna-yasm/yasm-frontend/commit/ed61a98da476c2fa4c68e4e6dcf88155e6bbaf7f) by [dkrizic](https://github.com/dkrizic) on 2024-05-31 09:29:09 +0000 UTC

- [Merge pull request #680 from PRODYNA-YASM/dependabot/npm_and_yarn/opentelemetry/instrumentation-user-interaction-0.38.0](https://github.com/prodyna-yasm/yasm-frontend/commit/cae388560c3dcf346386c1ac55baced450b429fb) by [dkrizic](https://github.com/dkrizic) on 2024-05-30 19:25:45 +0000 UTC

- [Bump @opentelemetry/instrumentation-user-interaction](https://github.com/prodyna-yasm/yasm-frontend/commit/7199d27e99c59cbc625e29b0c8933931b34dd606) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-05-30 04:56:00 +0000 UTC

- [Merge pull request #677 from PRODYNA-YASM/feature/add-release-title-changelog](https://github.com/prodyna-yasm/yasm-frontend/commit/24429217e4d71560c0bf7bc2ca827b6cc3a3eca7) by [dkrizic](https://github.com/dkrizic) on 2024-05-29 14:10:53 +0000 UTC

- [250: Added Release-Title in Changelog](https://github.com/prodyna-yasm/yasm-frontend/commit/9298b56c6fea4c3ce95b2177adcc17c15dd3377b) by [eersada-prodyna](https://github.com/eersada-prodyna) on 2024-05-29 14:05:37 +0000 UTC

- [Merge pull request #676 from PRODYNA-YASM/675-bug-changelog-also-for-tags](https://github.com/prodyna-yasm/yasm-frontend/commit/4c74a6b97b08716236be9d8af8bb24b54d29eb66) by [dkrizic](https://github.com/dkrizic) on 2024-05-29 13:18:11 +0000 UTC

- [Fix tags on main](https://github.com/prodyna-yasm/yasm-frontend/commit/aa3ea677e61bf2ca170f10fe0e04e41731aa60d2) by [dkrizic](https://github.com/dkrizic) on 2024-05-29 13:16:42 +0000 UTC

- [Changelog should run on tags as well](https://github.com/prodyna-yasm/yasm-frontend/commit/bb553de7f16795f8a2ca957f628e8832595f9564) by [dkrizic](https://github.com/dkrizic) on 2024-05-29 13:14:20 +0000 UTC




### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-frontend/pulls) (8)

- [hide parentPath in SkillDetailView and fixed Organization-Create-Form](https://github.com/PRODYNA-YASM/yasm-frontend/pull/687)

- [Bump @types/node from 20.12.12 to 20.12.13](https://github.com/PRODYNA-YASM/yasm-frontend/pull/684)

- [Feature/refactor async select](https://github.com/PRODYNA-YASM/yasm-frontend/pull/683)

- [Bump rimraf from 4.4.1 to 5.0.7](https://github.com/PRODYNA-YASM/yasm-frontend/pull/682)

- [Bump @babel/register from 7.23.7 to 7.24.6](https://github.com/PRODYNA-YASM/yasm-frontend/pull/681)

- [Base structure for testing](https://github.com/PRODYNA-YASM/yasm-frontend/pull/679)

- [Bump memfs from 3.5.3 to 4.9.2](https://github.com/PRODYNA-YASM/yasm-frontend/pull/672)

- [Bump html-loader from 1.3.2 to 5.0.0](https://github.com/PRODYNA-YASM/yasm-frontend/pull/619)



### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  9230ff8 |  1.26.2 | 
| Release |  :red_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: | 


### Last releases

- [Added changelog and upgrade dependencies](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.26.2) on 2024-05-29 08:23:30 +0000 UTC

- [Added Skill Parent Path (Kindgiver), add check if user has GitHub access, and multiple bug fixes](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.26.1) on 2024-05-24 10:35:49 +0000 UTC

- [Added detail-view for Organizations, Industries, Certifications and Skills](https://github.com/PRODYNA-YASM/yasm-frontend/releases/tag/1.26.0) on 2024-05-16 11:59:35 +0000 UTC






## [yasm-integration](https://github.com/prodyna-yasm/yasm-integration) 1.26.4




### [Commits on main since 1.26.4](https://github.com/prodyna-yasm/yasm-integration/compare/1.26.4..HEAD) (2)

- [Merge pull request #428 from PRODYNA-YASM/dependabot/go_modules/github.com/microsoftgraph/msgraph-sdk-go-1.44.0](https://github.com/prodyna-yasm/yasm-integration/commit/0420dce37a8f6f077a9274fbd98d21ac6450cabd) by [dkrizic](https://github.com/dkrizic) on 2024-05-31 05:07:45 +0000 UTC

- [Bump github.com/microsoftgraph/msgraph-sdk-go from 1.43.0 to 1.44.0](https://github.com/prodyna-yasm/yasm-integration/commit/81493ba563550aa298b2b524582f6a16c1870157) by [dependabot[bot]](https://github.com/dependabot[bot]) on 2024-05-31 02:00:55 +0000 UTC





### Environments

| Environment |  dev |  staging | 
| --- |  --- |  --- | 
| Version |  0420dce |  1.26.4 | 
| Release |  :red_square: |  :green_square: | 
| Current |  :red_square: |  :green_square: | 


### Last releases

- [Update alpine image](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.26.4) on 2024-05-23 05:35:03 +0000 UTC

- [OpenTelemetry 1.27](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.26.3) on 2024-05-22 09:50:41 +0000 UTC

- [1.26.2](https://github.com/PRODYNA-YASM/yasm-integration/releases/tag/1.26.2) on 2024-05-21 15:38:28 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-integration/actions?query=is%3Awaiting) (8)

- [Merge pull request #427 from PRODYNA-YASM/dependabot/docker/alpine-3.…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9207758718) created on 2024-05-23 12:14:09 +0000 UTC

- [Merge pull request #426 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9189201188) created on 2024-05-22 09:56:06 +0000 UTC

- [Merge pull request #421 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9177468495) created on 2024-05-21 15:44:35 +0000 UTC

- [Merge pull request #419 from PRODYNA-YASM/dependabot/go_modules/googl…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9108351279) created on 2024-05-16 07:35:56 +0000 UTC

- [Merge pull request #418 from PRODYNA-YASM/technology-update](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/9077209401) created on 2024-05-14 09:42:04 +0000 UTC

- [Merge pull request #415 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/8998943989) created on 2024-05-08 08:45:36 +0000 UTC

- [Merge pull request #414 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/8981989926) created on 2024-05-07 08:15:33 +0000 UTC

- [Merge pull request #413 from PRODYNA-YASM/412-migrate-to-api-123](https://github.com/PRODYNA-YASM/yasm-integration/actions/runs/8965688522) created on 2024-05-06 07:39:36 +0000 UTC




## [yasmctl](https://github.com/prodyna-yasm/yasmctl) 1.26.2







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.26.2 |  1.26.2 |  1.19.6 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [New libraries](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.26.2) on 2024-05-21 22:00:27 +0000 UTC

- [1.26.1](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.26.1) on 2024-05-21 15:41:38 +0000 UTC

- [Using API 1.26.0](https://github.com/PRODYNA-YASM/yasmctl/releases/tag/1.26.0) on 2024-05-14 00:18:12 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasmctl/actions?query=is%3Awaiting) (6)

- [Merge pull request #324 from PRODYNA-YASM/dependabot/go_modules/go.op…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9182087461) created on 2024-05-21 22:05:09 +0000 UTC

- [Merge pull request #320 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9177461182) created on 2024-05-21 15:43:57 +0000 UTC

- [Merge pull request #319 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/9077198208) created on 2024-05-14 09:41:06 +0000 UTC

- [Merge pull request #318 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8998896608) created on 2024-05-08 08:41:31 +0000 UTC

- [Merge pull request #317 from PRODYNA-YASM/dependabot/go_modules/githu…](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8981999058) created on 2024-05-07 08:16:13 +0000 UTC

- [Merge pull request #316 from PRODYNA-YASM/315-migrate-to-api-123](https://github.com/PRODYNA-YASM/yasmctl/actions/runs/8965684044) created on 2024-05-06 07:39:04 +0000 UTC




## [yasm-proxy-odbc](https://github.com/prodyna-yasm/yasm-proxy-odbc) 1.11.9







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.11.9 |  1.11.9 |  1.11.9 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [OpenTelemetry 1.27.0](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.9) on 2024-05-27 14:14:44 +0000 UTC

- [1.11.8](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.8) on 2024-05-21 15:38:12 +0000 UTC

- [OTelChi 0.8.0](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/releases/tag/1.11.7) on 2024-05-06 13:08:14 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-proxy-odbc/actions?query=is%3Awaiting) (1)

- [Merge pull request #188 from PRODYNA-YASM/feature/technolgy-update](https://github.com/PRODYNA-YASM/yasm-proxy-odbc/actions/runs/9177465100) created on 2024-05-21 15:44:16 +0000 UTC




## [yasm-github](https://github.com/prodyna-yasm/yasm-github) 1.4.8







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.4.8 |  1.4.8 |  1.4.7 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [Improved error handling](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.8) on 2024-05-28 14:28:02 +0000 UTC

- [OpenTelemetry 1.27](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.7) on 2024-05-22 09:50:59 +0000 UTC

- [1.4.6](https://github.com/PRODYNA-YASM/yasm-github/releases/tag/1.4.6) on 2024-05-21 15:39:11 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-github/actions?query=is%3Awaiting) (2)

- [Merge pull request #90 from PRODYNA-YASM/89-correct-error-handling](https://github.com/PRODYNA-YASM/yasm-github/actions/runs/9300804735) created on 2024-05-30 10:10:34 +0000 UTC

- [Merge pull request #82 from PRODYNA-YASM/81-dummy-issue](https://github.com/PRODYNA-YASM/yasm-github/actions/runs/9173421502) created on 2024-05-21 10:50:14 +0000 UTC




## [yasm-geocoding](https://github.com/prodyna-yasm/yasm-geocoding) 1.9.12







### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.9.12 |  1.9.12 |  1.9.12 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


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
| Version |  1.26.0 |  1.26.0 |  1.10.2 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :red_square: | 


### Last releases

- [Add some roles](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.26.0) on 2024-04-29 06:13:23 +0000 UTC

- [New roles](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.2) on 2024-04-29 06:13:23 +0000 UTC

- [Main branch](https://github.com/PRODYNA-YASM/yasm-data/releases/tag/1.10.1) on 2024-04-19 13:36:35 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-data/actions?query=is%3Awaiting) (1)

- [Merge pull request #116 from PRODYNA-YASM/115-add-ai-engineer-data-sc…](https://github.com/PRODYNA-YASM/yasm-data/actions/runs/9257652491) created on 2024-05-27 16:05:14 +0000 UTC




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






## [yasm-infrastructure-staged](https://github.com/prodyna-yasm/yasm-infrastructure-staged) 1.26.2






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-infrastructure-staged/pulls) (2)

- [Bump azurerm from 3.104.2 to 3.106.0 in /terraform/kubernetes](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/pull/520)

- [Bump azurerm from 3.104.2 to 3.105.0 in /terraform/azure](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/pull/519)



### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.26.2 |  1.26.2 |  1.26.2 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [Otel Collector 0.92](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.26.2) on 2024-05-22 11:53:37 +0000 UTC

- [Compactor memory](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.26.1) on 2024-05-14 13:49:34 +0000 UTC

- [Component updates, preparation for Apps 1.26](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/releases/tag/1.26.0) on 2024-05-14 12:44:07 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/yasm-infrastructure-staged/actions?query=is%3Awaiting) (1)

- [Merge pull request #485 from PRODYNA-YASM/feature/update-kubernetes-1…](https://github.com/PRODYNA-YASM/yasm-infrastructure-staged/actions/runs/8983687209) created on 2024-05-07 10:20:55 +0000 UTC




## [yasm-api](https://github.com/prodyna-yasm/yasm-api) 1.26.0






### [Open Pull Requests](https://github.com/prodyna-yasm/yasm-api/pulls) (7)

- [Feature/324-project-images](https://github.com/PRODYNA-YASM/yasm-api/pull/194)

- [Bump io.swagger.codegen.v3:swagger-codegen-maven-plugin from 3.0.55 to 3.0.57](https://github.com/PRODYNA-YASM/yasm-api/pull/193)

- [Bump jakarta.validation:jakarta.validation-api from 3.0.2 to 3.1.0](https://github.com/PRODYNA-YASM/yasm-api/pull/191)

- [Bump org.openapitools:openapi-generator-maven-plugin from 7.5.0 to 7.6.0](https://github.com/PRODYNA-YASM/yasm-api/pull/190)

- [Bump com.fasterxml.jackson.core:jackson-databind from 2.17.0 to 2.17.1](https://github.com/PRODYNA-YASM/yasm-api/pull/184)

- [Bump jakarta.ws.rs:jakarta.ws.rs-api from 3.1.0 to 4.0.0](https://github.com/PRODYNA-YASM/yasm-api/pull/180)

- [Draft: Skill kind giver refactoring](https://github.com/PRODYNA-YASM/yasm-api/pull/105)



### Environments

| Environment | 
| --- | 
| Version | 
| Release | 
| Current | 


### Last releases

- [Skill API KindGiver](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.26.0) on 2024-05-13 14:21:44 +0000 UTC

- [Skill Search and Clean api from suggestable and linkable](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.25.0) on 2024-05-07 11:54:45 +0000 UTC

- [Add Industry Search](https://github.com/PRODYNA-YASM/yasm-api/releases/tag/1.24.0) on 2024-05-06 14:47:35 +0000 UTC






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






## [yasm-test](https://github.com/prodyna-yasm/yasm-test) 


> [!WARNING]
> GET https://api.github.com/repos/prodyna-yasm/yasm-test/releases/latest: 404 Not Found []


## [sales-copilot](https://github.com/prodyna-yasm/sales-copilot) 1.0.1




### [Commits on main since 1.0.1](https://github.com/prodyna-yasm/sales-copilot/compare/1.0.1..HEAD) (1)

- [Change QR-Code Ref Header!](https://github.com/prodyna-yasm/sales-copilot/commit/9ed01244d543b171dc27ebeacdbda2485d2c44e6) by [](https://github.com/) on 2024-05-24 09:13:26 +0000 UTC





### Environments

| Environment |  dev |  staging |  prod | 
| --- |  --- |  --- |  --- | 
| Version |  1.0.1 |  1.0.1 |  1.0.1 | 
| Release |  :green_square: |  :green_square: |  :green_square: | 
| Current |  :green_square: |  :green_square: |  :green_square: | 


### Last releases

- [1.0.1 Formatting and Crash Fixes](https://github.com/PRODYNA-YASM/sales-copilot/releases/tag/1.0.1) on 2024-05-24 08:34:42 +0000 UTC

- [Version 1.0.0](https://github.com/PRODYNA-YASM/sales-copilot/releases/tag/1.0.0) on 2024-05-14 11:34:42 +0000 UTC




### [Workflows requiring approval](https://github.com/prodyna-yasm/sales-copilot/actions?query=is%3Awaiting) (2)

- [Adjust volume estimation guesstimate!](https://github.com/PRODYNA-YASM/sales-copilot/actions/runs/9003211686) created on 2024-05-08 14:04:41 +0000 UTC

- [Add an estimate for consultant days! Needs empiric testing!](https://github.com/PRODYNA-YASM/sales-copilot/actions/runs/8982656227) created on 2024-05-07 09:04:34 +0000 UTC





---

Created with :heart: by the GitHub Action [deployment-overview](https://github.com/prodyna/deployment-overview) by [@dkrizic](https://github.com/dkrizic)

