# A3H

ArmA 3 Hunting Simulator - 2017

### Development Environment

See the [ACE3 documentation](http://ace3mod.com/wiki/development/setting-up-the-development-environment.html) on setting up your development environment.

### Using CI

This template comes with some basic scripts to validate and enforce parts of the ACE3 coding guidelines. You can find those scripts in the tools directory.

- sqf_validator.py - checks all .sqf files in the addons directory and checks for missing brackets, missing semi-colons and tab usage.
- config_style_checker.py - checks all .hpp and .cpp files in the addons directory and checks for missing brackets and tabs.

For more information on the guidelines, see ACE3 coding guidelines.

You can use these scripts in combination with CI - if you are on GitHub and use Travis-CI, here is an example:

```yml
language: python
python:
- '3.4'
script:
- python3 tools/sqf_validator.py
- python3 tools/config_style_checker.py
```

Check out the [Official Website](http://innovativestudios.github.io/a3h)
