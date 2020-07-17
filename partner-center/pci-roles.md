---
title: Доступ на основе ролей центра партнеров Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Сведения о конкретных ролях, необходимых для просмотра отчетов центра партнеров. К ним относятся роли средства просмотра отчетов руководителя и средства просмотра отчетов.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a9df2b6f67ca4e825da2c273c82d7cd46763f1b
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436643"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="4fe5a-104">Управление доступом на основе ролей на панели мониторинга центра партнеров</span><span class="sxs-lookup"><span data-stu-id="4fe5a-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="4fe5a-105">Панель мониторинга Insights использует две новые роли в центре партнеров для управления доступом сотрудников к диспетчеру отчетов и средству просмотра отчетов.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="4fe5a-106">Пользователи в роли средства просмотра отчетов руководителя имеют доступ ко всем наборам данных отчетов, а пользователи в роли средства просмотра отчетов не будут иметь доступ к конфиденциальным наборам, таким как доход, а также персональные данные клиентов и сотрудников.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="4fe5a-107">Как и в случае с другими ролями центра партнеров, глобальный администратор или администратор учетной записи сможет назначить пользователей этим ролям на странице Управление пользователями.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="4fe5a-108">Роли могут быть применимы ко всей компании или к конкретным MPN расположениям.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="4fe5a-109">Роли, назначенные для конкретных расположений MPN, ограничивают пользователя для просмотра данных отчетов, связанных только с выбранными расположениями MPN.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="4fe5a-110">Партнер может выбрать одно или несколько расположений из приведенного ниже представления.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-110">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Роли":::

>[!Note]
> <span data-ttu-id="4fe5a-112">Пользователи, MPN администраторов на 20 января, 2020 автоматически добавляются в роль **средства просмотра отчетов руководителя** Организации для всех расположений для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-112">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="4fe5a-113">Таким образом, эти пользователи могут получить доступ к отчетам в качестве средства просмотра отчетов руководителя без явного действия, необходимого глобальному администратору или администратору учетной записи. Глобальные администраторы и администраторы учетных записей могут переопределять автоматические назначенные роли этих пользователей для дальнейшего увеличения или ограничения их возможностей.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4fe5a-114">Дальнейшие шаги</span><span class="sxs-lookup"><span data-stu-id="4fe5a-114">Next steps</span></span>

- <span data-ttu-id="4fe5a-115">Дополнительные сведения о [партнерских аналитиках](partner-center-insights.md) и различных отчетах.</span><span class="sxs-lookup"><span data-stu-id="4fe5a-115">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
