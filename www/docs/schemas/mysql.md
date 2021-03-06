---
id: mysql
title: MySQL Schema
---

The schema generated for a MySQL database when using the built-in models.

## User

```json
{
  "id": {
    "name": "id",
    "type": "int",
    "nullable": false,
    "default": null
  },
  "name": {
    "name": "name",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "email": {
    "name": "email",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "email_verified": {
    "name": "email_verified",
    "type": "timestamp",
    "nullable": false,
    "default": null
  },
  "image": {
    "name": "image",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "created": {
    "name": "created",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  },
  "updated": {
    "name": "updated",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  }
}
```

## Account

```json
{
  "id": {
    "name": "id",
    "type": "int",
    "nullable": false,
    "default": null
  },
  "compound_id": {
    "name": "compound_id",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "user_id": {
    "name": "user_id",
    "type": "int",
    "nullable": false,
    "default": null
  },
  "provider_type": {
    "name": "provider_type",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "provider_id": {
    "name": "provider_id",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "provider_account_id": {
    "name": "provider_account_id",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "refresh_token": {
    "name": "refresh_token",
    "type": "text",
    "nullable": false,
    "default": null
  },
  "access_token": {
    "name": "access_token",
    "type": "text",
    "nullable": false,
    "default": null
  },
  "access_token_expires": {
    "name": "access_token_expires",
    "type": "timestamp",
    "nullable": false,
    "default": null
  },
  "created": {
    "name": "created",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  },
  "updated": {
    "name": "updated",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  }
}
```

## Session

```json
{
  "id": {
    "name": "id",
    "type": "int",
    "nullable": false,
    "default": null
  },
  "user_id": {
    "name": "user_id",
    "type": "int",
    "nullable": false,
    "default": null
  },
  "expires": {
    "name": "expires",
    "type": "timestamp",
    "nullable": false,
    "default": null
  },
  "session_token": {
    "name": "session_token",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "access_token": {
    "name": "access_token",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "created": {
    "name": "created",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  },
  "updated": {
    "name": "updated",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  }
}
```

## Verification Request

```json
{
  "id": {
    "name": "id",
    "type": "int",
    "nullable": false,
    "default": null
  },
  "identifier": {
    "name": "identifier",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "token": {
    "name": "token",
    "type": "varchar(255)",
    "nullable": false,
    "default": null
  },
  "expires": {
    "name": "expires",
    "type": "timestamp",
    "nullable": false,
    "default": null
  },
  "created": {
    "name": "created",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  },
  "updated": {
    "name": "updated",
    "type": "timestamp(6)",
    "nullable": false,
    "default": "CURRENT_TIMESTAMP(6)"
  }
}
```