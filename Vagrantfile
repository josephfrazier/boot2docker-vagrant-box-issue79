Vagrant.configure(2) do |config|
  config.vm.provider "docker" do |d|
    d.build_dir = "."
    d.remains_running = false
  end
  # https://github.com/mitchellh/boot2docker-vagrant-box/issues/79#issuecomment-167066247
  config.ssh.insert_key = true
  config.ssh.username = 'docker'
  config.ssh.password = 'tcuser'
  config.ssh.guest_port = 2222
  config.ssh.port = 22
  config.ssh.host = '127.0.0.1'
end
