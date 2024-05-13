# Take Hostage Script for FiveM

## Description

This script allows players in FiveM to take other players hostage. It adds a new level of interaction and role-playing opportunities to your server.

## Features

- Easy to use commands for taking and releasing hostages.
- Customizable key bindings and commands.
- Compatible with both ESX and standalone servers.
- Optimized for performance to ensure minimal impact on server resources.

## Requirements

- FiveM server
- ESX Framework (optional, if you want ESX integration)

## Installation

1. **Download the script**: Download the latest version of the script from the [releases page](#) (replace with your download link).

2. **Extract the script**: Extract the downloaded file into your FiveM server's `resources` directory.

3. **Add to server config**: Add the following line to your `server.cfg` file:
    ```plaintext
    ensure take-hostage
    ```

4. **Configure the script**: Open the `config.lua` file inside the `take-hostage` resource folder to customize the settings as per your requirements.

## Usage

### Commands

- **Take Hostage**: Use the command `/takehostage` to initiate taking a nearby player as a hostage.
- **Release Hostage**: Use the command `/releasehostage` to release a hostage.

### Key Bindings

By default, you can use the following key bindings (can be changed in the `config.lua`):

- **Take Hostage**: Press `H`
- **Release Hostage**: Press `R`

## Configuration

The script is highly configurable. You can modify the following settings in the `config.lua` file:

- **Key bindings**: Change the keys for taking and releasing hostages.
- **Distance**: Set the maximum distance for taking a hostage.
- **Messages**: Customize the messages displayed to players when they take or release a hostage.

Example `config.lua`:

Config = {}

-- Key bindings
Config.TakeHostageKey = 74 -- H
Config.ReleaseHostageKey = 82 -- R

-- Maximum distance to take a hostage
Config.MaxDistance = 2.0

-- Messages
Config.Messages = {
    TakeHostage = "You have taken a hostage!",
    ReleaseHostage = "You have released the hostage!",
    TooFar = "You are too far away to take a hostage."
}
