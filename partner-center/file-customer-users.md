---
title: Поля для CSV-файла для импорта нескольких пользователей для учетной записи клиента
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Чтобы добавить нескольких пользователей в учетную запись клиента, создайте файл значений с разделителями-запятыми (CSV) с соответствующими полями.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150987"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="8e145-103">Добавление нескольких пользователей в учетную запись клиента путем создания CSV-файла</span><span class="sxs-lookup"><span data-stu-id="8e145-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="8e145-104">**Соответствующие роли** — глобальный администратор.</span><span class="sxs-lookup"><span data-stu-id="8e145-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8e145-105">Одновременное добавление нескольких пользователей в учетную запись клиента путем отправки файла данных в формате файла с разделителями-запятыми (CSV) в центр партнеров.</span><span class="sxs-lookup"><span data-stu-id="8e145-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="8e145-106">Вы можете скачать образец файла данных из центра партнеров, а затем изменить его для использования или создать новый файл данных, используя модель данных, определенную ниже.</span><span class="sxs-lookup"><span data-stu-id="8e145-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="8e145-107">Требования к файлу данных</span><span class="sxs-lookup"><span data-stu-id="8e145-107">Data file requirements</span></span>

<span data-ttu-id="8e145-108">Чтобы добавить нескольких пользователей в учетную запись клиента с помощью процесса групповой отправки, необходимо выполнить следующие требования.</span><span class="sxs-lookup"><span data-stu-id="8e145-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="8e145-109">у вас должны быть разрешения глобального администратора для учетной записи клиента;</span><span class="sxs-lookup"><span data-stu-id="8e145-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="8e145-110">у каждого пользователя должен быть уникальный электронный адрес в почтовом домене пользователя;</span><span class="sxs-lookup"><span data-stu-id="8e145-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="8e145-111">одновременно можно передавать до 100 записей.</span><span class="sxs-lookup"><span data-stu-id="8e145-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="8e145-112">Если вам необходимо добавить более 100 пользователей, создайте и загрузите дополнительные файлы данных;</span><span class="sxs-lookup"><span data-stu-id="8e145-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="8e145-113">все пользователи должны быть в одном географическом **регионе**;</span><span class="sxs-lookup"><span data-stu-id="8e145-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="8e145-114">вводите только данные, описанные ниже.</span><span class="sxs-lookup"><span data-stu-id="8e145-114">Enter only the data described below.</span></span> <span data-ttu-id="8e145-115">Лишние данные приведут к ошибке отправки.</span><span class="sxs-lookup"><span data-stu-id="8e145-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="8e145-116">Введите следующие данные в файле данных:</span><span class="sxs-lookup"><span data-stu-id="8e145-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="8e145-117">**Имя столбца**</span><span class="sxs-lookup"><span data-stu-id="8e145-117">**Column name**</span></span> | <span data-ttu-id="8e145-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8e145-118">**Description**</span></span>  | <span data-ttu-id="8e145-119">**Ограничения**</span><span class="sxs-lookup"><span data-stu-id="8e145-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="8e145-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8e145-120">First name</span></span>  | <span data-ttu-id="8e145-121">Имя пользователя (необязательное поле)</span><span class="sxs-lookup"><span data-stu-id="8e145-121">User's first name (optional field)</span></span>  | <span data-ttu-id="8e145-122">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="8e145-122">50-character limit</span></span>  |
| <span data-ttu-id="8e145-123">Фамилия</span><span class="sxs-lookup"><span data-stu-id="8e145-123">Last name</span></span>  | <span data-ttu-id="8e145-124">Фамилия пользователя (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="8e145-124">User's last name (optional field)</span></span>  | <span data-ttu-id="8e145-125">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="8e145-125">50-character limit</span></span>  |
| <span data-ttu-id="8e145-126">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="8e145-126">Display name</span></span>    | <span data-ttu-id="8e145-127">Имя, отображаемое в центре партнеров (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="8e145-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="8e145-128">Не более 50 знаков</span><span class="sxs-lookup"><span data-stu-id="8e145-128">50-character limit</span></span>                         |
| <span data-ttu-id="8e145-129">Email</span><span class="sxs-lookup"><span data-stu-id="8e145-129">Email</span></span>   | <span data-ttu-id="8e145-130">Рабочий адрес электронной почты пользователя в клиентской компании (обязательное поле)</span><span class="sxs-lookup"><span data-stu-id="8e145-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="8e145-131">Каждый пользователь должен иметь уникальный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8e145-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="8e145-132">Обновление состояния</span><span class="sxs-lookup"><span data-stu-id="8e145-132">Status update</span></span>   | <span data-ttu-id="8e145-133">Используется для указания, успешно ли создана новая запись пользователя</span><span class="sxs-lookup"><span data-stu-id="8e145-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="8e145-134">\*\*Оставить пустым\*\*</span><span class="sxs-lookup"><span data-stu-id="8e145-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="8e145-135">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="8e145-135">Next steps</span></span>

- [<span data-ttu-id="8e145-136">Как добавить нескольких пользователей для клиента</span><span class="sxs-lookup"><span data-stu-id="8e145-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)