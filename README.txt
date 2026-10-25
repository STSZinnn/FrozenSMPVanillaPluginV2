Punch Snowball + Infinite TNT v1.3 for Paper 1.21.11

BUILD ONCE USING EXISTING GITHUB ACTIONS
Upload/replace the source file, config.yml and plugin.yml in your existing repository.
Edit build.gradle.kts version to 1.3.0. Use Actions -> Build plugin -> Run workflow.
Download JAR from Artifacts; put JAR in plugins and remove older JAR; restart.

FROM THEN ON - CHANGE SETTINGS WITHOUT COMPILING
1. Open plugins/PunchSnowball/config.yml ON THE RUNNING SERVER.
2. Edit values (tnt cooldown, fuse, radius, power, damage, snowball knockback).
3. Save and run /punchreload as OP.

COMMANDS
/givesnowball [player]
/givetnt [player]
/punchreload

CAVEATS
- TNT creates a real explosion and CAN DESTROY BLOCKS. Back up your world first.
- 4 blocks is a maximum radius: block hardness and explosion physics affect actual destruction.
- A 2-heart hit means 4 health points; extra protections/events may change it.
- TNT item cooldown also prevents using ordinary TNT until cooldown ends.
- New config settings do not backfill automatically if old config.yml already exists.
  Replace or merge its TNT section with the updated config.
- Existing TNT item keys are preserved; old special items should still work.
- This source was not compiled in this environment; GitHub Actions validates the build.
