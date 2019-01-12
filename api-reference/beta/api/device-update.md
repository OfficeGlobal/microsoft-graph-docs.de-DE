---
title: Gerät aktualisieren
description: Aktualisieren Sie die Eigenschaften eines Geräts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42471e32eac050b84e36477c1cd48fd06feb4244
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916376"
---
# <a name="update-device"></a><span data-ttu-id="07c8a-103">Gerät aktualisieren</span><span class="sxs-lookup"><span data-stu-id="07c8a-103">Update device</span></span>

> <span data-ttu-id="07c8a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="07c8a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07c8a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="07c8a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="07c8a-106">Aktualisieren Sie die Eigenschaften eines Geräts.</span><span class="sxs-lookup"><span data-stu-id="07c8a-106">Update the properties of a device.</span></span>

<span data-ttu-id="07c8a-107">Nur bestimmte Eigenschaften eines Geräts können über genehmigte Geräteverwaltungs-App (Mobile Device Management, MDM) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="07c8a-107">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c8a-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="07c8a-108">Permissions</span></span>
<span data-ttu-id="07c8a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c8a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="07c8a-111">Permission type</span></span>      | <span data-ttu-id="07c8a-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="07c8a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07c8a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="07c8a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07c8a-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07c8a-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="07c8a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="07c8a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c8a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07c8a-116">Not supported.</span></span> |
|<span data-ttu-id="07c8a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="07c8a-117">Application</span></span> | <span data-ttu-id="07c8a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="07c8a-118">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="07c8a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="07c8a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```

> <span data-ttu-id="07c8a-120">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="07c8a-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07c8a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="07c8a-121">Request headers</span></span>
| <span data-ttu-id="07c8a-122">Name</span><span class="sxs-lookup"><span data-stu-id="07c8a-122">Name</span></span>       | <span data-ttu-id="07c8a-123">Typ</span><span class="sxs-lookup"><span data-stu-id="07c8a-123">Type</span></span> | <span data-ttu-id="07c8a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07c8a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="07c8a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c8a-125">Authorization</span></span>  | <span data-ttu-id="07c8a-126">string</span><span class="sxs-lookup"><span data-stu-id="07c8a-126">string</span></span>  | <span data-ttu-id="07c8a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="07c8a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c8a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="07c8a-129">Request body</span></span>

<span data-ttu-id="07c8a-130">Geben Sie im Anforderungstext die Werte für die Eigenschaften des [device](../resources/device.md)-Objekts an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="07c8a-130">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="07c8a-131">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="07c8a-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07c8a-132">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="07c8a-132">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07c8a-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="07c8a-133">Property</span></span>     | <span data-ttu-id="07c8a-134">Typ</span><span class="sxs-lookup"><span data-stu-id="07c8a-134">Type</span></span>   |<span data-ttu-id="07c8a-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="07c8a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07c8a-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="07c8a-136">accountEnabled</span></span>|<span data-ttu-id="07c8a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="07c8a-137">Boolean</span></span>| <span data-ttu-id="07c8a-138">**true**, wenn das Konto aktiviert ist; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="07c8a-138">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="07c8a-139">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="07c8a-139">operatingSystem</span></span>|<span data-ttu-id="07c8a-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07c8a-140">String</span></span>|<span data-ttu-id="07c8a-141">Der Typ des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="07c8a-141">The type of operating system on the device.</span></span>|
|<span data-ttu-id="07c8a-142">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="07c8a-142">operatingSystemVersion</span></span>|<span data-ttu-id="07c8a-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07c8a-143">String</span></span>|<span data-ttu-id="07c8a-144">Die Version des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="07c8a-144">The version of the operating system on the device</span></span>|
|<span data-ttu-id="07c8a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="07c8a-145">displayName</span></span>|<span data-ttu-id="07c8a-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="07c8a-146">String</span></span>|<span data-ttu-id="07c8a-147">Der Anzeigename für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="07c8a-147">The display name for the device.</span></span>|
|<span data-ttu-id="07c8a-148">isCompliant</span><span class="sxs-lookup"><span data-stu-id="07c8a-148">isCompliant</span></span>|<span data-ttu-id="07c8a-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="07c8a-149">Boolean</span></span>|<span data-ttu-id="07c8a-150">**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="07c8a-150">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="07c8a-151">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="07c8a-151">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="07c8a-152">isManaged</span><span class="sxs-lookup"><span data-stu-id="07c8a-152">isManaged</span></span>|<span data-ttu-id="07c8a-153">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="07c8a-153">Boolean</span></span>|<span data-ttu-id="07c8a-154">**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="07c8a-154">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="07c8a-155">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="07c8a-155">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

<span data-ttu-id="07c8a-156">Da die Ressource **Gerät** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **Gerät** .</span><span class="sxs-lookup"><span data-stu-id="07c8a-156">Since the **device** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **device** instance.</span></span>

## <a name="response"></a><span data-ttu-id="07c8a-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="07c8a-157">Response</span></span>

<span data-ttu-id="07c8a-158">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="07c8a-158">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="07c8a-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="07c8a-159">Example</span></span>

##### <a name="request"></a><span data-ttu-id="07c8a-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="07c8a-160">Request</span></span>

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
##### <a name="response"></a><span data-ttu-id="07c8a-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="07c8a-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="07c8a-162">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="07c8a-162">See also</span></span>

- [<span data-ttu-id="07c8a-163">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="07c8a-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="07c8a-164">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="07c8a-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="07c8a-165">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="07c8a-165">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
