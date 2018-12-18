---
title: roleDefinition erstellen
description: Erstellt neue Objekte des Typs roleDefinition.
author: tfitzmac
ms.openlocfilehash: 0ad52c78b6b414fc0419078cd44bcbca2b82ed83
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322400"
---
# <a name="create-roledefinition"></a><span data-ttu-id="cf07b-103">roleDefinition erstellen</span><span class="sxs-lookup"><span data-stu-id="cf07b-103">Create roleDefinition</span></span>

> <span data-ttu-id="cf07b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf07b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf07b-105">Erstellt neue Objekte des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cf07b-105">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf07b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf07b-106">Prerequisites</span></span>
<span data-ttu-id="cf07b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf07b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf07b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf07b-109">Permission type</span></span>|<span data-ttu-id="cf07b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf07b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf07b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf07b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf07b-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf07b-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cf07b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf07b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf07b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf07b-114">Not supported.</span></span>|
|<span data-ttu-id="cf07b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf07b-115">Application</span></span>|<span data-ttu-id="cf07b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf07b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf07b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf07b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="cf07b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf07b-118">Request headers</span></span>
|<span data-ttu-id="cf07b-119">Header</span><span class="sxs-lookup"><span data-stu-id="cf07b-119">Header</span></span>|<span data-ttu-id="cf07b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="cf07b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf07b-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cf07b-121">Authorization</span></span>|<span data-ttu-id="cf07b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf07b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf07b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf07b-123">Accept</span></span>|<span data-ttu-id="cf07b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf07b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf07b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf07b-125">Request body</span></span>
<span data-ttu-id="cf07b-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs roleDefinition an.</span><span class="sxs-lookup"><span data-stu-id="cf07b-126">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="cf07b-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der roleDefinition erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cf07b-127">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="cf07b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cf07b-128">Property</span></span>|<span data-ttu-id="cf07b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="cf07b-129">Type</span></span>|<span data-ttu-id="cf07b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf07b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf07b-131">id</span><span class="sxs-lookup"><span data-stu-id="cf07b-131">id</span></span>|<span data-ttu-id="cf07b-132">String</span><span class="sxs-lookup"><span data-stu-id="cf07b-132">String</span></span>|<span data-ttu-id="cf07b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cf07b-133">Key of the entity.</span></span> <span data-ttu-id="cf07b-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="cf07b-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cf07b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cf07b-135">displayName</span></span>|<span data-ttu-id="cf07b-136">String</span><span class="sxs-lookup"><span data-stu-id="cf07b-136">String</span></span>|<span data-ttu-id="cf07b-137">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="cf07b-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="cf07b-138">description</span><span class="sxs-lookup"><span data-stu-id="cf07b-138">description</span></span>|<span data-ttu-id="cf07b-139">String</span><span class="sxs-lookup"><span data-stu-id="cf07b-139">String</span></span>|<span data-ttu-id="cf07b-140">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="cf07b-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="cf07b-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cf07b-141">rolePermissions</span></span>|<span data-ttu-id="cf07b-142">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cf07b-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="cf07b-143">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="cf07b-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cf07b-144">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="cf07b-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="cf07b-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cf07b-145">isBuiltIn</span></span>|<span data-ttu-id="cf07b-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cf07b-146">Boolean</span></span>|<span data-ttu-id="cf07b-147">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="cf07b-147">Type of Role.</span></span> <span data-ttu-id="cf07b-148">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="cf07b-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="cf07b-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf07b-149">Response</span></span>
<span data-ttu-id="cf07b-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf07b-150">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf07b-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf07b-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf07b-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf07b-152">Request</span></span>
<span data-ttu-id="cf07b-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf07b-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="cf07b-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf07b-154">Response</span></span>
<span data-ttu-id="cf07b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf07b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



