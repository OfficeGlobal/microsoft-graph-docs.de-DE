---
title: roleAssignment erstellen
description: Erstellen eines neuen roleAssignment-Objekts.
ms.openlocfilehash: 887e802371c8545baf44bca81da9b79455eb262d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017103"
---
# <a name="create-roleassignment"></a><span data-ttu-id="fb7d3-103">roleAssignment erstellen</span><span class="sxs-lookup"><span data-stu-id="fb7d3-103">Create roleAssignment</span></span>

> <span data-ttu-id="fb7d3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb7d3-105">Erstellen eines neuen [roleAssignment](../resources/intune-rbac-roleassignment.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb7d3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fb7d3-106">Prerequisites</span></span>
<span data-ttu-id="fb7d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb7d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb7d3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fb7d3-109">Permission type</span></span>|<span data-ttu-id="fb7d3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fb7d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb7d3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fb7d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb7d3-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb7d3-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fb7d3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fb7d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb7d3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb7d3-114">Not supported.</span></span>|
|<span data-ttu-id="fb7d3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fb7d3-115">Application</span></span>|<span data-ttu-id="fb7d3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb7d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb7d3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb7d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="fb7d3-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fb7d3-118">Request headers</span></span>
|<span data-ttu-id="fb7d3-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fb7d3-119">Header</span></span>|<span data-ttu-id="fb7d3-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fb7d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb7d3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb7d3-121">Authorization</span></span>|<span data-ttu-id="fb7d3-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fb7d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb7d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fb7d3-123">Accept</span></span>|<span data-ttu-id="fb7d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fb7d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb7d3-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fb7d3-125">Request body</span></span>
<span data-ttu-id="fb7d3-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleAssignment an.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="fb7d3-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleAssignment erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="fb7d3-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fb7d3-128">Property</span></span>|<span data-ttu-id="fb7d3-129">Typ</span><span class="sxs-lookup"><span data-stu-id="fb7d3-129">Type</span></span>|<span data-ttu-id="fb7d3-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb7d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb7d3-131">id</span><span class="sxs-lookup"><span data-stu-id="fb7d3-131">id</span></span>|<span data-ttu-id="fb7d3-132">String</span><span class="sxs-lookup"><span data-stu-id="fb7d3-132">String</span></span>|<span data-ttu-id="fb7d3-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fb7d3-133">Key of the entity.</span></span> <span data-ttu-id="fb7d3-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fb7d3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fb7d3-135">displayName</span></span>|<span data-ttu-id="fb7d3-136">String</span><span class="sxs-lookup"><span data-stu-id="fb7d3-136">String</span></span>|<span data-ttu-id="fb7d3-137">Der Anzeigename der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="fb7d3-138">description</span><span class="sxs-lookup"><span data-stu-id="fb7d3-138">description</span></span>|<span data-ttu-id="fb7d3-139">String</span><span class="sxs-lookup"><span data-stu-id="fb7d3-139">String</span></span>|<span data-ttu-id="fb7d3-140">Beschreibung der Rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="fb7d3-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fb7d3-141">resourceScopes</span></span>|<span data-ttu-id="fb7d3-142">String collection</span><span class="sxs-lookup"><span data-stu-id="fb7d3-142">String collection</span></span>|<span data-ttu-id="fb7d3-143">Liste der IDs der Rollenbereichsmitglieder-Sicherheitsgruppen.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fb7d3-144">Dies sind IDs aus Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="fb7d3-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb7d3-145">Response</span></span>
<span data-ttu-id="fb7d3-146">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [roleAssignment](../resources/intune-rbac-roleassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb7d3-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fb7d3-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb7d3-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb7d3-148">Request</span></span>
<span data-ttu-id="fb7d3-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
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

### <a name="response"></a><span data-ttu-id="fb7d3-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb7d3-150">Response</span></span>
<span data-ttu-id="fb7d3-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb7d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



