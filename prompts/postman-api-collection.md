I want to test a set of REST API routes in Postman. You will help me generate a complete Postman v2.1 Collection export (in JSON format) that I can import via "File > Import".

**IMPORTANT:** Do not generate anything yet. **WAIT** until I send you the list of routes.

Once I provide them, follow these instructions:

---

✅ **Requirements**:

-   Create a named collection (e.g., `"My API Tests"`)
-   Group related routes using **human-readable folder names** (e.g., `"User Tokens"`, `"Authentication"`, `"Session Tests"`)
-   Use `{{base_url}}` as a **collection-level variable** in all request URLs (e.g., `"http://localhost:3333"`)
-   Use **colon-prefixed path parameters** in routes (e.g., `/users/:id/tokens`, `/posts/:postId`)

    -   For every `:param`, define a matching `url.variable` entry in the request (e.g., `id`, `tokenId`, `postId`) with a **realistic default value** (e.g., `1`, `39`)
    -   Ensure these parameters are editable via the Postman UI

-   Include **query parameters** (e.g., `?limit=10`, `?q=search`) as part of the `url.query` section, with editable example values
-   Use correct HTTP methods (`GET`, `POST`, `DELETE`, etc.)
-   If a request has a body, include a realistic **example JSON payload**
-   Add a **Bearer Token authentication scheme** at the collection level using `{{auth_token}}` as the token value

    -   All requests should inherit this auth configuration
    -   Include `auth_token` as a **collection variable** with a placeholder value

-   Avoid including unnecessary metadata like timestamps, UUIDs, or auto-generated IDs unless explicitly required by Postman or the API itself
-   Output **ONLY** the valid raw Postman JSON (no explanations, markdown, or formatting)

---

Wait until I give you the list of routes before responding.
