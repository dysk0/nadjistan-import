# XML format
To import property, please folow XML creation guide.

## IO_EstatesMode
This is one of the most important taxonomies. You can use hardcoded values:

```
class  IO_EstatesMode
{
  const Buy = 'buy';
  const Sell = 'sell';
  const Rent = 'rent';
  const Lease = 'lease';
}
```



## IO_EstatesType
This is one of the most important taxonomies. If you are using values from the REST endpoint, please note that you'll need to provide one ID where `parent` is 0 and you can provide one subitem of that parent if it exists.

| IO_EstatesType |  |   |
| --- | --- | --- |
| Homes |  | 8 |
|  |  Duplex | 9 |
|  |  Montazna | 10 |
|  |  Samostalna | 11 |
|  |  Vikendica | 11 |


You can use hardcoded values:
```
class IO_EstatesType
{
  const Homes = 8;
  const Garage = 3;
  const Office = 13;
  const Apartment = 23;
  const Land = 24;
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_type`


## IO_EstatesWaste
This taxonomy is used to set waste for property.

You can use hardcoded values:

```
class IO_EstatesWaste
{
  const None = 247;
  const Public = 246;
  const CessPit = 245;
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_waste`

## IO_EstatesRooms
Taxonomy is used to specify number of rooms for a property. Can be used only with Home and Apartment `IO_EstatesType`.
```
class IO_EstatesRooms
{
  const Studio = 38;
  const OneRoom = 39;
  const TwoRooms = 37;
  const ThreeRooms = 40;
  const FourRooms = 41;
  const FiveAndMoreRooms = 42;
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_rooms`


## IO_EstatesHeating
Taxonomy is used to specify heating method. It is meaningfull only to Home and Apartment `IO_EstatesType`.
```
class IO_EstatesHeating
{
  const Wood = 51;        // drva
  const City = 52;        // gradsko
  const BoilerRoom = 53;  // kotlovnica u zgradi
  const Other = 54;       // ostalo
  const Gas = 55;         // plin
  const Floor = 56;       // podno grijanje
  const Electricity = 57; // el. energija
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_heating`

## IO_EstatesAttributes
Taxonomy is used to specify additional atributes of the property. 
```
class IO_EstatesAttributes
{
  const AutomatskaVrata = 65;
  const Alarm = 66;
  const Balkon = 67;
  const Bazen = 240;
  const Klima = 68;
  const Lift = 69;
  const Podrum = 241;
  const Shupa = 241;
  const Uknjizeno = 71;
  const VideoNadzor = 70;
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_attr`

## IO_EstatesCondition
```
class IO_EstatesCondition
{
  const New = 59;
  const Good = 308;
  const Renovated = 60;
  const Old = 309;
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_condition`


## IO_EstatesEquipment
```
class IO_EstatesEquipment
{
  const Equipped = 62;
  const Unequipped = 63;
  const Semiequipped = 64;
}
```
Or fetch data from on following endpoint:
`/wp-json/wp/v2/io_estates_equip`

## IO_EstatesPaymentInterval
```
class IO_EstatesPaymentInterval
{
  const Month = 'month';
  const Day = 'day';
  const None = null;
}
```
