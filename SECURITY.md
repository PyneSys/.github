# Security Policy

This policy covers every PyneSys repository, including PyneCore and its broker plugins.

## Supported versions

Security fixes are released for the latest published version of each package. Please upgrade
to the latest release before reporting, and check whether the problem still occurs there.

## Reporting a vulnerability

**Do not open a public issue, discussion or pull request for a security problem.** Report it
privately on GitHub instead:

1. Open the **Security** tab of the affected repository.
2. Click **Report a vulnerability**.

For PyneCore, the form is at
[github.com/PyneSys/pynecore/security/advisories/new](https://github.com/PyneSys/pynecore/security/advisories/new).
If you are unsure which repository is affected, report it on PyneCore. If you cannot use GitHub,
send a short note through the [contact form](https://pynesys.io/contact/) without the details,
and we will arrange a private channel.

Please include:

- the affected package and version;
- what the problem is and what an attacker could do with it;
- the steps or a minimal script that reproduce it.

## What happens next

We acknowledge the report, confirm or rule out the problem, and keep you updated while a fix is
prepared. Once a fixed version is released, we publish a security advisory and credit you,
unless you ask to stay anonymous. Please keep the details private until then.

## Scope

In scope, for example:

- leaking or mishandling broker credentials and API keys (configuration files, logs, error
  messages);
- a broker plugin sending, changing or cancelling orders that the strategy did not request;
- exposing the Pine source or the API key that `pyne compile` sends to the PyneSys API;
- code execution or file access that a crafted data file, configuration file or downloaded
  package can trigger.

Out of scope:

- differences from TradingView results (please open a regular issue);
- losses caused by a strategy's own logic;
- problems in third-party services, brokers or exchanges themselves.
