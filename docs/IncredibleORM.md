
# IncredibleORM: More than incredible, marvelous

This is the most advanced ORM in the market, you'll use it to create your models, fields and relationships.

## Declaring a model

Models must inherit from `IncredibleModel` abstract class.

A model is like any other Python class, but it defines fields, that stores data.

Example:

```python
class MyModel(IncredibleModel):
    field = IncredibleField(arg=value)

    def my_method(self):
        return something
```

## Fields

### IncredibleIntegerField

This field stores integers, A.K.A. `int` in Python data types.

Args:
- `optional`: Indicates wether this field is optional, the default value is `True`.

Example:

```python
class MyModel(IncredibleModel):
    count = IncredibleIntegerField(optional=False)
```

### IncredibleCharField

This field stores a sequence of characters, A.K.A. `string` in Python data types.

Args:
- `optional` (bool): Indicates wether this field is optional, the default value is `True`.
- `max_length` (int): Maximum length of the stored string.

Example:

```python
class MyModel(IncredibleModel):
    country = IncredibleCharField(optional=False, max_length=32)
```

### IncredibleForeignKey    

This field stores a reference to another model class.

Args:
- `optional` (bool): Indicates wether this field is optional, the default value is `True`.
- `to` (class): Target model of the relation.

Example:

```python
class MyModel(IncredibleModel):
    parent = IncredibleForeignKey(optional=False, to=ParentModel)
```