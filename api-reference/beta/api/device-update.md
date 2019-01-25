---
title: Gerät aktualisieren
description: Aktualisieren Sie die Eigenschaften eines Geräts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 70c5e6475f32f7e545371064411885d2690e4f0e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520942"
---
# <a name="update-device"></a><span data-ttu-id="bc5df-103">Gerät aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bc5df-103">Update device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc5df-104">Aktualisieren Sie die Eigenschaften eines Geräts.</span><span class="sxs-lookup"><span data-stu-id="bc5df-104">Update the properties of a device.</span></span>

<span data-ttu-id="bc5df-105">Nur bestimmte Eigenschaften eines Geräts können über genehmigte Geräteverwaltungs-App (Mobile Device Management, MDM) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="bc5df-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc5df-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc5df-106">Permissions</span></span>
<span data-ttu-id="bc5df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc5df-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc5df-109">Permission type</span></span>      | <span data-ttu-id="bc5df-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc5df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc5df-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc5df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc5df-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc5df-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="bc5df-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc5df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5df-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc5df-114">Not supported.</span></span> |
|<span data-ttu-id="bc5df-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc5df-115">Application</span></span> | <span data-ttu-id="bc5df-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc5df-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc5df-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc5df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="bc5df-118">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="bc5df-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc5df-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc5df-119">Request headers</span></span>
| <span data-ttu-id="bc5df-120">Name</span><span class="sxs-lookup"><span data-stu-id="bc5df-120">Name</span></span>       | <span data-ttu-id="bc5df-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bc5df-121">Type</span></span> | <span data-ttu-id="bc5df-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc5df-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc5df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc5df-123">Authorization</span></span>  | <span data-ttu-id="bc5df-124">string</span><span class="sxs-lookup"><span data-stu-id="bc5df-124">string</span></span>  | <span data-ttu-id="bc5df-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc5df-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc5df-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc5df-127">Request body</span></span>

<span data-ttu-id="bc5df-128">Geben Sie im Anforderungstext die Werte für die Eigenschaften des [device](../resources/device.md)-Objekts an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="bc5df-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="bc5df-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="bc5df-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bc5df-130">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="bc5df-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc5df-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc5df-131">Property</span></span>     | <span data-ttu-id="bc5df-132">Typ</span><span class="sxs-lookup"><span data-stu-id="bc5df-132">Type</span></span>   |<span data-ttu-id="bc5df-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc5df-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc5df-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="bc5df-134">accountEnabled</span></span>|<span data-ttu-id="bc5df-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bc5df-135">Boolean</span></span>| <span data-ttu-id="bc5df-136">**true**, wenn das Konto aktiviert ist; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="bc5df-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="bc5df-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bc5df-137">operatingSystem</span></span>|<span data-ttu-id="bc5df-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc5df-138">String</span></span>|<span data-ttu-id="bc5df-139">Der Typ des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="bc5df-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="bc5df-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="bc5df-140">operatingSystemVersion</span></span>|<span data-ttu-id="bc5df-141">String</span><span class="sxs-lookup"><span data-stu-id="bc5df-141">String</span></span>|<span data-ttu-id="bc5df-142">Die Version des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="bc5df-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="bc5df-143">displayName</span><span class="sxs-lookup"><span data-stu-id="bc5df-143">displayName</span></span>|<span data-ttu-id="bc5df-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc5df-144">String</span></span>|<span data-ttu-id="bc5df-145">Der Anzeigename für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="bc5df-145">The display name for the device.</span></span>|
|<span data-ttu-id="bc5df-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="bc5df-146">isCompliant</span></span>|<span data-ttu-id="bc5df-147">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bc5df-147">Boolean</span></span>|<span data-ttu-id="bc5df-148">**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="bc5df-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="bc5df-149">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="bc5df-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="bc5df-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="bc5df-150">isManaged</span></span>|<span data-ttu-id="bc5df-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bc5df-151">Boolean</span></span>|<span data-ttu-id="bc5df-152">**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="bc5df-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="bc5df-153">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="bc5df-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="bc5df-154">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **Gerät** .</span><span class="sxs-lookup"><span data-stu-id="bc5df-154">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="bc5df-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc5df-155">Response</span></span>

<span data-ttu-id="bc5df-156">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc5df-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc5df-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc5df-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bc5df-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc5df-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/beta/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="bc5df-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc5df-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="bc5df-160">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="bc5df-160">See also</span></span>

- [<span data-ttu-id="bc5df-161">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="bc5df-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bc5df-162">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="bc5df-162">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bc5df-163">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="bc5df-163">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
