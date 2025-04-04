
# 🧠 Zadanie: Porównywanie obiektów

Twoim celem jest zaimplementowanie mechanizmu, który umożliwia **porównywanie obiektów klas `Person` oraz `Address`**.

---

## 🔎 Kiedy obiekty uznajemy za równe?

Dwa obiekty są **takie same**, gdy:
- wszystkie **wartości pól** są identyczne,
- jeżeli pole jest **referencją** (np. do innego obiektu lub kolekcji obiektów),
  - to również **wszystkie pola tych referencji muszą być równe**.

> Przykład: Obiekt `Person` zawiera listę adresów (`ArrayList<Address>`). W takim przypadku należy sprawdzić, czy wszystkie pola w każdym `Address` są również równe.

W każdym innym przypadku obiekty powinny być uznane za **różne**.

---

## 🛠️ Wymagania techniczne

Aby prawidłowo rozwiązać zadanie, należy **nadpisać** poniższe metody dziedziczone z klasy `Object`:

- `equals(Object other)`  
- `hashCode()`  
- `toString()`

---

## 🧾 Wskazówka

Podczas implementacji metody `toString()` warto użyć klasy `StringBuilder` — pozwala ona wydajnie tworzyć złożone reprezentacje tekstowe obiektów.
