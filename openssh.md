### Secure OpenSSH server
Linux & OpenSSH

Config file: /etc/ssh/sshd_config

#### Use SSH public key for login (>=2048 bits)
    PubkeyAuthentication yes
    PasswordAuthentication no
    ChallengeResponseAuthentication no

#### Disable root login
    PermitRootLogin no
    
#### Limit access to given users
    AllowUsers user1 user2 user3
    
#### Limit access to given IP address
    Port 22
    ListenAddress 10.0.0.1
    ListenAddress 192.168.0.1
    
#### Set an idle timeout interval
    ClientAliveInterval 300
    ClientAliveCountMax 0
    
#### Change user root directory
    ChrootDirectory /home/%u
    
#### Use Firewall to filter connections

#### Keep system and service up to date
