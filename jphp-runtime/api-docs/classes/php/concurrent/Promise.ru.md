# Promise

- **класс** `Promise` (`php\concurrent\Promise`)
- **пакет** `std`
- **исходники** [`php/concurrent/Promise.php`](./src/main/resources/JPHP-INF/sdk/php/concurrent/Promise.php)

**Описание**

Class Promise

---

#### Статичные Методы

- `Promise ::`[`resolve()`](#method-resolve)
- `Promise ::`[`reject()`](#method-reject)
- `Promise ::`[`race()`](#method-race)
- `Promise ::`[`all()`](#method-all)

---

#### Методы

- `->`[`__construct()`](#method-__construct) - _Promise constructor._
- `->`[`makeFulfill()`](#method-makefulfill)
- `->`[`makeReject()`](#method-makereject)
- `->`[`then()`](#method-then)
- `->`[`catch()`](#method-catch)
- `->`[`wait()`](#method-wait) - _Stops execution until this promise is resolved._

---
# Методы

<a name="method-__construct"></a>

### __construct()
```php
__construct(callable $executor): void
```
Promise constructor.

---

<a name="method-makefulfill"></a>

### makeFulfill()
```php
makeFulfill( $result): void
```

---

<a name="method-makereject"></a>

### makeReject()
```php
makeReject(Throwable $error): void
```

---

<a name="method-then"></a>

### then()
```php
then(callable|null $onFulfilled, callable|null $onRejected): php\concurrent\Promise
```

---

<a name="method-catch"></a>

### catch()
```php
catch([ callable|null $onRejected): php\concurrent\Promise
```

---

<a name="method-wait"></a>

### wait()
```php
wait(): mixed
```
Stops execution until this promise is resolved.

---