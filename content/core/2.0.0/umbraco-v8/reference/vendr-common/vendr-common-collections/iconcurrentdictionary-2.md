---
title: IConcurrentDictionary<TKey,TValue>
description: API reference for IConcurrentDictionary<TKey,TValue> in Vendr, the eCommerce solution for Umbraco
---
## IConcurrentDictionary&lt;TKey,TValue&gt;

```csharp
public interface IConcurrentDictionary<TKey, TValue> : ICollection<KeyValuePair<TKey, TValue>>, 
    IDictionary<TKey, TValue>, IEnumerable<KeyValuePair<TKey, TValue>>
    where TValue : class
```

**Namespace**
* [Vendr.Common.Collections](../)

### Properties

#### IsEmpty

```csharp
public bool IsEmpty { get; }
```


### Methods

#### AddOrUpdate (1 of 2)

```csharp
public TValue AddOrUpdate(TKey key, Func<TKey, TValue> addValueFactory, 
    Func<TKey, TValue, TValue> updateValueFactory)
```

---

#### AddOrUpdate (2 of 2)

```csharp
public TValue AddOrUpdate(TKey key, TValue addValue, Func<TKey, TValue, TValue> updateValueFactory)
```


---

#### GetOrAdd

```csharp
public TValue GetOrAdd(TKey key, Func<TKey, TValue> valueFactory)
```


---

#### GetOrAddIfNotNull

```csharp
public TValue GetOrAddIfNotNull(TKey key, Func<TKey, TValue> valueFactory)
```


---

#### ToArray

```csharp
public KeyValuePair<TKey, TValue>[] ToArray()
```


---

#### TryAdd

```csharp
public bool TryAdd(TKey key, TValue value)
```


---

#### TryRemove

```csharp
public bool TryRemove(TKey key, out TValue value)
```


---

#### TryUpdate

```csharp
public bool TryUpdate(TKey key, TValue newValue, TValue comparisonValue)
```


<!-- DO NOT EDIT: generated by xmldocmd for Vendr.Common.dll -->
