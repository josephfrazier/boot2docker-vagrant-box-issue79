Attempt a minimal reproduction of https://github.com/mitchellh/boot2docker-vagrant-box/issues/79

At each commit in this repo, run the following

    vagrant version
    sw_vers
    vagrant destroy -f && vagrant up
