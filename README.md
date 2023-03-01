# XML format
To import property, please folow XML creation guide.
## IO_EstatesType
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
```
class IO_EstatesRooms
{
  const Garsonjera = 38;
  const OneRoom = 39;
  const TwoRooms = 37;
  const ThreeRooms = 40;
  const FourRooms = 41;
  const FiveAndMoreRooms = 42;
}
```

## IO_EstatesHeating
```
class IO_EstatesHeating
{
  const Drva = 51;
  const Gradsko = 52;
  const Kotlovnica = 53;
  const Ostalo = 54;
  const Plin = 55;
  const Podno = 56;
  const Struja = 57;
}
```
## IO_EstatesAttributes
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
## IO_EstatesEquipment
```
class IO_EstatesEquipment
{
  const Equipped = 62;
  const Unequipped = 63;
  const Semiequipped = 64;
}
```
## IO_EstatesPaymentInterval
```
class IO_EstatesPaymentInterval
{
  const Month = 'month';
  const Day = 'day';
  const None = null;
}
```
## IO_EstatesMode
```
class  IO_EstatesMode
{
  const Buy = 'buy';
  const Sell = 'sell';
  const Rent = 'rent';
  const Lease = 'lease';
}
```
