---
title: Gerät aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines registrierten Geräts aktualisieren.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f24372e122045eee9d79cde6334038f0dc1ccddf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962233"
---
# <a name="update-device"></a><span data-ttu-id="0e386-103">Gerät aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0e386-103">Update device</span></span>

<span data-ttu-id="0e386-104">Mit dieser API können Sie die Eigenschaften eines registrierten Geräts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="0e386-104">Update the properties of a registered device.</span></span>

<span data-ttu-id="0e386-105">Nur bestimmte Eigenschaften eines Geräts können über genehmigte Geräteverwaltungs-App (Mobile Device Management, MDM) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="0e386-105">Only certain properties of a device can be updated through approved Mobile Device Managment (MDM) apps.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e386-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e386-106">Permissions</span></span>
<span data-ttu-id="0e386-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e386-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e386-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e386-109">Permission type</span></span>      | <span data-ttu-id="0e386-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e386-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e386-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e386-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e386-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e386-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0e386-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e386-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e386-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e386-114">Not supported.</span></span> |
|<span data-ttu-id="0e386-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e386-115">Application</span></span> | <span data-ttu-id="0e386-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e386-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e386-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e386-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> <span data-ttu-id="0e386-118">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="0e386-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e386-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e386-119">Request headers</span></span>
| <span data-ttu-id="0e386-120">Name</span><span class="sxs-lookup"><span data-stu-id="0e386-120">Name</span></span>       | <span data-ttu-id="0e386-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0e386-121">Type</span></span> | <span data-ttu-id="0e386-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e386-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e386-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e386-123">Authorization</span></span>  | <span data-ttu-id="0e386-124">string</span><span class="sxs-lookup"><span data-stu-id="0e386-124">string</span></span>  | <span data-ttu-id="0e386-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e386-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e386-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e386-127">Request body</span></span>

<span data-ttu-id="0e386-128">Geben Sie im Anforderungstext die Werte für die Eigenschaften des [device](../resources/device.md)-Objekts an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="0e386-128">In the request body, supply the values for the [device](../resources/device.md) properties that should be updated.</span></span> <span data-ttu-id="0e386-129">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="0e386-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0e386-130">Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0e386-130">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e386-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e386-131">Property</span></span>     | <span data-ttu-id="0e386-132">Typ</span><span class="sxs-lookup"><span data-stu-id="0e386-132">Type</span></span>   |<span data-ttu-id="0e386-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e386-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e386-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="0e386-134">accountEnabled</span></span>|<span data-ttu-id="0e386-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e386-135">Boolean</span></span>| <span data-ttu-id="0e386-136">**true**, wenn das Konto aktiviert ist; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="0e386-136">**true** if the account is enabled; otherwise, **false**.</span></span> |
|<span data-ttu-id="0e386-137">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e386-137">operatingSystem</span></span>|<span data-ttu-id="0e386-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e386-138">String</span></span>|<span data-ttu-id="0e386-139">Der Typ des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="0e386-139">The type of operating system on the device.</span></span>|
|<span data-ttu-id="0e386-140">operatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="0e386-140">operatingSystemVersion</span></span>|<span data-ttu-id="0e386-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e386-141">String</span></span>|<span data-ttu-id="0e386-142">Die Version des Betriebssystems auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="0e386-142">The version of the operating system on the device</span></span>|
|<span data-ttu-id="0e386-143">displayName</span><span class="sxs-lookup"><span data-stu-id="0e386-143">displayName</span></span>|<span data-ttu-id="0e386-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e386-144">String</span></span>|<span data-ttu-id="0e386-145">Der Anzeigename für das Gerät.</span><span class="sxs-lookup"><span data-stu-id="0e386-145">The display name for the device.</span></span>|
|<span data-ttu-id="0e386-146">isCompliant</span><span class="sxs-lookup"><span data-stu-id="0e386-146">isCompliant</span></span>|<span data-ttu-id="0e386-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e386-147">Boolean</span></span>|<span data-ttu-id="0e386-148">**true**, wenn das Gerät den Richtlinien für mobile Geräteverwaltung ( Mobile Device Management, MDM) entspricht; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="0e386-148">**true** if the device complies with Mobile Device Management (MDM) policies; otherwise, **false**.</span></span> <span data-ttu-id="0e386-149">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="0e386-149">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |
|<span data-ttu-id="0e386-150">isManaged</span><span class="sxs-lookup"><span data-stu-id="0e386-150">isManaged</span></span>|<span data-ttu-id="0e386-151">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0e386-151">Boolean</span></span>|<span data-ttu-id="0e386-152">**true**, wenn das Gerät durch die mobile Geräteverwaltungs-App verwaltet wird; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="0e386-152">**true** if the device is managed by a Mobile Device Management (MDM) app; otherwise, **false**.</span></span> <span data-ttu-id="0e386-153">Dies kann nur durch Intune für einen beliebigen Gerätetyp Betriebssystem oder durch eine [genehmigt MDM-app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) für Windows-Betriebssystem Geräte aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="0e386-153">This can only be updated by Intune for any device OS type or by an [approved MDM app](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm) for Windows OS devices.</span></span> |

## <a name="response"></a><span data-ttu-id="0e386-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e386-154">Response</span></span>

<span data-ttu-id="0e386-155">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e386-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e386-156">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e386-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e386-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e386-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

{
  "accountEnabled": false
}
```
##### <a name="response"></a><span data-ttu-id="0e386-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e386-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
HTTP/1.1 204 No Content
```
