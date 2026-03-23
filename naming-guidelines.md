# Descriptive Variable and Function Names

Use names that communicate intent without extra comments. Favor clarity over brevity and choose domain words the team already uses.

- Variables: prefer specific nouns; avoid ambiguous letters like `x` or `data`. Include units (`durationMs`, `distanceKm`) and the collection shape (`usersById`, `pendingOrders`).
- Booleans: start with `is`, `has`, `can`, or `should` to show truthiness (`isAuthorized`, `hasUnsavedChanges`).
- Functions: use verb + object to state the action and target (`loadUserProfile`, `calculateInvoiceTotal`). Describe outcomes or side effects (`sendPasswordResetEmail`, `saveDraftAndNotify`).
- Temporary or loop variables: describe role, not position (`currentUser`, `nextPageUrl`, `matchingOrder`) unless the code truly needs indices (`i`, `j`).
- Error variables: encode context and failure (`orderSaveError`, `tokenValidationError`) so logs are searchable.
- Event handlers and callbacks: make trigger clear (`onFormSubmit`, `handleSocketReconnect`).

Before/after examples:

| Avoid | Prefer | Why |
| --- | --- | --- |
| `tmp`, `data` | `pendingOrders`, `userProfile` | Names reflect the domain object. |
| `flag` | `isEmailVerified` | Shows boolean nature and meaning. |
| `getInfo()` | `fetchCustomerSummary()` | States action and subject. |
| `doIt()` | `retryPaymentAndLog()` | Explains side effects. |
| `arr`, `list1` | `visibleProducts`, `archivedSessions` | Shows contents and purpose. |
| `calc()` | `calculateTaxAmount()` | Verb + object, includes unit/target. |

If a name still needs a comment to make sense, rename it.
