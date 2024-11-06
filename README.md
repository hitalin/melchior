# Provisioning servers with Nix

## wpa_supplicant
```consol
wpa_passphrase MYSSID passphrase > /etc/wpa_supplicant.conf
```

## tailscale
```consol
tailscale login
tailscale up --ssh
```

## cloudflared
```consol
cloudflared tunnel login
cloudflared tunnel create imisskey
```

## warp

```
warp-cli registration new
warp-cli registration license <your-warp-licence-key-subscribed-on-mobile-device>
warp-cli registration show
warp-cli connect
```

## nix
```consol
sudo nixos-rebuild switch --flake ".#myNixOS"
nix run home-manager -- switch --flake ".#myHome"
```