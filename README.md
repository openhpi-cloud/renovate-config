# Shared Renovate Presets

Shared configuration preset for @renovatebot.

```json5 title="renovate.json5"
{
  $schema: "https://docs.renovatebot.com/renovate-schema.json",
  extends: [
    "local>openhpi-cloud/renovate-config"
  ]
}
```

## Validate preset configs locally

```console
$ docker run -it --rm -v .:/usr/src/app --entrypoint renovate-config-validator renovate/renovate --strict *.json5
 INFO: Validating default.json5
 INFO: Validating go.json5
 INFO: Validating node.json5
 INFO: Validating ruby.json5
 INFO: Validating terraform.json5
 INFO: Validating tool-version.json5
 INFO: Config validated successfully
```
