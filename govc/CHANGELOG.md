# changelog

### (unreleased)

* Add cluster.{create,change,add} commands

* Add host.{disconnect,reconnect,remove,maintenance.enter,maintenance.exit} commands

* Add license.decode, license.assigned.list and license.assign commands

* Add firewall.ruleset.find command

* Add logs, logs.ls and logs.download commands

* Add support for LoginExtensionByCertificate with new `-cert` and `-key` flags

* Add govc extension.{info,register,unregister,setcert} commands

* Add govc vapp.{info,destroy,power} commands

...

### 0.2.0 (2015-09-15)

* The `vm.power` guest `-s` and `-r` options will fallback to hard `-off` / `-reset` if tools is unavailable and `-force` flag is given

* Add `PowerOn, InjectOvfEnv, WaitForIP` options to `import.ovf` and `import.ova` option spec file

* Add `import.spec` to produce an example json document

* Add `-options` to `import.ovf` and `import.ova`

* Add `-folder` to `import.ovf` and `import.ova`

* Add `fields` command to manage custom fields

* Add `datastore.info` command

* Add `events` command

* Add `-net.address` (Hardware Address) option to `vm.change` and `vm.create`

* Add `host.add` command to add host to datacenter.

* Add `GOVC_USERNAME` and `GOVC_PASSWORD` to allow overriding username and/or
  password (used when they contain special characters that prevent them from
  being embedded in the URL).

* Add `-e' (ExtraConfig) option to `vm.change` and `vm.info`

* Retry twice on temporary network errors.

* Add `host.autostart` commands to manage VM autostart.

* Add `-persist-session` flag to control whether or not the session is
  persisted to disk (defaults to true).

### 0.1.0 (2015-03-17)

Prior to this version the changes to govc's command set were not documented.
