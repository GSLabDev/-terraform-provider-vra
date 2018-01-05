---
layout: "vra"
page_title: "vRealize Automation: vra_execute_blueprint"
sidebar_current: "docs-vra-resource-inventory-folder"
description: |-
  Provides a vRealize Blueprint Executing resource. This can be used to execute blueprint in vRealize.
---

# vra\_execute\_blueprint

Provides a vRealize executing resource. This can be used to execute blueprints in vRealize.

## Example Usage

```hcl
# Execute a blueprint
resource "vra_execute_blueprint" "ExecuteBlueprint" {
       blueprint_name = "Create simple virtual machine"
       input_file_name = "data.json"
       time_out = 20
}
```

## Argument Reference

The following arguments are supported:

* `blueprint_name` - (Required) The Blueprint Name which we want to execute
* `input_file_name` - (Required) The configuration file which is required to execute blueprint
* `timeout` - (Optional) Maximum time to wait for the blueprint to execute