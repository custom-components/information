# Information - custom_components

This organization (shared space) was a result of a short discussion over on the [Discord server](https://discord.gg/c5DvZ4e).

A similar organization (shared space) was also made for [custom_cards](https://github.com/custom-cards).

This shared space is **not** supposed to be a replacement of any kind to the official sites/documentation for Home Assistant.

 - [Home Assistant GitHub](https://github.com/home-assistant)
 - [Home Assistant website](https://www.home-assistant.io/)
 - [Home Assistant developer documentation](https://developers.home-assistant.io/)

This shared space is a place where all users that develop custom_components are invited to share their codes for discoverability.
This space has some benefits.
 - Users that are looking for custom_components will have fever places to look.
 - There is less chance that multiple developers are working on the same thing.

## Rules

Like all other places there are need for some rules.
Your repository should have a name like this `component.platform` so for a sensor platform named abc the repo should be named `sensor.abc`, if abc is a component and not a platform give it the name `abc`.

In the reposiory there should be at least 2 files.
the component/platform (.py) file, and a README.md file.
The README file should contain instructions on how to "install" it (which folder to put the file in), and a configuration example.

## Updater component

The [custom_components](https://github.com/custom-components/custom_components) repository has a custom_component that will check the users installed custom_components against this org, to see if there is an update.

The  [tracker-card](https://github.com/ciotlosm/custom-lovelace/tree/master/tracker-card) custom_card makes a good companion for that component.

For the component to be able to check your repository, it **has** to be published here.
And must comply with this _standard_:

If it is a component the `.py` file **must** be here in your repository:\
`custom_components/YOUR_COMPONENT.py`

If it is a platform the `.py` file **must** be here in your repository:\
`custom_components/COMPONENT/YOUR_PLATFORM.py`

The `.py` file also will have to include a `__version__` variable, [example here](https://github.com/custom-components/sensor.authenticated/blob/master/custom_components/sensor/authenticated.py#L17)

## Want access to push your amazing stuff to this space?

Contact one of the users with an owner role.  
This are currently:

- [ludeeus](https://github.com/ludeeus) - You can find him on he [Discord server](https://discord.gg/c5DvZ4e) as `@Ludeeus#4212`

## When components / platforms are added to Home Assistant

If you get your custom_component in Home Assistant, the custom version of it should be archived.
Before archiving the README file should be updated to point users to the official documentation.
For a suggestion on how this can be done see the custom_component for [Cloudflare](https://github.com/custom-components/cloudflare).
