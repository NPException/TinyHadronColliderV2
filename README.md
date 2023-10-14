This fork of the amazing "Tiny Hadron Collider" by Matt Hurtado now serves as a small
example on how to integrate the [babashka](https://babashka.org) based build system from
NPException's [Playdate App Template](https://github.com/NPException/playdate-app-template).

The only necessary change to the project was to add the [bb.edn](bb.edn) file.
Now, if you have babashka installed you can build the project, run it in the simulator,
or create a distribution-ready `.pdx.zip` of it by using any the following commands:

```bash
# just build the app (for example to have the Playdate compiler check for some errors)
bb build
```
```bash
# build the app and start it in the Playdate simulator
bb build-and-run
```
```bash
# create a .pdx.zip file ready for distribution on itch.io (or anywhere else)
bb build-release
```

After copying over the [GitHub workflow folder](.github) too, this project now has automated
release builds too: ![Automated Release Badge](https://github.com/NPException/TinyHadronColliderV2/actions/workflows/auto-release.yml/badge.svg)

# Tiny Hadron Collider
<img src="https://i.imgur.com/v7ULMUu.gif" width="400" height="240" />

### A very small idler for the PlayDate

---

# Requirements
Tiny Hadron Collider runs using the following modules:
* [Noble Engine](https://github.com/NobleRobot/NobleEngine)
* [AnimatedSprite](https://github.com/Whitebrim/AnimatedSprite)

# Gameplay:
1. **Crank** the handle to fill up the circle to increase your score
2. **Press B** to open/close the item menu to improve your Tiny Hadron Collider
3. **Press Start** to save, load, or reset the game