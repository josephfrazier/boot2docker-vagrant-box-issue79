Attempt a minimal reproduction of https://github.com/mitchellh/boot2docker-vagrant-box/issues/79

At each commit in this repo, run the following

    vagrant version
    sw_vers
    vagrant global-status | grep -E "docker-host|$PWD" | tee /dev/stderr | cut -d ' ' -f 1 | xargs -t vagrant destroy -f && git checkout head^ && vagrant up
