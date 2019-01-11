---
title: Aktualisieren einer Gruppeneinstellung
description: Mit dieser API können Sie die Eigenschaften des jeweils angegebenen Gruppeneinstellungsobjekts aktualisieren.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: a1b677e9d1a00dc01aaf2455ac075fe20cbe4d1b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804956"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="61793-103">Aktualisieren einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="61793-103">Update a group setting</span></span>

<span data-ttu-id="61793-104">Mit dieser API können Sie die Eigenschaften des jeweils angegebenen Gruppeneinstellungsobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="61793-104">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="61793-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="61793-105">Permissions</span></span>

<span data-ttu-id="61793-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="61793-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="61793-108">Permission type</span></span>      | <span data-ttu-id="61793-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="61793-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61793-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="61793-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61793-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61793-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61793-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="61793-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61793-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="61793-113">Not supported.</span></span>    |
|<span data-ttu-id="61793-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="61793-114">Application</span></span> | <span data-ttu-id="61793-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61793-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61793-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="61793-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="61793-117">Aktualisiert eine mandantenweite oder gruppenspezifische Einstellung.</span><span class="sxs-lookup"><span data-stu-id="61793-117">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="61793-118">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="61793-118">Optional request headers</span></span>
| <span data-ttu-id="61793-119">Name</span><span class="sxs-lookup"><span data-stu-id="61793-119">Name</span></span> | <span data-ttu-id="61793-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61793-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="61793-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="61793-121">Authorization</span></span>  | <span data-ttu-id="61793-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="61793-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="61793-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61793-124">Content-Type</span></span>  | <span data-ttu-id="61793-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61793-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61793-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="61793-126">Request body</span></span>
<span data-ttu-id="61793-127">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="61793-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="61793-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61793-128">Property</span></span> | <span data-ttu-id="61793-129">Typ</span><span class="sxs-lookup"><span data-stu-id="61793-129">Type</span></span> | <span data-ttu-id="61793-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61793-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="61793-131">values</span><span class="sxs-lookup"><span data-stu-id="61793-131">values</span></span> | <span data-ttu-id="61793-132">settingValue-Sammlung</span><span class="sxs-lookup"><span data-stu-id="61793-132">settingValue collection</span></span> | <span data-ttu-id="61793-p103">Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="61793-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="61793-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="61793-136">Response</span></span>

<span data-ttu-id="61793-137">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="61793-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="61793-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="61793-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="61793-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="61793-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "True"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="61793-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="61793-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
