# terraform refresh

> Update the state file to match the current state of remote infrastructure.
> This command is deprecated in favor of `terraform apply -refresh-only`.
> More information: <https://developer.hashicorp.com/terraform/cli/commands/refresh>.

- Refresh the state in the current directory:

`terraform refresh`

- Specify values for input variables:

`terraform refresh -var '{{name1}}={{value1}}' -var '{{name2}}={{value2}}'`

- Specify values for input variables from a file:

`terraform refresh -var-file {{path/to/file.tfvars}}`

- Refresh a specific resource:

`terraform refresh -target {{resource_type.resource_name[instance_index]}}`

- Refresh without holding the state lock:

`terraform refresh -lock=false`

- Refresh with a custom parallelism limit:

`terraform refresh -parallelism {{5}}`
