---
description: Thrown when an authenticated user has insufficient permissions to accomplish a task.
seo-description: Thrown when an authenticated user has insufficient permissions to accomplish a task.
seo-title: authorizationFault
solution: Experience Manager
title: authorizationFault
topic: Scene7 Image Production System API
uuid: 8b8df22a-aa76-4cbd-9c14-89969c5f9620
---

# authorizationFault{#authorizationfault}

Thrown when an authenticated user has insufficient permissions to accomplish a task.

 Syntax 

## Fault Types {#section-1f04dec489714ee6bb7256fae6ab7730}

|  ID  | Fault  |
|---|---|
|  20000  | `AUTHORIZATION_FAULT_CODE_INVALID_COMPANY`  |
|  20001  | `AUTHORIZATION_FAULT_CODE_INVALID_REQUEST_USERNAME`  |
|  20002  | `AUTHORIZATION_FAULT_CODE_INVALID_REQUEST_USER`  |
|  20003  | `AUTHORIZATION_FAULT_CODE_NO_OPERATION_PERMISSION`  |
|  20004  | `AUTHORIZATION_FAULT_CODE_NO_IMPERSONATION_PERMISSION`  |
|  20005  | `AUTHORIZATION_FAULT_CODE_ILLEGAL_PARAMETER_VALUE`  |
|  20006  | `AUTHORIZATION_FAULT_CODE_ILLEGAL_COMPANY`  |
|  20007  | `AUTHORIZATION_FAULT_CODE_ILLEGAL_REQUEST_USER`  |
|  20008  | `AUTHORIZATION_FAULT_CODE_ILLEGAL_ACCESS_GROUP`  |
|  20009  | `AUTHORIZATION_FAULT_CODE_MISSING_PERMISSION`  |

## Fault Fields {#section-4e3e41f41fea402a9ae314bfd05f663e}

|  Name  | Type  | Description  |
|---|---|---|
|  `code`  | `xsd:int`  | Fault ID  |
|  `reason`  | `xsd:string`  | An informative message describing the fault.  |

