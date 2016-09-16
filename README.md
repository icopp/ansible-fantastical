# ansible-fantastical

Install Fantastical via the Mac App Store or Homebrew Cask.

Note that the name of the app bundle is `Fantastical 2.app`.

## Role Variables

* `prefer_mas_over_homebrew`: Defaults to `false`.

## Dependencies

* [icopp.mas-cli](https://github.com/icopp/ansible-mas-cli), but only if `prefer_mas_over_homebrew` is `true`.
* [icopp.homebrew-cask](https://github.com/icopp/ansible-homebrew-cask), but only if `prefer_mas_over_homebrew` is `false`.

## Example Playbook

```
  - hosts: all
    roles:
      - role: icopp.fantastical
```

```
  - hosts: all
    roles:
      - role: icopp.fantastical
        prefer_mas_over_homebrew: true
```

## License

MIT
