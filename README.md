# Provisioning servers with Nix

```consol
sudo nixos-rebuild switch --flake ".#myNixOS"
nix run home-manager -- switch --flake ".#myHome"
```