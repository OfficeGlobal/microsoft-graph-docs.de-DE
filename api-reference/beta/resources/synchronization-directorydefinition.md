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
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="08794-105">Ressourcentyp directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="08794-105">directoryDefinition resource type</span></span>

> <span data-ttu-id="08794-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08794-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08794-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08794-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08794-108">Enthält die Synchronisierung Engine ein Verzeichnis und ihre Objekte Informationen.</span><span class="sxs-lookup"><span data-stu-id="08794-108">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="08794-109">Diese Ressource weist dem Synchronisierungsmodul beispielsweise, dass das Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="08794-109">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="08794-110">In der Reihenfolge für das Objekt und das Attribut an [Synchronisierungsregeln](synchronization-synchronizationrule.md) und [Objekt Zuordnungen](synchronization-objectmapping.md)teilzunehmen müssen sie als Teil der Definition der Directory definiert werden.</span><span class="sxs-lookup"><span data-stu-id="08794-110">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="08794-111">Im Allgemeinen wird dem [Synchronisierungsschema](synchronization-synchronizationschema.md) als Teil der [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md) bereitgestellt am häufigsten verwendeten Objekte und Attribute für dieses Verzeichnis definieren.</span><span class="sxs-lookup"><span data-stu-id="08794-111">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="08794-112">Wenn das Verzeichnis, das Hinzufügen von benutzerdefinierten Attributen unterstützt, sollten Sie die Standarddefinition durch eigene benutzerdefinierte Objekte oder Attribute zu erweitern.</span><span class="sxs-lookup"><span data-stu-id="08794-112">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="08794-113">Weitere Informationen finden Sie unter [Konfigurieren der Synchronisierung mit benutzerdefinierten Attributen](synchronization-configure-with-custom-target-attributes.md) und [Synchronisierung mit Erweiterung Verzeichnisattributen konfigurieren](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="08794-113">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="08794-114">Verzeichnis Definitionen werden als Teil der [Synchronisierungsschema](synchronization-synchronizationschema.md)aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="08794-114">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="08794-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08794-115">Properties</span></span>

| <span data-ttu-id="08794-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08794-116">Property</span></span>      | <span data-ttu-id="08794-117">Typ</span><span class="sxs-lookup"><span data-stu-id="08794-117">Type</span></span>      | <span data-ttu-id="08794-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08794-118">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="08794-119">id</span><span class="sxs-lookup"><span data-stu-id="08794-119">id</span></span>           |<span data-ttu-id="08794-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08794-120">String</span></span>     |<span data-ttu-id="08794-121">Directory-Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="08794-121">Directory identifier.</span></span> <span data-ttu-id="08794-122">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="08794-122">Not nullable.</span></span>|
|<span data-ttu-id="08794-123">Metadaten</span><span class="sxs-lookup"><span data-stu-id="08794-123">metadata</span></span>       |<span data-ttu-id="08794-124">MetadataEntry-Auflistung</span><span class="sxs-lookup"><span data-stu-id="08794-124">metadataEntry collection</span></span>    |<span data-ttu-id="08794-125">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="08794-125">Additional extension properties.</span></span> <span data-ttu-id="08794-126">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="08794-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="08794-127">name</span><span class="sxs-lookup"><span data-stu-id="08794-127">name</span></span>           |<span data-ttu-id="08794-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08794-128">String</span></span>     |<span data-ttu-id="08794-129">Der Name des Verzeichnisses.</span><span class="sxs-lookup"><span data-stu-id="08794-129">Name of the directory.</span></span> <span data-ttu-id="08794-130">Muss innerhalb der [Synchronisierungsschema](synchronization-synchronizationschema.md)eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="08794-130">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="08794-131">Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="08794-131">Not nullable.</span></span>|
|<span data-ttu-id="08794-132">Objekte</span><span class="sxs-lookup"><span data-stu-id="08794-132">objects</span></span>        |<span data-ttu-id="08794-133">[sind](synchronization-objectdefinition.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="08794-133">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="08794-134">Auflistung von Objekten, die durch das Verzeichnis unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08794-134">Collection of objects supported by the directory.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08794-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08794-135">JSON representation</span></span>

<span data-ttu-id="08794-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08794-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-example"></a><span data-ttu-id="08794-137">Beispiel von JSON</span><span class="sxs-lookup"><span data-stu-id="08794-137">JSON Example</span></span>

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
