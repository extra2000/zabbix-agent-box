# Changelog

## [3.0.0](https://github.com/extra2000/zabbix-agent-box/compare/v2.1.0...v3.0.0) (2021-03-17)


### ⚠ BREAKING CHANGES

* **submodule:** Deployment has changed to Podman pod only

### Features

* **submodule:** Add [podman-formula v2.2.1](https://github.com/extra2000/podman-formula/releases/tag/v2.2.1) ([840df1a](https://github.com/extra2000/zabbix-agent-box/commit/840df1aea444bfbe5b025626eba970c203d97b65))
* **submodule:** Update `zabbix-agent-formula` to [v3.0.0](https://github.com/extra2000/zabbix-agent-formula/releases/tag/v3.0.0) ([568c39b](https://github.com/extra2000/zabbix-agent-box/commit/568c39bb71c7150b99cc7979266231f6bdaa4596))


### Documentations

* **pillar/zabbix_agent.sls.example:** Add `storage_devices`, `storage_mounts`, and booleans to enable type of checks ([2210c33](https://github.com/extra2000/zabbix-agent-box/commit/2210c33de9cf448e5004dd59468cb868a3db0a5f))

## [2.1.0](https://github.com/extra2000/zabbix-agent-box/compare/v2.0.0...v2.1.0) (2021-03-17)


### Features

* **submodule:** Update `zabbix-agent-formula` to [v2.0.2](https://github.com/extra2000/zabbix-agent-formula/releases/tag/v2.0.2) ([15a33cc](https://github.com/extra2000/zabbix-agent-box/commit/15a33cc1556d714b6bc2b369ea2277d3b3e103d6))


### Fixes

* **/etc/minion:** Using new style for `module.run` ([b69b0b3](https://github.com/extra2000/zabbix-agent-box/commit/b69b0b300ee6eac8d97d1905fc7ccf9b42d95aec))


### Styles

* **pillar/zabbix_agent.sls.example:** Fix double quote placements ([9e4dff7](https://github.com/extra2000/zabbix-agent-box/commit/9e4dff70c1e6fc823ebd3cfa75b5e187369bc92f))

## [2.0.0](https://github.com/extra2000/zabbix-agent-box/compare/v1.0.0...v2.0.0) (2021-03-08)


### ⚠ BREAKING CHANGES

* **pillar/zabbix_agent:** Pillar format for `zabbix_agent.config` have changed.

### Features

* **submodule:** Update `zabbix-agent-formula` to [v2.0.0](https://github.com/extra2000/zabbix-agent-formula/releases/tag/v2.0.0) ([e7bfc12](https://github.com/extra2000/zabbix-agent-box/commit/e7bfc12960137bde2e66e99e594221dbf00ff4c3))


### Fixes

* **pillar/zabbix_agent:** Add different configurations for passive checks and active checks ([8089307](https://github.com/extra2000/zabbix-agent-box/commit/808930793904879c4fe2f51ad55e39dc4ec2855c))

## 1.0.0 (2021-03-05)


### Features

* **salt:** Add implementations for `salt/` states ([1b27465](https://github.com/extra2000/zabbix-agent-box/commit/1b27465301eb76dfab88d80cf8db01d8ec8afb3f))
* **submodule:** Add [zabbix-agent-formula v1.0.0](https://github.com/extra2000/zabbix-agent-formula/releases/tag/v1.0.0) ([a7676df](https://github.com/extra2000/zabbix-agent-box/commit/a7676dfdfa346f413c9c952aca8f3f90103f1a24))
* **vagrant:** Import Vagrant files from [extra2000/zabbix-box v1.1.1](https://github.com/extra2000/zabbix-box/releases/tag/v1.1.1) ([bebd121](https://github.com/extra2000/zabbix-agent-box/commit/bebd12111f866aebc34d243f2fb37d8108ab8de7))


### Continuous Integrations

* Add AppVeyor with `semantic-release` bot ([7145467](https://github.com/extra2000/zabbix-agent-box/commit/714546775a9f1a3a152e8086ad30496d35d6619f))


### Documentations

* **README:** Update `README.md` ([18364ea](https://github.com/extra2000/zabbix-agent-box/commit/18364eabd79e3187850aa19c5bd79e55634bc4e7))
