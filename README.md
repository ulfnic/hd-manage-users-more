# hd-manage-users-more

Created for HedgeDoc 1.9.9, mileage may vary on other versions.

Accompanies and expands on the existing CLI management in `bin/manage_users` using the same format.

## Syntax
```bash
manage_users_more
  --verify EMAIL        # Verify user password with specified user-email
  --change EMAIL        # Change user password with specified user-email
  --pass PASSWORD       # Use password from cmdline rather than prompting
  --new-pass PASSWORD   # Use new-password from cmdline rather than prompting
```

## Examples of use
```bash
# Verify a password
/hedgedoc/bin/manage_users_more --verify 'my@account.com' --pass '1234'
```
```bash
# Verify a password with a password prompt
/hedgedoc/bin/manage_users_more --verify 'my@account.com'
```
```bash
# Change a password
/hedgedoc/bin/manage_users_more --change 'my@account.com' --pass '1234' --new-pass 'abcd'
```
```bash
# Change a password with a password prompt
/hedgedoc/bin/manage_users_more --change 'my@account.com'
```

## License
Licensed under GNU Affero General Public License v3. See LICENSE for details.
