# Repositories for self created deb packages

open-vm-tools for arm64 (focal hirsute)

## add gpg key
wget -q -O - http://dharenkamp.github.io/repositories/ubuntu/gpg | apt-key add -

## create sources list
echo "deb http://dharenkamp.github.io/repositories/ubuntu/ $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/open-vm-tools.list > /dev/null

