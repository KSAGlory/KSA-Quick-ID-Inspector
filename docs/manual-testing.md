# Manual Testing Guide

Use a separate test save and back up important game files before validating a new build.

## Test environment

Record the following information before beginning:

- GTA San Andreas version
- CLEO version
- Mod Loader version, if used
- Relevant compatibility mods
- Display resolution and aspect ratio

## Installation

1. Install the compiled script through Mod Loader or the CLEO directory.
2. Start the game and load the test save.
3. Confirm that no new errors appear in `cleo.log` or `modloader.log`.

## Pedestrian inspection

1. Aim at several pedestrian models.
2. Confirm that the displayed model ID matches the targeted pedestrian.
3. Confirm that the displayed health value updates when the pedestrian takes damage.
4. Move the aim away and verify that stale information does not remain visible.

## Vehicle inspection

1. Enter several vehicle models.
2. Confirm that the vehicle name and model ID are correct.
3. Damage a vehicle and confirm that the health value updates.
4. Exit the vehicle and verify that stale vehicle information is cleared.

## Repeated vehicle transitions

1. Enter a vehicle and note the displayed name, model ID, and health value.
2. Exit the vehicle and confirm that all vehicle details disappear immediately.
3. Enter a different vehicle and confirm that every displayed field updates to the new vehicle.
4. Repeat the enter-and-exit cycle at least five times, alternating vehicles when possible.
5. After the final exit, wait several seconds and confirm that no outdated vehicle information reappears.

## Toggle and presentation

1. Type `KSAID` and confirm that the interface is disabled.
2. Type `KSAID` again and confirm that the interface returns.
3. Repeat the test at standard and widescreen resolutions.
4. Confirm that the overlay remains readable without hiding important game information.

## Reporting results

Record every failed step with reproduction instructions and the relevant log lines. Remove usernames, personal paths, and unrelated private information before sharing logs.
