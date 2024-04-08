# Tag example
```yaml
# overlays.yaml
overlay: 1.0.0
info:
  title: Overlay to customise API for Protect Earth
  version: 0.0.1
actions:
  - target: '$.tags[?(@.name=="Order")]'
    description: Provide more information for Order tag.
    update:
      description: >
        The Order resource represents a single order for trees, which can be fulfilled by one or more
        deliveries. Orders are created by the [Protect Earth team](https://protect.earth/contact) and
        are used to track the progress of your order from creation to delivery.
  - target: '$.tags[?(@.name=="Organization")]'
    description: Provide more information for Organization tag.
    update:
      description: >
        The Organization resource represents a single organization, which can be a charity, business,
        or other entity. Organizations are created by the [Protect Earth team](https://protect.earth/contact)
        and are connected to each of your Orders.
```
