---
title: Erstellen einer Einstellung directory
description: Verwenden Sie diese API, um eine neue Einstellung, basierend auf den in DirectorySettingTemplates verfügbaren Vorlagen erstellen. Diese Einstellungen kann die Mandanten-Ebene oder auf Objektebene (derzeit nur für Gruppen). Die Anforderung zum Erstellen eines muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben. Für die Gruppe-spezifischen Einstellungen kann die Option nur die Einstellung steuern, ob Mitglieder einer Gruppe Gastbenutzer einladen können festgelegt werden. Dies wird dieses Verhalten gesteuert, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe im Allgemeinen verfügbar ist.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f74c449f02726adc4ba0993f450a8a4351ec8f2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520753"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="3443a-107">Erstellen einer Einstellung directory</span><span class="sxs-lookup"><span data-stu-id="3443a-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3443a-108">Verwenden Sie diese API, um eine neue Einstellung, basierend auf den in DirectorySettingTemplates verfügbaren Vorlagen erstellen.</span><span class="sxs-lookup"><span data-stu-id="3443a-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="3443a-109">Diese Einstellungen kann die Mandanten-Ebene oder auf Objektebene (derzeit nur für Gruppen).</span><span class="sxs-lookup"><span data-stu-id="3443a-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="3443a-110">Die Anforderung zum Erstellen eines muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben.</span><span class="sxs-lookup"><span data-stu-id="3443a-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="3443a-111">Für die Gruppe-spezifischen Einstellungen kann die Option nur die Einstellung steuern, ob Mitglieder einer Gruppe Gastbenutzer einladen können festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3443a-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="3443a-112">Dies wird dieses Verhalten gesteuert, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe im Allgemeinen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="3443a-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="3443a-113">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="3443a-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="3443a-114">Die Version /v1.0 dieser API wurde in *Create GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="3443a-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="3443a-115">Eine Liste der Vorlagen und die Eigenschaften, die sie in der Betaversion unterstützen, verwenden Sie eine [DirectorySettingTemplate Abfrage](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="3443a-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="3443a-116">(Für v1. 0-Endpunkte, rufen Sie [GroupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="3443a-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="3443a-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3443a-117">Permissions</span></span>
<span data-ttu-id="3443a-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3443a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3443a-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3443a-120">Permission type</span></span>      | <span data-ttu-id="3443a-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3443a-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3443a-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3443a-122">Delegated (work or school account)</span></span> | <span data-ttu-id="3443a-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3443a-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3443a-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3443a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3443a-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3443a-125">Not supported.</span></span>    |
|<span data-ttu-id="3443a-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3443a-126">Application</span></span> | <span data-ttu-id="3443a-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3443a-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3443a-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3443a-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="3443a-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3443a-129">Request headers</span></span>
| <span data-ttu-id="3443a-130">Name</span><span class="sxs-lookup"><span data-stu-id="3443a-130">Name</span></span>       | <span data-ttu-id="3443a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3443a-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3443a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="3443a-132">Authorization</span></span>  | <span data-ttu-id="3443a-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3443a-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3443a-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3443a-135">Request body</span></span>
<span data-ttu-id="3443a-136">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3443a-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="3443a-137">Jedoch wird der Anzeigename für die Einstellung basierend auf den Vorlagennamen referenzierten Einstellungen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="3443a-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="3443a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3443a-138">Response</span></span>

<span data-ttu-id="3443a-139">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="3443a-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3443a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3443a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3443a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3443a-141">Request</span></span>
<span data-ttu-id="3443a-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3443a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
<span data-ttu-id="3443a-143">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="3443a-143">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3443a-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3443a-144">Response</span></span>
<span data-ttu-id="3443a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3443a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
