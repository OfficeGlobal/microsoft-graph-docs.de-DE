---
title: Ressourcentyp directoryDefinition
description: Enthält die Synchronisierung Engine ein Verzeichnis und ihre Objekte Informationen. Diese Ressource weist dem Synchronisierungsmodul beispielsweise, dass das Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden. In der Reihenfolge für das Objekt und das Attribut an Synchronisierungsregeln und Objekt Zuordnungen teilzunehmen müssen sie als Teil der Definition der Directory definiert werden.
localization_priority: Normal
ms.openlocfilehash: 22ba4a7f3b5b5d3154ec6b3f5d42bd6f1b8f09d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508125"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="250b7-105">Ressourcentyp directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="250b7-105">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="250b7-106">Enthält die Synchronisierung Engine ein Verzeichnis und ihre Objekte Informationen.</span><span class="sxs-lookup"><span data-stu-id="250b7-106">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="250b7-107">Diese Ressource weist dem Synchronisierungsmodul beispielsweise, dass das Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="250b7-107">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="250b7-108">In der Reihenfolge für das Objekt und das Attribut an [Synchronisierungsregeln](synchronization-synchronizationrule.md) und [Objekt Zuordnungen](synchronization-objectmapping.md)teilzunehmen müssen sie als Teil der Definition der Directory definiert werden.</span><span class="sxs-lookup"><span data-stu-id="250b7-108">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="250b7-109">Im Allgemeinen wird dem [Synchronisierungsschema](synchronization-synchronizationschema.md) als Teil der [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md) bereitgestellt am häufigsten verwendeten Objekte und Attribute für dieses Verzeichnis definieren.</span><span class="sxs-lookup"><span data-stu-id="250b7-109">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="250b7-110">Wenn das Verzeichnis, das Hinzufügen von benutzerdefinierten Attributen unterstützt, sollten Sie die Standarddefinition durch eigene benutzerdefinierte Objekte oder Attribute zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="250b7-110">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="250b7-111">Weitere Informationen finden Sie unter [Konfigurieren der Synchronisierung mit benutzerdefinierten Attributen](synchronization-configure-with-custom-target-attributes.md) und [Synchronisierung mit Erweiterung Verzeichnisattributen konfigurieren](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="250b7-111">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="250b7-112">Verzeichnis Definitionen werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="250b7-112">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="250b7-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="250b7-113">Properties</span></span>

| <span data-ttu-id="250b7-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="250b7-114">Property</span></span>      | <span data-ttu-id="250b7-115">Typ</span><span class="sxs-lookup"><span data-stu-id="250b7-115">Type</span></span>      | <span data-ttu-id="250b7-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="250b7-116">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="250b7-117">id</span><span class="sxs-lookup"><span data-stu-id="250b7-117">id</span></span>           |<span data-ttu-id="250b7-118">String</span><span class="sxs-lookup"><span data-stu-id="250b7-118">String</span></span>     |<span data-ttu-id="250b7-119">Directory-Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="250b7-119">Directory identifier.</span></span> <span data-ttu-id="250b7-120">Lässt keine NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="250b7-120">Not nullable.</span></span>|
|<span data-ttu-id="250b7-121">$metadata</span><span class="sxs-lookup"><span data-stu-id="250b7-121">metadata</span></span>       |<span data-ttu-id="250b7-122">MetadataEntry-Auflistung</span><span class="sxs-lookup"><span data-stu-id="250b7-122">metadataEntry collection</span></span>    |<span data-ttu-id="250b7-123">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="250b7-123">Additional extension properties.</span></span> <span data-ttu-id="250b7-124">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="250b7-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="250b7-125">name</span><span class="sxs-lookup"><span data-stu-id="250b7-125">name</span></span>           |<span data-ttu-id="250b7-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="250b7-126">String</span></span>     |<span data-ttu-id="250b7-127">Der Name des Verzeichnisses.</span><span class="sxs-lookup"><span data-stu-id="250b7-127">Name of the directory.</span></span> <span data-ttu-id="250b7-128">Muss innerhalb der [Synchronisierungsschema](synchronization-synchronizationschema.md)eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="250b7-128">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="250b7-129">Lässt keine NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="250b7-129">Not nullable.</span></span>|
|<span data-ttu-id="250b7-130">Objekte</span><span class="sxs-lookup"><span data-stu-id="250b7-130">objects</span></span>        |<span data-ttu-id="250b7-131">[sind](synchronization-objectdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="250b7-131">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="250b7-132">Auflistung von Objekten, die durch das Verzeichnis unterstützt.</span><span class="sxs-lookup"><span data-stu-id="250b7-132">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="250b7-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="250b7-133">JSON representation</span></span>

<span data-ttu-id="250b7-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="250b7-134">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="250b7-135">Beispiel von JSON</span><span class="sxs-lookup"><span data-stu-id="250b7-135">JSON Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-directorydefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
