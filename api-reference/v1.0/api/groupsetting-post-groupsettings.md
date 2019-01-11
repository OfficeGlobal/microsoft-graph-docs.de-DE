---
title: Erstellen einer Gruppeneinstellung
description: Verwenden Sie diese API zum Erstellen einer neuen Einstellung, basierend auf den Vorlagen, die in groupSettingTemplates zur Verfügung stehen. Diese Einstellungen können auf Mandantenebene oder auf Gruppenebene erfolgen. Die Erstellungsanforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. Bei gruppenspezifischen Einstellungen kann nur die Einstellung, die regelt, ob die Mitglieder einer Gruppe Gastbenutzer einladen können, festgelegt werden. Dies steuert dieses Verhalten, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe allgemein verfügbar ist.
localization_priority: Normal
ms.openlocfilehash: c5ba428380e6503f8d54682709d36e12b7ff4de3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894537"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="ae545-107">Erstellen einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="ae545-107">Create a group setting</span></span>

<span data-ttu-id="ae545-p102">Verwenden Sie diese API zum Erstellen einer neuen Einstellung, basierend auf den Vorlagen, die in [groupSettingTemplates](../resources/groupsettingtemplate.md) zur Verfügung stehen. Diese Einstellungen können auf Mandantenebene oder auf Gruppenebene erfolgen. Die Erstellungsanforderung muss [settingValues](../resources/settingvalue.md) für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. Bei gruppenspezifischen Einstellungen kann nur die Einstellung, die regelt, ob die Mitglieder einer Gruppe Gastbenutzer einladen können, festgelegt werden. Dies steuert dieses Verhalten, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe allgemein verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ae545-p102">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="ae545-113">Verwenden Sie eine Liste der Vorlagen und die Eigenschaften, die sie in v1. 0 unterstützen, einer [GroupSettingTemplate Abfrage](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0) (für Beta Endpunkte, Anruf [DirectorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span><span class="sxs-lookup"><span data-stu-id="ae545-113">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="ae545-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ae545-114">Permissions</span></span>

<span data-ttu-id="ae545-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae545-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae545-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae545-117">Permission type</span></span>      | <span data-ttu-id="ae545-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae545-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae545-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae545-119">Delegated (work or school account)</span></span> | <span data-ttu-id="ae545-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae545-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae545-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae545-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae545-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae545-122">Not supported.</span></span>    |
|<span data-ttu-id="ae545-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae545-123">Application</span></span> | <span data-ttu-id="ae545-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae545-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae545-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae545-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="ae545-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae545-126">Request headers</span></span>

| <span data-ttu-id="ae545-127">Name</span><span class="sxs-lookup"><span data-stu-id="ae545-127">Name</span></span> | <span data-ttu-id="ae545-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae545-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ae545-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae545-129">Authorization</span></span> | <span data-ttu-id="ae545-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae545-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae545-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae545-132">Content-Type</span></span> | <span data-ttu-id="ae545-133">application/json</span><span class="sxs-lookup"><span data-stu-id="ae545-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae545-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae545-134">Request body</span></span>
<span data-ttu-id="ae545-p105">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupSetting](../resources/groupsetting.md)-Objekts an. Der Anzeigenamen für die Einstellung wird jedoch basierend auf dem Namen der referenzierten Einstellungsvorlage festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ae545-p105">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="ae545-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae545-137">Response</span></span>

<span data-ttu-id="ae545-138">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `201 Created` und das [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ae545-138">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae545-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae545-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ae545-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae545-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
<span data-ttu-id="ae545-141">Geben Sie im Anforderungstext eine JSON-Darstellung des [groupSetting](../resources/groupsetting.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ae545-141">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ae545-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae545-142">Response</span></span>

<span data-ttu-id="ae545-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae545-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
