# Useful Lab Commands

## Check audit policy

```cmd
auditpol /get /category:*
```

## Check logon auditing

```cmd
auditpol /get /subcategory:"Logon"
```

## Check process-creation auditing

```cmd
auditpol /get /subcategory:"Process Creation"
```

## Enable process-creation success auditing

Run Command Prompt as Administrator:

```cmd
auditpol /set /subcategory:"Process Creation" /success:enable
```

## Enable logon success/failure auditing

Run Command Prompt as Administrator:

```cmd
auditpol /set /subcategory:"Logon" /success:enable /failure:enable
```

These commands are for the authorized local test environment only.
