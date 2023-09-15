# Bonus Activity

Objectives:
- Implement a `swagger-ui` for a simple API interaction and documentation

What to do:
- In `build.gradle`, add `implementation 'org.springdoc:springdoc-openapi-starter-webmvc-ui:2.0.4'` under `dependencies`
- In `TodoController.java`, add `@Operation(summary = "Get Todo")` above `@GetMapping`
- In `TodoController.java`, add `@Operation(summary = "Create Todo")` above `@PostMapping`
- In `TodoController.java`, add `@Operation(summary = "Update Todo")` above `@PutMapping`

Acceptance Criteria:
- Can access the `swagger-ui` using `http://localhost:8080/swagger-ui.html`
- `swagger-ui` should have the following:
    - `GET /todo`
    - `POST /todo`
    - `PUT /todo`