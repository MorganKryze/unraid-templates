# Unraid templates

Community Applications templates maintained by MorganKryze.

| App | What it is |
| --- | --- |
| [cairn](https://github.com/MorganKryze/cairn) | The directory page you hand to the people you host services for |

## cairn

One YAML file in, a static multilingual page out. No account to create, no
database, no outbound requests.

The first run works with an empty config folder: cairn serves a getting-started
page. Write a `services.yaml` in the folder you mapped to `/config` and cairn
picks it up within seconds, with no restart. The mapping is read-only because
cairn never writes to it.

The container runs read-only with every Linux capability dropped, and the image
is a single static Go binary in a `scratch` image, around 4 MB to pull.

Report anything broken on [the project's issues](https://github.com/MorganKryze/cairn/issues).
