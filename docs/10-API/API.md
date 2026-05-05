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

| **Message Num** | **Byte 1-2(uint16_t)** | **Byte 3 (uint8_t)** | **Byte 4 (uint8_t)** | **Byte 5 (uint8_t)**  | **Byte 6 (uint8_t)**  | **Byte 7 (uint8_t)**  |  **Byte 8 (uint8_t)**   | **Purpose** |
| :--------------:| :--------------------: | :------------------: | :------------------: | :-------------------: | :-------------------: | :-------------------: | :---------------------: |:---------------------: |
|        3        |         0x03           |    Subsystem number  | Sensor number        | Upper sensor number          | Lower sensor number          | String Space          | String Space            | Print Sensor Value |

Example: AZ511015YB

### Message Type 14 — Error Acknowledgement

| **Message Num** | **Byte 1-2(uint16_t)** | **Byte 3 (uint8_t)** | **Byte 4 (uint8_t)** | **Byte 5 (uint8_t)**  | **Byte 6 (uint8_t)**  | **Byte 7 (uint8_t)**  |  **Byte 8 (uint8_t)**   | **Purpose** |
| :--------------:| :--------------------: | :------------------: | :------------------: | :-------------------: | :-------------------: | :-------------------: | :---------------------: |:---------------------: |
|        14       |         0x0E           |    Subsystem number  | Sending Subsystem Number | Upper number         | Lower number          | String Space          | String Space            | Subsystem error code response |

Example: AZ52E2YB

### Message Type 15 — Alert Control to Subsystem Status

| **Message Num** | **Byte 1-2(uint16_t)** | **Byte 3 (uint8_t)** | **Byte 4 (uint8_t)** | **Byte 5 (uint8_t)**  | **Byte 6 (uint8_t)**  | **Byte 7 (uint8_t)**  |  **Byte 8 (uint8_t)**   | **Purpose** |
| :--------------:| :--------------------: | :------------------: | :------------------: | :-------------------: | :-------------------: | :-------------------: | :---------------------: |:---------------------: |
|        15       |         0x0F           |    Subsystem number  | Sending Subsystem Number | Upper number         | Lower number          | String Space          | String Space            | Subsystem status code response |

Example: AZ52F2YB

---

## Messages Received

---

### Message Type 12 — Subsystem Status Request

| **Message Num** | **Byte 1-2(uint16_t)** | **Byte 3 (uint8_t)** | **Byte 4 (uint8_t)** | **Byte 5 (uint8_t)**  | **Byte 6 (uint8_t)**  | **Byte 7 (uint8_t)**  |  **Byte 8 (uint8_t)**   | **Purpose** |
| :--------------:| :--------------------: | :------------------: | :------------------: | :-------------------: | :-------------------: | :-------------------: | :---------------------: |:---------------------: |
|        12       |         0x0C           |    Subsystem number  | Upper number         | Lower number          | String Space          | String Space          | String Space            | Subsystem status code |

Example: AZ25CYB