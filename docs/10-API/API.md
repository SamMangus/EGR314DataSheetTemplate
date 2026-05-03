---
title: API
---

## Temperature Subsystem

My responsibility is to sense temperature and report the information to Adrian

## Team Member IDs

| Individual | Subsystem Number |
|------------|------------------|
| Sam B      | 1                |
| Adrian P   | 2                |
| Andrew I   | 3                |
| Jacob D    | 4                |
| Sam M(me)  | 5                |
| Mo A       | 6                |

---

## Messages Sent

---

### Message Type 3 — Print Sensor Value

| Field         | Byte 1       | Byte 2        | Byte 3          | Byte 4          | Byte 5          |
|---------------|--------------|---------------|-----------------|-----------------|-----------------|
| Variable Name | message_type | subsys_#      | sensor_id       | upper_sensor_#  | lower_sensor_#  |
| Variable Type | uint8_t      | uint8_t       | uint8_t         | int8_t          | int8_t          |
| Min Value     | 3            | 5             | 1               | 0               | 0               |
| Max Value     | 3            | 5             | 1               | 255             | 255             |
| Example       | 3            | 5             | 1               | 0x01            | 0x2C            |

Example: AZ511015YB

### Message Type 14 — Error Acknowledgement

| Field         | Byte 1       | Byte 2        | Byte 3          | Byte 4     |
|---------------|--------------|---------------|-----------------|------------|
| Variable Name | message_type | subsys_#      | error_code      | sender_#   |
| Variable Type | uint8_t      | uint8_t       | uint8_t         | int8_t     |
| Min Value     | 10           | 2             | 0               | 5          |
| Max Value     | 10           | 2             | 64              | 5          |
| Example       | 10           | 2             | 12              | 5          |

Example: AZ52E2YB

### Message Type 15 — Alert Control to Subsystem Status

| Field         | Byte 1       | Byte 2        | Byte 3          | Byte 4      |
|---------------|--------------|---------------|-----------------|-------------|
| Variable Name | message_type | subsys_#      | sender_#        | status_code |
| Variable Type | uint8_t      | uint8_t       | uint8_t         | int8_t      |
| Min Value     | 13           | 2             | 5               | 0           |
| Max Value     | 13           | 2             | 5               | 10          |
| Example       | 13           | 2             | 5               | 7           |

Example: AZ52F2YB

---

## Messages Received

---

### Message Type 12 — Subsystem Status Request

| Field         | Byte 1       | Byte 2        | Byte 3          |
|---------------|--------------|---------------|-----------------|
| Variable Name | message_type | subsys_#      | code            |
| Variable Type | uint8_t      | uint8_t       | uint8_t         |
| Min Value     | 12           | 5             | 0               |
| Max Value     | 12           | 5             | 15              |
| Example       | 12           | 5             | 4               |

Example: AZ25CYB