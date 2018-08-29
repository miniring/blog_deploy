---
title: mac-dockbar 딜레이 조정
categories:
  - null
tags:
  - mac
date: 2018-08-29 10:28:03
---

# Dockbar 딜레이 조정

### 딜레이 제거

```bash
defaults write com.apple.dock autohide -bool true && defaults write com.apple.dock autohide-delay -float 0 && defaults write com.apple.dock autohide-time-modifier -float 0 && killall Dock
```

### 딜레이 조정

```bash
defaults write com.apple.dock autohide -bool true && defaults write com.apple.dock autohide-delay -float 0.3 && defaults write com.apple.dock autohide-time-modifier -float 0.3 && killall Dock
```

### 원상복구

```bash
defaults delete com.apple.dock autohide && defaults delete com.apple.dock autohide-delay && defaults delete com.apple.dock autohide-time-modifier && killall Dock
```
