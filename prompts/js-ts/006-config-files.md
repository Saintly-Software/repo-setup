Move all config files and environment files to a new `.config/` folder to clean up the root directory of the project.

Some exceptions:

- typescript config
- storybook config

Update any commands in `package.json` that utilize any of these config files so that the command will find the config file correctly.
