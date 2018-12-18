---
title: Gerät aktualisieren
description: Aktualisieren Sie die Eigenschaften eines Geräts.
author: tfitzmac
ms.openlocfilehash: df86581c1edb531e822204698486358fac29f106
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356560"
---
# <a name="update-device"></a><span data-ttu-id="b3c62-103">Gerät aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b3c62-103">Update device</span></span>

> <span data-ttu-id="b3c62-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3c62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3c62-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3c62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3c62-106">Aktualisieren Sie die Eigenschaften eines Geräts.</span><span class="sxs-lookup"><span data-stu-id="b3c62-106">Update the properties of a device.</span></span>

<span data-ttu-id="b3c62-107">Nur bestimmte Eigenschaften eines Geräts können über genehmigte Geräteverwaltungs-App (Mobile Device Management, MDM) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b3c62-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3c62-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b3c62-108">Permissions</span></span>
<span data-ttu-id="b3c62-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3c62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3c62-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3c62-111">Permission type</span></span>      | <span data-ttu-id="b3c62-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3c62-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3c62-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3c62-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3c62-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3c62-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b3c62-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3c62-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c62-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3c62-116">Not supported.</span></span> |
|<span data-ttu-id="b3c62-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3c62-117">Application</span></span> | <span data-ttu-id="b3c62-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3c62-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3c62-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3c62-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="b3c62-120">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="b3c62-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3c62-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3c62-121">Request headers</span></span>
| <span data-ttu-id="b3c62-122">Name</span><span class="sxs-lookup"><span data-stu-id="b3c62-122">Name</span></span>       | <span data-ttu-id="b3c62-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b3c62-123">Type</span></span> | <span data-ttu-id="b3c62-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3c62-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b3c62-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b3c62-125">Authorization</span></span>  | <span data-ttu-id="b3c62-126">string</span><span class="sxs-lookup"><span data-stu-id="b3c62-126">string</span></span>  | <span data-ttu-id="b3c62-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b3c62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3c62-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3c62-129">Request body</span></span>

<span data-ttu-id="b3c62-130">Geben Sie im Anforderungstext die Werte für die Eigenschaften des [device](../resources/device.md)-Objekts an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b3c62-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="b3c62-131">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="b3c62-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b3c62-132">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="b3c62-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b3c62-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3c62-133">Property</span></span>     | <span data-ttu-id="b3c62-134">Typ</span><span class="sxs-lookup"><span data-stu-id="b3c62-134">Type</span></span>   |<span data-ttu-id="b3c62-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3c62-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3c62-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="b3c62-136">accountEnabled</span></span>|<span data-ttu-id="b3c62-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3c62-137">Boolean</span></span>| <span data-ttu-id="b3c62-138">**true**, wenn das Konto aktiviert ist; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="b3c62-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="b3c62-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b3c62-139">operatingSystem</span></span>|<span data-ttu-id="b3c62-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3c62-140">String</span></span>|<span data-ttu-id="b3c62-141">Der Typ des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="b3c62-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="b3c62-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="b3c62-142">operatingSystemVersion</span></span>|<span data-ttu-id="b3c62-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3c62-143">String</span></span>|<span data-ttu-id="b3c62-144">Die Version des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="b3c62-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="b3c62-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b3c62-145">displayName</span></span>|<span data-ttu-id="b3c62-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b3c62-146">String</span></span>|<span data-ttu-id="b3c62-147">Der Anzeigename für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="b3c62-147">The display name for the device.</span></span>|
|<span data-ttu-id="b3c62-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="b3c62-148">isCompliant</span></span>|<span data-ttu-id="b3c62-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3c62-149">Boolean</span></span>|<span data-ttu-id="b3c62-150">**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="b3c62-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="b3c62-151">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b3c62-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="b3c62-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="b3c62-152">isManaged</span></span>|<span data-ttu-id="b3c62-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b3c62-153">Boolean</span></span>|<span data-ttu-id="b3c62-154">**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="b3c62-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="b3c62-155">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="b3c62-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="b3c62-156">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **Gerät** .</span><span class="sxs-lookup"><span data-stu-id="b3c62-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b3c62-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3c62-157">Response</span></span>

<span data-ttu-id="b3c62-158">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3c62-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b3c62-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3c62-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3c62-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3c62-160">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="b3c62-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3c62-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="b3c62-162">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="b3c62-162">See also</span></span>

- [<span data-ttu-id="b3c62-163">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="b3c62-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b3c62-164">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="b3c62-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="b3c62-165">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="b3c62-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
