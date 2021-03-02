# React övningar - components, state och props

## 1. Static Profile card
Skapa en komponent ```<ProfileCard>``` innehållandes en bild, namn, titel och en knapp.

## 2. Dynamic Profile card using state
Skapa en komponent ```<ProfileCard>``` innehållandes en bild, namn, titel och en knapp. Namn och titel ska vara dynamiska med hjälp av *state*. Vid knapptryck ska titeln ändras till *senior ninja*.

## 3. Dynamic Profile card using props
Skapa en komponent ```<ProfileCard>``` innehållandes en bild, namn, titel och en knapp. Namn och titel ska vara props nedskickade ifrån ```<App />```.

## 4. Dynamic Profile card using deconstructed props
Skapa två komponenter: ```<Parent />``` och ```<ProfileCard />```. Propa ner följande user i ```<ProfileCard />```. Använd endast egenskaperna *namn* och *titel* i ProfileCard-komponenten med hjälp av deconstruction.

```javascript
const user = {
    name: 'Nicodemus Naveltuta',
    age: '47',
    title: 'vice ninja',
    email: 'nicokick@theoffice.net'
}
```

## 5. Multilevel props in nested components
Skapa komponenter enligt följande struktur:

```javascript
<Grandparent>
    <Parent>
        <Child>
 ```

Skicka stringen ```Hej barnbarnet!``` från ```<Grandparent />``` ner till ```<Child />```.


## 6. Levelup Candyman
Expandera övning 5 med följande:

### Grandparent
Grandparent ska ha en button *Give candy*". När man klickar på den ska ett värde skickas till Parent med props.

### Parent
Parent ska ha **två** buttons: *Nope* och *Alright, it's saturday*.
När man klickar ska olika värden skickas ner till Child med props.

### Child
Child ska visa antingen texten *Energy: low" eller "Energy: it's over 9000" baserat på vilket värde som skickas ner. Du bestämmer vart gränsen går mellan "Energy: Low" och "Energy: it's over 9000".