# Description

The resource allows you to configure a computer by changing its name and
description and modifying its Active Directory domain or workgroup membership.

## Parameters

### DeleteExistingComputerAccount

When joining a domain, if a computer account with the same name already exists:

- **`$true`** (default): The existing computer account is deleted and recreated
  (historical behavior).
- **`$false`**: The existing computer account is reused. This preserves the
  machine SID, group memberships, GPO links, and other AD attributes.
