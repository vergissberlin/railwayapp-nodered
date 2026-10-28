# Changelog

## [0.2.9](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.8...railwayapp-nodered-v0.2.9) (2026-10-28)


### Features

* pre-install @vergissberlin/node-red-contrib-mjml node ([#41](https://github.com/vergissberlin/railwayapp-nodered/issues/41)) ([2a248cf](https://github.com/vergissberlin/railwayapp-nodered/commit/2a248cf10170833da0ffe37358ea5276cb98acc2))

## [0.2.8](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.7...railwayapp-nodered-v0.2.8) (2026-10-28)


### Bug Fixes

* **deps:** update node-red to 5.0.9 and dashboard to 1.34.1, resolve critical audit findings ([d7e7c4a](https://github.com/vergissberlin/railwayapp-nodered/commit/d7e7c4a2440bb47dd6afdbd9a91dbc812fa3697c))
* persist flows in the /data volume instead of the container filesystem ([6760227](https://github.com/vergissberlin/railwayapp-nodered/commit/67602278f7de67e6520df4bbb18b90b56621e5ea))

## [0.2.7](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.6...railwayapp-nodered-v0.2.7) (2026-10-28)


### Bug Fixes

* require Node.js 22.9+ for Node-RED 5 on Railpack ([#37](https://github.com/vergissberlin/railwayapp-nodered/issues/37)) ([226d319](https://github.com/vergissberlin/railwayapp-nodered/commit/226d31990a42db62d54c688ab263db8ee719bc65))


### Documentation

* fix Railway deploy button link and add template forum link ([#35](https://github.com/vergissberlin/railwayapp-nodered/issues/35)) ([7497b87](https://github.com/vergissberlin/railwayapp-nodered/commit/7497b87b805615ebed60888b06770f699ad04f1a))

## [0.2.6](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.5...railwayapp-nodered-v0.2.6) (2026-10-04)


### Bug Fixes

* serve /healthz on the admin app so the Railway healthcheck passes ([b7a20eb](https://github.com/vergissberlin/railwayapp-nodered/commit/b7a20eb74b2f81c993070cc10eadf3a72c42920b))


### Documentation

* add architecture diagram to README ([#31](https://github.com/vergissberlin/railwayapp-nodered/issues/31)) ([fa8ed21](https://github.com/vergissberlin/railwayapp-nodered/commit/fa8ed215f531266b3b0fe8d71ae20f10c50e6cfe))
* refresh shared template footer badges ([756daf6](https://github.com/vergissberlin/railwayapp-nodered/commit/756daf6e8ce45a3b844070c82717aeb795dff94b))


### Chores

* **deps:** bump node-red to v5 ([#14](https://github.com/vergissberlin/railwayapp-nodered/issues/14)) ([effeed7](https://github.com/vergissberlin/railwayapp-nodered/commit/effeed7dfeb532d37bd383ba4e304446c817b86f))
* update shared template footer ([951344e](https://github.com/vergissberlin/railwayapp-nodered/commit/951344e735278f34418e6facf3f5f38f8fe7adc3))
* update shared template footer ([48b9e8f](https://github.com/vergissberlin/railwayapp-nodered/commit/48b9e8f6bf9c9ed144e294d608df49a84b81b8f8))

## [0.2.5](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.4...railwayapp-nodered-v0.2.5) (2026-08-03)


### Bug Fixes

* **deps:** update dependency node-red to v5 ([#13](https://github.com/vergissberlin/railwayapp-nodered/issues/13)) ([c146e50](https://github.com/vergissberlin/railwayapp-nodered/commit/c146e5051f8abccfb4dda11e507b643c69a6a2c7))


### Chores

* **deps:** bump the npm_and_yarn group across 1 directory with 3 updates ([#28](https://github.com/vergissberlin/railwayapp-nodered/issues/28)) ([ab72505](https://github.com/vergissberlin/railwayapp-nodered/commit/ab725052ca50094aee8fab6650affb203c445d02))

## [0.2.4](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.3...railwayapp-nodered-v0.2.4) (2026-08-01)


### Features

* add railway-template.json metadata ([5e8afc8](https://github.com/vergissberlin/railwayapp-nodered/commit/5e8afc80b3827dc1ae2670df050ac5bbc12f6aa9))


### Bug Fixes

* clarify secret handling in .env.example, fix Railway button domain, expand README intro ([#26](https://github.com/vergissberlin/railwayapp-nodered/issues/26)) ([7178392](https://github.com/vergissberlin/railwayapp-nodered/commit/7178392334c08c148e41b282a7b29b56dd51e5f0))
* enforce persistent volume guidance for Railway deploys ([0574c8c](https://github.com/vergissberlin/railwayapp-nodered/commit/0574c8c5aeafc32f4c423abe0531bcf48e48a0cf))
* remove duplicated footer marker and resync badge footer ([#24](https://github.com/vergissberlin/railwayapp-nodered/issues/24)) ([d4cf618](https://github.com/vergissberlin/railwayapp-nodered/commit/d4cf618df66969e856a404661f7ba79527200ea6))


### Documentation

* rename agent.md to AGENTS.md, add conventional commits rule ([#25](https://github.com/vergissberlin/railwayapp-nodered/issues/25)) ([284afce](https://github.com/vergissberlin/railwayapp-nodered/commit/284afce69935b8c1138c7611de76b55d72219167))
* sync template header and cross-repo footer badges ([493673b](https://github.com/vergissberlin/railwayapp-nodered/commit/493673b5bb341b2facf74694b5b26d90a26e5925))
* sync template header and cross-repo footer badges ([ee6b19b](https://github.com/vergissberlin/railwayapp-nodered/commit/ee6b19b5ecf4f24a67f61c212298130e7384d537))
* update footer section in README.md with new badge formatting ([6fa6460](https://github.com/vergissberlin/railwayapp-nodered/commit/6fa6460507496f158a4b2dfb4fff671c6ebd1cae))


### Chores

* **deps:** update dependency node-red to v4.1.11 ([#11](https://github.com/vergissberlin/railwayapp-nodered/issues/11)) ([3c5c8a8](https://github.com/vergissberlin/railwayapp-nodered/commit/3c5c8a88255cd3a7a83261876fe16609c1ee53cc))

## [0.2.3](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.2...railwayapp-nodered-v0.2.3) (2026-03-22)


### Chores

* harden railway runtime defaults ([#8](https://github.com/vergissberlin/railwayapp-nodered/issues/8)) ([5db665e](https://github.com/vergissberlin/railwayapp-nodered/commit/5db665ef8eddc9f24874e8977deab01a28b8d37f))

## [0.2.2](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.1...railwayapp-nodered-v0.2.2) (2026-03-22)


### Bug Fixes

* **deps:** update dependency bcryptjs to v3 ([#4](https://github.com/vergissberlin/railwayapp-nodered/issues/4)) ([b735125](https://github.com/vergissberlin/railwayapp-nodered/commit/b735125f815641175781f392039a1af1747d370f))


### Chores

* migrate dashboard dependency to FlowFuse ([#7](https://github.com/vergissberlin/railwayapp-nodered/issues/7)) ([03c5a4e](https://github.com/vergissberlin/railwayapp-nodered/commit/03c5a4e328922e49c368ebe8798efbc3cfe46d68))

## [0.2.1](https://github.com/vergissberlin/railwayapp-nodered/compare/railwayapp-nodered-v0.2.0...railwayapp-nodered-v0.2.1) (2026-03-22)


### Documentation

* document production setup and release commit conventions ([20d0b8f](https://github.com/vergissberlin/railwayapp-nodered/commit/20d0b8f8f48eea2e549a8e6291d3a773c7c00cb8))


### CI

* trigger releases for docs ci refactor and chore commits ([3b99e6c](https://github.com/vergissberlin/railwayapp-nodered/commit/3b99e6c4cc4c0519f40858a0c7f8ad0ebd9127a9))


### Chores

* align repository with Railway deployment best practices ([396819c](https://github.com/vergissberlin/railwayapp-nodered/commit/396819ca6e0f8f822bc8e669c169f991b361314b))
* upgrade node-red to 4.1.7 ([67e5830](https://github.com/vergissberlin/railwayapp-nodered/commit/67e5830b0b8aa8c67f10cc048eb60ec103e26cda))
