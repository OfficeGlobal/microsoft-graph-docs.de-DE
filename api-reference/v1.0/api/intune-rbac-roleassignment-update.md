---
title: roleAssignment aktualisieren
description: Aktualisieren der Eigenschaften eines roleAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: edcfa7d06cbe4348835109c2adc3a48d9f24fe7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816212"
---
# <a name="update-roleassignment"></a><span data-ttu-id="c1d21-103">roleAssignment aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c1d21-103">Update roleAssignment</span></span>

> <span data-ttu-id="c1d21-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1d21-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1d21-105">Aktualisieren der Eigenschaften eines [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c1d21-105">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c1d21-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1d21-106">Prerequisites</span></span>
<span data-ttu-id="c1d21-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d21-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1d21-109">Permission type</span></span>|<span data-ttu-id="c1d21-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1d21-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1d21-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1d21-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1d21-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1d21-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c1d21-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1d21-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1d21-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d21-114">Not supported.</span></span>|
|<span data-ttu-id="c1d21-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1d21-115">Application</span></span>|<span data-ttu-id="c1d21-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1d21-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1d21-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d21-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1d21-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1d21-118">Request headers</span></span>
|<span data-ttu-id="c1d21-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1d21-119">Header</span></span>|<span data-ttu-id="c1d21-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c1d21-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1d21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1d21-121">Authorization</span></span>|<span data-ttu-id="c1d21-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1d21-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1d21-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1d21-123">Accept</span></span>|<span data-ttu-id="c1d21-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1d21-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d21-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1d21-125">Request body</span></span>
<span data-ttu-id="c1d21-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="c1d21-126">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="c1d21-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleAssignment](../resources/intune-rbac-roleassignment.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c1d21-127">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="c1d21-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c1d21-128">Property</span></span>|<span data-ttu-id="c1d21-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c1d21-129">Type</span></span>|<span data-ttu-id="c1d21-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1d21-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1d21-131">id</span><span class="sxs-lookup"><span data-stu-id="c1d21-131">id</span></span>|<span data-ttu-id="c1d21-132">String</span><span class="sxs-lookup"><span data-stu-id="c1d21-132">String</span></span>|<span data-ttu-id="c1d21-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c1d21-133">Key of the entity.</span></span> <span data-ttu-id="c1d21-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="c1d21-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c1d21-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c1d21-135">displayName</span></span>|<span data-ttu-id="c1d21-136">String</span><span class="sxs-lookup"><span data-stu-id="c1d21-136">String</span></span>|<span data-ttu-id="c1d21-137">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="c1d21-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="c1d21-138">description</span><span class="sxs-lookup"><span data-stu-id="c1d21-138">description</span></span>|<span data-ttu-id="c1d21-139">String</span><span class="sxs-lookup"><span data-stu-id="c1d21-139">String</span></span>|<span data-ttu-id="c1d21-140">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="c1d21-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="c1d21-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="c1d21-141">resourceScopes</span></span>|<span data-ttu-id="c1d21-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c1d21-142">String collection</span></span>|<span data-ttu-id="c1d21-143">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="c1d21-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="c1d21-144">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1d21-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="c1d21-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d21-145">Response</span></span>
<span data-ttu-id="c1d21-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1d21-146">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1d21-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1d21-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1d21-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1d21-148">Request</span></span>
<span data-ttu-id="c1d21-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1d21-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c1d21-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1d21-150">Response</span></span>
<span data-ttu-id="c1d21-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1d21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



