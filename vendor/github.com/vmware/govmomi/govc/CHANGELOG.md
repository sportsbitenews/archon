# changelog

### 0.8.0 (2016-06-30)

* If username (`-u` / GOVC_USERNAME) is empty, attempt login via local ticket (Workstation)

* Add StoragePod support to govc folder.create

* Add `-folder` flag to datacenter.create command

* Logout when session persistence is disabled

* Add `-L` flag to ls command for resolving by managed object reference

* Add `-i` flag to ls command for listing the managed object reference

* Add vm.markasvm command

* Add vm.markastemplate command

### 0.7.1 (2016-06-03)

* Fix datastore.{upload,download} against VirtualCenter

### 0.7.0 (2016-06-02)

* Add `-require` flag to version command

* Add support for local type in the datastore.create command

* Add `-namespace` option to datastore.mkdir and datastore.rm to create/remove namespaces on VSANs

* Add host.service command

* Add host.storage.mark command

* Add `-rescan` option to host.storage.info command

### 0.6.0 (2016-04-29)

* Add folder commands: info, create, destroy, rename, moveinto

* Add datastore.info command

* Add `-a` and `-v4` flags to vm.ip command

* Add host.account.{create,update,remove} commands

* Add env command

* Add vm.clone command

### 0.5.0 (2016-03-30)

* Add dvs.portgroup.info command

* Add `-folder` flag to vm.create command

* Add `-dump` flag to OutputFlag

* Add `-f` flag to events command

* Add `-mode` flag to vm.disk.create command

* Add `-net` flag to device.info command

* Add `-eager` and `-thick` options to vm.create command

### 0.4.0 (2016-02-26)

* Add support for placement in datastore cluster to vm.create command

* Add support for creating new disks in vm.create command

* Add `-p` and `-a` options to govc datastore.ls command

### 0.3.0 (2016-01-16)

* Add permissions.{ls,set,remove} commands

* Add datastore.{create,remove} commands.
  The new create command supports both creating NAS and VMFS datastores.

* Add dvs.{create,add} and dvs.portgroup.add commands

* Add host.vnic.{service,info} commands

* Add cluster.{create,change,add} commands

* Add host.{disconnect,reconnect,remove,maintenance.enter,maintenance.exit} commands

* Add license.decode, license.assigned.list and license.assign commands

* Add firewall.ruleset.find command

* Add logs, logs.ls and logs.download commands

* Add support for LoginExtensionByCertificate with new `-cert` and `-key` flags

* Add govc extension.{info,register,unregister,setcert} commands

* Add govc vapp.{info,destroy,power} commands

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