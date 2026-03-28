---
title: API
---

## Temperature Subsystem

My responsibility is to sense temperature and report the information to Adrian

## Team Member IDs

| Individual | Subsystem Number |
|------------|-----------------|
| Sam B      | 1               |
| Adrian P   | 2               |
| Andrew I   | 3               |
| Jacob D    | 4               |
| Sam M(me)  | 5               |
| Mo A       | 6               |

---

## Messages Sent

All messages I send go directly to Adrian (Subsystem 2).

---

### Message Type 3 — Subsystem Status Request

Sent to Adrian to request a status update from the system.

| Field         | Byte 1       | Byte 2        | Byte 3          | Byte 4          | Byte 5          |                
|---------------|--------------|---------------|-----------------|-----------------|-----------------|
| Variable Name | message_type | subsys_#      | sensor_id       | upper_sensor_#  | lower_sensor_#  |                 
| Variable Type | uint8_t      | uint8_t       | uint8_t         | int8_t          | int8_t          |                 
| Min Value     | 3            | 5             | 1               |                 |                 |                 
| Max Value     | 3            | 5             | 1               |                 |                 |                 
| Example       | 3            | 5             | 1               |                 |                 |                 

**Example packet:**

### Message Type 14 — Error Acknowledgement

| Field         | Byte 1       | Byte 2        | Byte 3          | Byte 4     |
|---------------|--------------|---------------|-----------------|------------|
| Variable Name | message_type | sender_subsys | receiver_subsys | error_code |
| Variable Type | uint8_t      | uint8_t       | uint8_t         | int8_t     |
| Min Value     | 10           | 1             | 2               | 0          |
| Max Value     | 10           | 1             | 2               | 64         |
| Example       | 10           | 1             | 2               | 0          |

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


