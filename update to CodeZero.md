# 🔺 Upgrade to New Release (CodeZero) — Mac/Linux

## 1. Go to your gensyn screen (VPS)
```bash
screen -r gensyn
```

## 2. Stop your node
(Only if you are already inside the gensyn screen on VPS)  
Press:
```
ctrl + c
```

## 3. Move to rl-swarm directory
```bash
cd rl-swarm
```

## 4. Deactivate environment
```bash
deactivate
rm -rf .venv
```

## 5. Pull the latest release
```bash
git switch main
git reset --hard
git clean -fd
git pull origin main
```

### 6. Start the swarm node 🚀

```bash
python3 -m venv .venv
source .venv/bin/activate
```

```bash
./run_rl_swarm.sh
```

Stay synced — stay rewarded 🐝

