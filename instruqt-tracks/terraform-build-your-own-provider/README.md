# terraform-build-your-own-provider

## TODO

- Check the test suite runs successfully
- Merge Nick Polish
- Address Kawsar Feedback
- Remove the terraform lock file w/ the install Make directive (on every branch)
- Use the actual hashicorp version of hashicups instead of my version (git clone --branch boilerplate https://github.com/hashicorp/terraform-provider-hashicups)
- `last_updated` is being set to `tostring` not the actual timestamp
- https://www.terraform.io/docs/extend/resources/import.html

## Build the Image

Using `instruqt-packer/hashistack-go-development`.

```bash
make \
    PROJECT=instruqt-hashicorp \
    STACK_VERSION=0.9.1 \
    CONSUL_VERSION=1.9.5 \
    NOMAD_VERSION=1.0.4 \
    TERRAFORM_VERSION=0.15.3 \
    VAULT_VERSION=1.7.1 \
    DOCKER_COMPOSE_VERSION=1.29.1 \
    GO_VERSION=1.16.3 \
    build
```

### Challenge Work

- Setup and Implement Read (still can be a bit tricky if need to rebuild the provider)
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Add Authentication to a Provider
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Implement a Complex Read
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Debug a Terraform Provider
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Implement Create
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Implement Update
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Implement Delete
    -[x] Setup
    -[x] Check
    -[x] Solve
    -[?] Cleanup
- Implement Import
    -[x] Setup
    -[ ] Check
    -[ ] Solve
    -[?] Cleanup
