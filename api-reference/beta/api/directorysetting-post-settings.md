---
title: Erstellen einer Einstellung directory
description: Verwenden Sie diese API, um eine neue Einstellung, basierend auf den in DirectorySettingTemplates verfügbaren Vorlagen erstellen. Diese Einstellungen kann die Mandanten-Ebene oder auf Objektebene (derzeit nur für Gruppen). Die Anforderung zum Erstellen eines muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben. Für die Gruppe-spezifischen Einstellungen kann die Option nur die Einstellung steuern, ob Mitglieder einer Gruppe Gastbenutzer einladen können festgelegt werden. Dies wird dieses Verhalten gesteuert, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe im Allgemeinen verfügbar ist.
ms.openlocfilehash: 40e90f66c43032deea8ee866b13508fd73c0f17f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060571"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="37e23-107">Erstellen einer Einstellung directory</span><span class="sxs-lookup"><span data-stu-id="37e23-107">Create a directory setting</span></span>

> <span data-ttu-id="37e23-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="37e23-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37e23-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37e23-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37e23-110">Verwenden Sie diese API, um eine neue Einstellung, basierend auf den in DirectorySettingTemplates verfügbaren Vorlagen erstellen.</span><span class="sxs-lookup"><span data-stu-id="37e23-110">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="37e23-111">Diese Einstellungen kann die Mandanten-Ebene oder auf Objektebene (derzeit nur für Gruppen).</span><span class="sxs-lookup"><span data-stu-id="37e23-111">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="37e23-112">Die Anforderung zum Erstellen eines muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben.</span><span class="sxs-lookup"><span data-stu-id="37e23-112">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="37e23-113">Für die Gruppe-spezifischen Einstellungen kann die Option nur die Einstellung steuern, ob Mitglieder einer Gruppe Gastbenutzer einladen können festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="37e23-113">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="37e23-114">Dies wird dieses Verhalten gesteuert, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe im Allgemeinen verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="37e23-114">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="37e23-115">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="37e23-115">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="37e23-116">Die Version /v1.0 dieser API wurde in *Create GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="37e23-116">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="37e23-117">Eine Liste der Vorlagen und die Eigenschaften, die sie in der Betaversion unterstützen, verwenden Sie eine [DirectorySettingTemplate Abfrage](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="37e23-117">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="37e23-118">(Für v1. 0-Endpunkte, rufen Sie [GroupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="37e23-118">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="37e23-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="37e23-119">Permissions</span></span>
<span data-ttu-id="37e23-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e23-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e23-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37e23-122">Permission type</span></span>      | <span data-ttu-id="37e23-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37e23-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37e23-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37e23-124">Delegated (work or school account)</span></span> | <span data-ttu-id="37e23-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37e23-125">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37e23-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37e23-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37e23-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37e23-127">Not supported.</span></span>    |
|<span data-ttu-id="37e23-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37e23-128">Application</span></span> | <span data-ttu-id="37e23-129">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e23-129">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37e23-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37e23-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="37e23-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37e23-131">Request headers</span></span>
| <span data-ttu-id="37e23-132">Name</span><span class="sxs-lookup"><span data-stu-id="37e23-132">Name</span></span>       | <span data-ttu-id="37e23-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37e23-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="37e23-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="37e23-134">Authorization</span></span>  | <span data-ttu-id="37e23-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="37e23-p107">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37e23-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37e23-137">Request body</span></span>
<span data-ttu-id="37e23-138">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37e23-138">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="37e23-139">Jedoch wird der Anzeigename für die Einstellung basierend auf den Vorlagennamen referenzierten Einstellungen festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="37e23-139">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="37e23-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="37e23-140">Response</span></span>

<span data-ttu-id="37e23-141">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="37e23-141">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37e23-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37e23-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37e23-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37e23-143">Request</span></span>
<span data-ttu-id="37e23-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37e23-144">Here is an example of the request.</span></span>
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
<span data-ttu-id="37e23-145">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="37e23-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="37e23-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="37e23-146">Response</span></span>
<span data-ttu-id="37e23-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37e23-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->