---
title: Benutzer aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Benutzerobjekts aktualisieren.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 455a3e0c68fadc9768c434f5893dbc950a371bab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922522"
---
# <a name="update-user"></a><span data-ttu-id="8abc5-103">Benutzer aktualisieren</span><span class="sxs-lookup"><span data-stu-id="8abc5-103">Update user</span></span>

> <span data-ttu-id="8abc5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8abc5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8abc5-105">Aktualisieren der Eigenschaften eines [user](../resources/intune-shared-user.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8abc5-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8abc5-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8abc5-106">Prerequisites</span></span>
<span data-ttu-id="8abc5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8abc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8abc5-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8abc5-109">Permission type</span></span>|<span data-ttu-id="8abc5-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8abc5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8abc5-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8abc5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8abc5-112">_variiert je nach Kontext_</span><span class="sxs-lookup"><span data-stu-id="8abc5-112">_varies by context_</span></span>|
| <span data-ttu-id="8abc5-113">&nbsp;&nbsp; Gerätemanagement</span><span class="sxs-lookup"><span data-stu-id="8abc5-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="8abc5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="8abc5-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="8abc5-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="8abc5-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc5-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="8abc5-117">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="8abc5-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="8abc5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8abc5-119">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="8abc5-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="8abc5-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc5-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="8abc5-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8abc5-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8abc5-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8abc5-122">Not supported.</span></span>|
|<span data-ttu-id="8abc5-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8abc5-123">Application</span></span>|<span data-ttu-id="8abc5-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8abc5-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8abc5-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8abc5-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="8abc5-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8abc5-126">Request headers</span></span>
|<span data-ttu-id="8abc5-127">Header</span><span class="sxs-lookup"><span data-stu-id="8abc5-127">Header</span></span>|<span data-ttu-id="8abc5-128">Wert</span><span class="sxs-lookup"><span data-stu-id="8abc5-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8abc5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8abc5-129">Authorization</span></span>|<span data-ttu-id="8abc5-130">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8abc5-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8abc5-131">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8abc5-131">Accept</span></span>|<span data-ttu-id="8abc5-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8abc5-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8abc5-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8abc5-133">Request body</span></span>
<span data-ttu-id="8abc5-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/intune-shared-user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="8abc5-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="8abc5-135">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen des [user](../resources/intune-shared-user.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="8abc5-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="8abc5-136">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8abc5-136">Property</span></span>|<span data-ttu-id="8abc5-137">Typ</span><span class="sxs-lookup"><span data-stu-id="8abc5-137">Type</span></span>|<span data-ttu-id="8abc5-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8abc5-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8abc5-139">id</span><span class="sxs-lookup"><span data-stu-id="8abc5-139">id</span></span>|<span data-ttu-id="8abc5-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8abc5-140">String</span></span>|<span data-ttu-id="8abc5-141">Eindeutiger Bezeichner des Benutzers</span><span class="sxs-lookup"><span data-stu-id="8abc5-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="8abc5-142">**Onboarding**</span><span class="sxs-lookup"><span data-stu-id="8abc5-142">**Onboarding**</span></span>|
|<span data-ttu-id="8abc5-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="8abc5-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="8abc5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8abc5-144">Int32</span></span>|<span data-ttu-id="8abc5-145">Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann.</span><span class="sxs-lookup"><span data-stu-id="8abc5-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="8abc5-146">Zulässige Werte sind 5 oder 1000.</span><span class="sxs-lookup"><span data-stu-id="8abc5-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="8abc5-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="8abc5-147">Response</span></span>
<span data-ttu-id="8abc5-148">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [user](../resources/intune-shared-user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8abc5-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8abc5-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8abc5-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8abc5-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8abc5-150">Request</span></span>
<span data-ttu-id="8abc5-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8abc5-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="8abc5-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="8abc5-152">Response</span></span>
<span data-ttu-id="8abc5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8abc5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



