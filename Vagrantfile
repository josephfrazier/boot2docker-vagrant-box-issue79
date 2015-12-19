Vagrant.configure(2) do |config|
  config.vm.provider "docker" do |d|
    d.build_dir = "."
    d.remains_running = false
  end
  # https://github.com/mitchellh/boot2docker-vagrant-box/issues/79#issuecomment-70225360
  config.ssh.username = 'docker'
  config.ssh.password = 'tcuser'
end
