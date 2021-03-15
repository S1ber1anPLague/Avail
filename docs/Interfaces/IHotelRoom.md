# Интерфейс IHotelRoom

Интерфейс работает с методами класса [HotelRoom](../Classes/HotelRoom.md).

## Методы интерфейса

- **Add** (HotelRoom: HotelRoom): Result – функция, добавляющая номер отеля. Пара-метр «HotelRoom» – номер отеля, который нужно добавить. Возвращает инстанс класса Result с результатом операции и доп. информацией при ошибке;
- **Del** (HotelRoom: HotelRoom): Result – функция, удаляющая номер отеля. Параметр «HotelRoom» – номер отеля, который нужно удалить. Возвращает инстанс класса Re-sult с результатом операции и доп. информацией при ошибке;
- **Edit** (HotelRoom: HotelRoom): Result – функция, редактирующая номер отеля. Па-раметр «HotelRoom» – номер отеля, который нужно отредактировать. Возвращает инстанс класса Result с результатом операции и доп. информацией при ошибке;
- **GetSales** (ID: int): List< Sale > – функция, которая возвращает список продаж данного номера отеля. Параметр ID – идентификатор номера отеля, продажи которого долж-на вывести функция;
- **GetAll** (sorting: string, AskOrDesk: string, filterA: HotelRoom, filterB: HotelRoom, count: int, page: int): List< HotelRoom > – функция, возвращающая список номеров отеля с заданными параметрами. Параметры: 
    -	*sorting*: string – отвечает, по какому полю будет сортироваться список:
    -	*AskOrDesk*: string – отвечает, по возрастанию или убыванию будут сортиро-ваться элементы;
    -	*filterA*: HotelRoom – отвечает за фильтрацию, включает в себя левую границу интер-вала значений фильтра;
    -	*filter*: HotelRoom – отвечает за фильтрацию, включает в себя правую границу интер-вала значений фильтра; 
    -	*count*: int – отвечает, сколько элементов необходимо показать;
    -	*page*: int – отвечает, с какой страницы начинать поиск элементов. 