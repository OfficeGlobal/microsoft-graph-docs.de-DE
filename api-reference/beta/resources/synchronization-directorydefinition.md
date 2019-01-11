---
title: Ressourcentyp directoryDefinition
description: Enthält die Synchronisierung Engine ein Verzeichnis und ihre Objekte Informationen. Diese Ressource weist dem Synchronisierungsmodul beispielsweise, dass das Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden. In der Reihenfolge für das Objekt und das Attribut an Synchronisierungsregeln und Objekt Zuordnungen teilzunehmen müssen sie als Teil der Definition der Directory definiert werden.
localization_priority: Normal
ms.openlocfilehash: e6b2b55fb9e9e7963b01403c6aed2f0997e2318b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874522"
---
# <a name="directorydefinition-resource-type"></a>Ressourcentyp directoryDefinition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält die Synchronisierung Engine ein Verzeichnis und ihre Objekte Informationen. Diese Ressource weist dem Synchronisierungsmodul beispielsweise, dass das Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden. In der Reihenfolge für das Objekt und das Attribut an [Synchronisierungsregeln](synchronization-synchronizationrule.md) und [Objekt Zuordnungen](synchronization-objectmapping.md)teilzunehmen müssen sie als Teil der Definition der Directory definiert werden.

Im Allgemeinen wird dem [Synchronisierungsschema](synchronization-synchronizationschema.md) als Teil der [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md) bereitgestellt am häufigsten verwendeten Objekte und Attribute für dieses Verzeichnis definieren. Wenn das Verzeichnis, das Hinzufügen von benutzerdefinierten Attributen unterstützt, sollten Sie die Standarddefinition durch eigene benutzerdefinierte Objekte oder Attribute zu erweitern. Weitere Informationen finden Sie unter [Konfigurieren der Synchronisierung mit benutzerdefinierten Attributen](synchronization-configure-with-custom-target-attributes.md) und [Synchronisierung mit Erweiterung Verzeichnisattributen konfigurieren](synchronization-configure-with-directory-extension-attributes.md).

Verzeichnis Definitionen werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung    |
|:--------------|:----------|:---------------|
|id           |Zeichenfolge     |Directory-Bezeichner. Lässt keine Nullwerte zu.|
|Metadaten       |MetadataEntry-Auflistung    |Zusätzliche Erweiterungseigenschaften. Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.|
|name           |Zeichenfolge     |Der Name des Verzeichnisses. Muss innerhalb der [Synchronisierungsschema](synchronization-synchronizationschema.md)eindeutig sein. Lässt keine Nullwerte zu.|
|Objekte        |[sind](synchronization-objectdefinition.md) -Auflistung    |Auflistung von Objekten, die durch das Verzeichnis unterstützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "id": "String",
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}]
}

```

## <a name="json-example"></a>Beispiel von JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
    "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
    "name": "salesforce.com",
    "objects": [
        {
            "attributes": [
                {
                    "anchor": true,
                    "name": "Id",
                    "type": "String"
                },
                {
                    "name": "IsActive",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "mutability": "ReadWrite",
                    "name": "Alias",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "CompanyName",
                    "type": "String"
                },
                {
                    "name": "CommunityNickname",
                    "type": "String"
                },
                {
                    "name": "Email",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "EmailEncodingKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LanguageLocaleKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "FirstName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LastName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "LocaleSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "metadata": [
                        {
                            "key": "LinkTypeName",
                            "value": "PermissionSetAssignment"
                        },
                        {
                            "key": "LinkPropertyNames",
                            "value": "[\"PermissionSetId\"]"
                        }
                    ],
                    "name": "PermissionSets",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "PermissionSet"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "ProfileId",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ProfileName",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "TimeZoneSidKey",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "Username",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "UserPermissionsCallCenterAutoLogin",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "UserPermissionsMarketingUser",
                    "required": true,
                    "type": "Boolean"
                },
                {
                    "name": "Street",
                    "type": "String"
                },
                {
                    "name": "City",
                    "type": "String"
                },
                {
                    "name": "Division",
                    "type": "String"
                },
                {
                    "name": "EmployeeNumber",
                    "type": "String"
                },
                {
                    "name": "State",
                    "type": "String"
                },
                {
                    "name": "PostalCode",
                    "type": "String"
                },
                {
                    "name": "Country",
                    "type": "String"
                },
                {
                    "name": "Department",
                    "type": "String"
                },
                {
                    "name": "MobilePhone",
                    "type": "String"
                },
                {
                    "name": "Phone",
                    "type": "String"
                },
                {
                    "name": "Title",
                    "type": "String"
                },
                {
                    "name": "FederationIdentifier",
                    "required": true,
                    "type": "String"
                },
                {
                    "name": "ManagerId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "User"
                        }
                    ],
                    "type": "Reference"
                },
                {
                    "name": "UserRoleId",
                    "referencedObjects": [
                        {
                            "referencedObjectName": "UserRole"
                        }
                    ],
                    "type": "Reference"
                }
            ],
            "metadata": [
                {
                    "key": "IsSoftDeletionSupported",
                    "value": "false"
                },
                {
                    "key": "ConnectorDataStorageRequired",
                    "value": "false"
                },
                {
                    "key": "IsSynchronizeAllSupported",
                    "value": "false"
                }
            ],
            "name": "User"
        }
    ],
    "metadata": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
