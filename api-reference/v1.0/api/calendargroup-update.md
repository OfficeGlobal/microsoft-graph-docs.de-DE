---
title: CalendarGroup aktualisieren
description: Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „calendargroup“ aktualisieren.
author: angelgolfer-ms
ms.openlocfilehash: 24b09f3cd3dc23daf799eac70e59e0c4e32d7079
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324766"
---
# <a name="update-calendargroup"></a><span data-ttu-id="919a1-103">CalendarGroup aktualisieren</span><span class="sxs-lookup"><span data-stu-id="919a1-103">Update calendargroup</span></span>

<span data-ttu-id="919a1-104">Mit dieser API können Sie die Eigenschaften eines Objekts des Typs „calendargroup“ aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="919a1-104">Update the properties of calendargroup object.</span></span>

## <a name="permissions"></a><span data-ttu-id="919a1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="919a1-105">Permissions</span></span>

<span data-ttu-id="919a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="919a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="919a1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="919a1-108">Permission type</span></span>                        | <span data-ttu-id="919a1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="919a1-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="919a1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="919a1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="919a1-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="919a1-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="919a1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="919a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="919a1-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="919a1-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="919a1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="919a1-114">Application</span></span>                            | <span data-ttu-id="919a1-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="919a1-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="919a1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="919a1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="919a1-117">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="919a1-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="919a1-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="919a1-118">Request headers</span></span>

| <span data-ttu-id="919a1-119">Header</span><span class="sxs-lookup"><span data-stu-id="919a1-119">Header</span></span>        | <span data-ttu-id="919a1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="919a1-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="919a1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="919a1-121">Authorization</span></span> | <span data-ttu-id="919a1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="919a1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="919a1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="919a1-124">Content-Type</span></span>  | <span data-ttu-id="919a1-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="919a1-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="919a1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="919a1-127">Request body</span></span>

<span data-ttu-id="919a1-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="919a1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="919a1-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="919a1-131">Property</span></span> | <span data-ttu-id="919a1-132">Typ</span><span class="sxs-lookup"><span data-stu-id="919a1-132">Type</span></span>   | <span data-ttu-id="919a1-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="919a1-133">Description</span></span>     |
| :------- | :----- | :-------------- |
| <span data-ttu-id="919a1-134">name</span><span class="sxs-lookup"><span data-stu-id="919a1-134">name</span></span>     | <span data-ttu-id="919a1-135">String</span><span class="sxs-lookup"><span data-stu-id="919a1-135">String</span></span> | <span data-ttu-id="919a1-136">Der Gruppenname.</span><span class="sxs-lookup"><span data-stu-id="919a1-136">The group name.</span></span> |

## <a name="response"></a><span data-ttu-id="919a1-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="919a1-137">Response</span></span>

<span data-ttu-id="919a1-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="919a1-138">If successful, this method returns a `200 OK` response code and updated [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="919a1-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="919a1-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="919a1-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="919a1-140">Request</span></span>

<span data-ttu-id="919a1-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="919a1-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="919a1-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="919a1-142">Response</span></span>

<span data-ttu-id="919a1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="919a1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
