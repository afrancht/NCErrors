# NuCypher Error Report 3

## System Information

- MacOS Mojave 10.14.6 (18G95)
- MacBook Pro (13-inch, 2016, Four Thunderbolt 3 Ports)
- 2.9 GHz Intel Core i5
- 8 GB 2133 MHz LPDDR3

- Python Version: 3.7.0
- Branch: master

## Error 1 found in running local Ursula fleet command from `scripts/local_fleet`

- URL: https://docs.nucypher.com/en/latest/demos/local_fleet_demo.html?highlight=fleet
- Github URL: https://github.com/nucypher/nucypher/tree/master/scripts/local_fleet
- Video: https://youtu.be/jRAQHCHUBeQ

I can run a single Ursula node and I can then launch other Ursulas which do identify the first one (and I think recognises them as a Teacher node) but when I try to run a fleet using the command below I see the error below.

When executing command 3: `$ python run_local_ursula_fleet.py`

It returns the following error:

```
[nucypher-dItPgA_X]➜  local_fleet git:(master) ✗ python run_local_ursula_fleet.py
Traceback (most recent call last):
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/bin/nucypher", line 6, in <module>
    from nucypher.cli.main import nucypher_cli
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/main.py", line 22, in <module>
    from nucypher.cli import status
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/status.py", line 24, in <module>
    from nucypher.cli.config import nucypher_click_config
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 45, in <module>
    class NucypherClickConfig:
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 55, in NucypherClickConfig
    log_to_sentry = get_env_bool("NUCYPHER_SENTRY_LOGS", True)
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 40, in get_env_bool
    return strtoobool(os.environ[var_name])
NameError: name 'strtoobool' is not defined
Traceback (most recent call last):
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/bin/nucypher", line 6, in <module>
    from nucypher.cli.main import nucypher_cli
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/main.py", line 22, in <module>
    from nucypher.cli import status
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/status.py", line 24, in <module>
    from nucypher.cli.config import nucypher_click_config
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 45, in <module>
    class NucypherClickConfig:
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 55, in NucypherClickConfig
    log_to_sentry = get_env_bool("NUCYPHER_SENTRY_LOGS", True)
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 40, in get_env_bool
    return strtoobool(os.environ[var_name])
NameError: name 'strtoobool' is not defined
Traceback (most recent call last):
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/bin/nucypher", line 6, in <module>
    from nucypher.cli.main import nucypher_cli
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/main.py", line 22, in <module>
    from nucypher.cli import status
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/status.py", line 24, in <module>
    from nucypher.cli.config import nucypher_click_config
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 45, in <module>
    class NucypherClickConfig:
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 55, in NucypherClickConfig
    log_to_sentry = get_env_bool("NUCYPHER_SENTRY_LOGS", True)
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 40, in get_env_bool
    return strtoobool(os.environ[var_name])
NameError: name 'strtoobool' is not defined
Traceback (most recent call last):
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/bin/nucypher", line 6, in <module>
    from nucypher.cli.main import nucypher_cli
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/main.py", line 22, in <module>
    from nucypher.cli import status
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/status.py", line 24, in <module>
    from nucypher.cli.config import nucypher_click_config
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 45, in <module>
    class NucypherClickConfig:
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 55, in NucypherClickConfig
    log_to_sentry = get_env_bool("NUCYPHER_SENTRY_LOGS", True)
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 40, in get_env_bool
    return strtoobool(os.environ[var_name])
NameError: name 'strtoobool' is not defined
Traceback (most recent call last):
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/bin/nucypher", line 6, in <module>
    from nucypher.cli.main import nucypher_cli
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/main.py", line 22, in <module>
    from nucypher.cli import status
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/status.py", line 24, in <module>
    from nucypher.cli.config import nucypher_click_config
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 45, in <module>
    class NucypherClickConfig:
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 55, in NucypherClickConfig
    log_to_sentry = get_env_bool("NUCYPHER_SENTRY_LOGS", True)
  File "/Users/afrancht/.local/share/virtualenvs/nucypher-dItPgA_X/lib/python3.7/site-packages/nucypher/cli/config.py", line 40, in get_env_bool
    return strtoobool(os.environ[var_name])
NameError: name 'strtoobool' is not defined
A process has ended with a probable error condition: process ended with exit code 1.
A process has ended with a probable error condition: process ended with exit code 1.
A process has ended with a probable error condition: process ended with exit code 1.
A process has ended with a probable error condition: process ended with exit code 1.
A process has ended with a probable error condition: process ended with exit code 1.
```


