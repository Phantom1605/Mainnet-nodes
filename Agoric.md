![Ag icon](https://user-images.githubusercontent.com/85427001/169720946-449c7492-b40e-4e86-9da4-e5517b77a97d.png)

## How I launched my Agoric validator
### Hardware
- AMD® Ryzen™ 7 3700X
- 8c/16t @3.60GHz
- RAM64 GB
- Storage  1 TB NVME
- Network1 Gbps
### My Agoric architecture
![Axel845 Agoric Arch](https://user-images.githubusercontent.com/85427001/169721057-98dedfc9-cddf-479c-bb01-586ea60ae731.png)
- Validator node
- 5 Sentry Nodes
- 1 tmkms server
### Servers Login
All servers are set to multi-factor login mode. Google 2FA + SSH key.
#### tmkms server
1)On this diagram you can see that tmkms server uses Software Signing Provider.

#### 5 Sentry Nodes
I believe that 5 sentry nodes is the optimal number to resist DDoS attacks.
#### Validator node
It should be borne in mind that when the validator is working together with the tmkms server, the `priv_validator_key.json` is missing on the node with the validator. It is located on tmkms with Software Signing Provider.
