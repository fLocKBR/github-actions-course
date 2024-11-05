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