# vagrant-coreos


`/home/core/**` synced local directory
```
      config.vm.synced_folder(
        "../",
        "/home/core/#{File.basename(File.dirname(Dir.pwd))}",
        id: "core",
        :nfs => true,
        :mount_options => ['nolock,vers=3,udp'],
      )
```
