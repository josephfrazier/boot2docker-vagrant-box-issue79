Vagrant.configure(2) do |config|
  config.vm.provider "docker" do |d|
    d.build_dir = "."
    d.remains_running = false
  end
  config.vm.synced_folder ".", "/vagrant", disabled: true
end
