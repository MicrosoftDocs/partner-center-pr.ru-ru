---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. В составе нового продукта Майкрософт представляет клиентам новые планы подписки Microsoft Dynamics с 1 ноября 2016 года. Они во многом похожи на текущие планы.

В этом документе содержатся инструкции для косвенных поставщиков по переключению существующих подписок клиентов Microsoft Dynamics AX на новое решение Microsoft Dynamics 365. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

Планы Microsoft Dynamics CRM Online и AX перестают действовать.  С 1 июля 2017 г. вы больше не сможете обновить устаревшие планы. Кроме того, существующие подписки E4 не будут продлеваться автоматически после истечения срока действия.

По истечении срока действия подписок CRM Online и AX они будут отменены. Чтобы обеспечить непрерывность для пользователей, следует перенести пользователей с подписками, для которых истекает срок действия, на один из поддерживаемых SKU, которые перечислены ниже. Мы рекомендуем переводить клиентов на новые подписки до ежегодной даты завершения подписки, чтобы не допускать перерывов в предоставлении службы клиентам. 

На странице сведений подписки состояние подписки изменено с "Дата автоматического возобновления: [дата]" на "Срок действия истекает: [дата]". 

Если вы используете API (CREST или Центра партнеров), вы можете найти подписки с истекающим сроком действия по дате завершения подписки и свойству автоматического возобновления со значением "ложь" с 1 июля 2017 г. Перевести клиентов на новый план можно в любое время. 

**Изменения в лицензировании Microsoft Dynamics AX**

Использование серии продуктов Microsoft Dynamics AX прекращается с 1 ноября 2016 г. Подробнее узнать о новых вариантах лицензирования для Dynamics 365 можно в [руководстве по лицензированию](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).

 Подробные сведения о сопоставлении лицензий см. в следующей таблице:

|**Устаревшие SKU**   |**SKU-код Dynamics 365**   |
|-------------------|:----------------------|
|Enterprise SKU|План Microsoft Dynamics 365 for Unified Operations или Microsoft Dynamics 365 |
|Задача|Microsoft Dynamics 365 for Activity
|Задача/самообслуживание|Microsoft Dynamics 365 for Team Members|
|Устройство|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Изменения в лицензировании Microsoft Dynamics CRM Online 

**Microsoft Dynamics CRM Online**

Текущий план Microsoft Dynamics CRM Online снимается с учета 1 ноября 2016г. Подробнее узнать о новых вариантах лицензирования для Microsoft Dynamics 365 можно в предстоящем [руководстве по лицензированию](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf), которое скоро будет опубликовано. Подробнее о новых вариантах лицензирования см. в разделе [Важная информация для пользователей CRM Online](https://go.microsoft.com/fwlink/?linkid=831667).

Подробные сведения о сопоставлении лицензий см. в следующей таблице:

|**Устаревшие SKU**   |**SKU-код Dynamics 365**   |
|-------------------|:----------------------|
|Enterprise|План Dynamics 365 Enterprise Customer Engagement |
|Professional|План Dynamics 365 Enterprise Customer Engagement, Dynamics 365 for Sales или Dynamics 365 for Customer Service|
|Basic|План Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service или Dynamics 365 Enterprise Customer Engagement|
|Essential|Dynamics 365 for Team Members|
|Надстройка Field Service|План Dynamics 365 Enterprise Customer Engagement или Dynamics 365 for Field Service|
|Надстройка Project Service Automation|План Dynamics 365 Customer Engagement или Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Перевод клиентов на новые планы продуктов


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [Отменить старую подписку](#manual-subscription-migration-cancelsubscriptions).

С помощью следующих процедур клиент перемещается из Microsoft Dynamics AX или CRM Online в Dynamics 365.

В этом примере торговому посреднику требуется переместить клиента с существующей подпиской на Dynamics AX Enterprise в Dynamics 365 for Operations. Прежде всего необходимо приобрести Dynamics 365 for Operations.  Повторите эти действия для перемещения клиента CRM Online в Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Приобретение новой подписки**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



