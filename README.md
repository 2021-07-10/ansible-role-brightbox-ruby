# Ansible Role: Brightbox Ruby

Ruby packages for Ubuntu

## Requirements

None

## Role Variables

* `brightbox_ruby_version`: 指定 `Ruby` 版本号
* `brightbox_ruby_gems`: 需要全局安装的 `Gem`
* `brightbox_ruby_gems_deps`: `Gem` 依赖的扩展包

## Dependencies

None

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: guxiaobai.brightbox-ruby
      brightbox_ruby_version: 2.7
      brightbox_ruby_gems:
        - mysql2
      brightbox_ruby_gems_deps:
        - libmysqlclient-dev
```

##  License

BSD

## Ref

* [Ruby packages for Ubuntu - Brightbox](https://www.brightbox.com/docs/ruby/ubuntu/)