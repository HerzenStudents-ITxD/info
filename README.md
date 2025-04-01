# info
## Бекэнд
Для тех, у кого не получается сделать нормальный бекэнд, можно использовать инструмент его эмулирования:
* Сначала узнаём номер своей команды (owner): GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owners;
* Потом смотрите список существующих типов json, которые существуют в команде: GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/types;
* Если не находите нужного, придумываете его название, например (products);
* Сохранить json для products: POST https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/products, сам json в body складываете,
на вход принимается только валидный json;
* Получить все json для product: GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/products; 
* Получить конкретный json по его id: GET https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/products/17;
* Изменить конкретный json по его id: PATCH https://d5dvn9i0jk96ihl2ngsb.8wihnuyr.apigw.yandexcloud.net/api/owner/1/products/17, сам json в body складываете,
на вход принимается только валидный json.
