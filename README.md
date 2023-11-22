# Mdadm home work
Собранная сборка Linux для первого ДЗ

Ссылка на сборку(box): 
https://app.vagrantup.com/ruselbbc/boxes/kernelCentOs8

Готовый Vagrant файл в репозитории.

Для создания сборки по умолчанию в Vagrant:
Vagrant.configure("2") do |config|
  config.vm.box = "ruselbbc/kernelCentOs8"
  config.vm.box_version = "0"
end
