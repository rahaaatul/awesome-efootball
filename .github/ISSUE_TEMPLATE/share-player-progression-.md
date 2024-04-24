name: "🐞 Share Player Training Method"
description: Share how you trained your player
title: "[Player Card Name] [Player Name] Training Method"
labels: ["training"]
assignees: []
body:
  - type: markdown
    attributes:
      value: |
        First off, thanks for taking the time to contribute! Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make will benefit everybody else and are greatly appreciated.
  - type: input
    id: player-card
    attributes:
      label: Player Card Name
      description: >
        Please describe your environment in as much detail as possible. Otherwise, we may not be able to reproduce the issue.
      placeholder: >
        Example:
          print "Device: $VENDOR | $OSTYPE | $CPUTYPE"
          print "Shell: $SHELL | $ZSH_ARGZERO | $ZSH_PATCHLEVEL"
          print "Zi: $(git -C $ZI[BIN_DIR] rev-parse HEAD)"
    validations:
      required: true
  - type: textarea
    id: repro
    attributes:
      label: Training Method
      description: "Fill the 0's with your progression points"
      value: |
        Shooting: `0`
        Passing: `0`
        Dribbling: `0`
        Dexterity: `0`
        Lower Body Strength: `0`
        Aerial Strength: `0`
        Defending: `0`
        GK 1: `0`
        GK 2: `0`
        GK 3: `0`
      render: bash
    validations:
      required: true
  - type: textarea
    id: screenshot
    attributes:
      label: Screenshot
      description: "Give a screenshot of the player card."
    validations:
      required: true