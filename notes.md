Jobs:
  Run in parallel by default

Steps:
  Run sequentially by default

Event Filters
  ```
  on:
    push:
      branches:
        - main
        - 'releases/**'
      paths-ignore:
        - 'docs/**'
  ```

Activity Types
  ```
  on:
    pull_request:
      types: [opened, synchronize]
      branches:
        - main
        - 'releases/**'
  ```

Ternary Operations
  Providing a default: ${{ expression || default_value }}. The default_value will be used if the expression evaluates to a falsy value.
  Using the ternary operation: ${{ expression && truthy_value || falsy_value }}. The truthy_value will be used if the expression evaluates to a truthy value, and the falsy_value will be used otherwise.