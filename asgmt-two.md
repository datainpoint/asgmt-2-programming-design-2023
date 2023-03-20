# Assignment 2

> Programming Design 2023

## 01. Define a function `describe_bmi()` which returns the description of BMI with 3 levels: `"Underweight"`, `"Normal weight"`, or `"Overweight"` given a person's height in centimeters and weight in kilograms.

$$
\text{BMI} = \frac{\text{Weight}_{\text{kg}}}{\text{Height}_{\text{m}}^2}
$$

|BMI|Description|
|:---:|-----------|
|$< 18.5$|Underweight|
|$18.5 – 24.9$|Normal weight|
|$25.0 - $|Overweight|

```python
def describe_bmi(height: int, weight: int) -> str:
    """
    >>> describe_bmi(172, 50)
    'Underweight'
    >>> describe_bmi(172, 65)
    'Normal weight'
    >>> describe_bmi(175, 100)
    'Overweight'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a function `is_upper_or_lower_cased()` which returns `"Upper-cased"` if intput alphabet is upper-cased, otherwise returns `"Lower-cased"`.

```python
def is_upper_or_lower_cased(x: str) -> str:
    """
    >>> is_upper_or_lower_cased("a")
    'Lower-cased'
    >>> is_upper_or_lower_cased("A")
    'Upper-cased'
    >>> is_upper_or_lower_cased("z")
    'Lower-cased'
    >>> is_upper_or_lower_cased("Z")
    'Upper-cased'
    >>> is_upper_or_lower_cased("e")
    'Lower-cased'
    >>> is_upper_or_lower_cased("E")
    'Upper-cased'
    >>> is_upper_or_lower_cased("b")
    'Lower-cased'
    >>> is_upper_or_lower_cased("B")
    'Upper-cased'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a function `reverse_vowel()` which swaps a vowel's case and does nothing given a non-vowel alphabet.

```python
def reverse_vowel(x: str) -> str:
    """
    >>> reverse_vowel("a")
    'A'
    >>> reverse_vowel("A")
    'a'
    >>> reverse_vowel("z")
    'z'
    >>> reverse_vowel("Z")
    'Z'
    >>> reverse_vowel("e")
    'E'
    >>> reverse_vowel("E")
    'e'
    >>> reverse_vowel("b")
    'b'
    >>> reverse_vowel("B")
    'B'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a function `convert_temperature_degrees_to_different_scales(x, from_scale, to_scale)` which converts temperature degrees between 3 different scales.

$$
\text{Fahrenheit}(^{\circ} F) = \text{Celsius}(^{\circ} C) \times \frac{9}{5} + 32 \\
\text{Celsius}(^{\circ} C) = (\text{Fahrenheit}(^{\circ} F) - 32) \times \frac{5}{9} \\
\text{Kelvin}(K) = \text{Celsius}(^{\circ} C) + 273.15
$$

```python
def convert_temperature_degrees_to_different_scales(x: float, from_scale: str, to_scale: str) -> float:
    """
    >>> convert_temperature_degrees_to_different_scales(0, "Celsius", "Fahrenheit")
    32.0
    >>> convert_temperature_degrees_to_different_scales(100, "Celsius", "Fahrenheit")
    212.0
    >>> convert_temperature_degrees_to_different_scales(32, "Fahrenheit", "Celsius")
    0.0
    >>> convert_temperature_degrees_to_different_scales(212, "Fahrenheit", "Celsius")
    100.0
    >>> convert_temperature_degrees_to_different_scales(0, "Celsius", "Kelvin")
    273.15
    >>> convert_temperature_degrees_to_different_scales(100, "Celsius", "Kelvin")
    373.15
    >>> convert_temperature_degrees_to_different_scales(32, "Fahrenheit", "Kelvin")
    273.15
    >>> convert_temperature_degrees_to_different_scales(212, "Fahrenheit", "Kelvin")
    373.15
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a function `get_alphabet_with_order()` which returns alphabets given its order.

```python
def get_alphabet_with_order(x: int, is_upper_cased: bool) -> str:
    """
    >>> get_alphabet_with_order(1, False)
    'a'
    >>> get_alphabet_with_order(1, True)
    'A'
    >>> get_alphabet_with_order(2, False)
    'b'
    >>> get_alphabet_with_order(2, True)
    'B'
    >>> get_alphabet_with_order(25, False)
    'y'
    >>> get_alphabet_with_order(25, True)
    'Y'
    >>> get_alphabet_with_order(26, False)
    'z'
    >>> get_alphabet_with_order(26, True)
    'Z'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a function `categorize_nikes_running_shoes()` which returns Nike's running shoe series given its features.

|Series|Has ZoomX|Has Carbon plate|Has Airbag|
|------|---------|----------------|----------|
|Pegasus|No|No|No|
|Tempo|No|No|Yes|
|Turbo|Yes|No|No|
|Vaporfly|Yes|Yes|No|
|Alphafly|Yes|Yes|Yes|

```python
def categorize_nikes_running_shoes(has_zoomx: bool, has_carbon_plate: bool, has_airbag: bool) -> str:
    """
    >>> categorize_nikes_running_shoes(False, False, False)
    'Pegasus'
    >>> categorize_nikes_running_shoes(False, False, True)
    'Tempo'
    >>> categorize_nikes_running_shoes(True, False, False)
    'Turbo'
    >>> categorize_nikes_running_shoes(True, True, False)
    'Vaporfly'
    >>> categorize_nikes_running_shoes(True, True, True)
    'Alphafly'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a function `use_lists_pop_method()` which returns the last element of given list and the remaining list as a dictionary.

```python
def use_lists_pop_method(x: list) -> dict:
    """
    >>> input_list = [2, 3, 5, 7]
    >>> use_lists_pop_method(input_list)
    {'last_element': 7, 'remaining_list': [2, 3, 5]}
    >>> input_list = [2, 3, 5]
    >>> use_lists_pop_method(input_list)
    {'last_element': 5, 'remaining_list': [2, 3]}
    >>> input_list = [2, 3]
    >>> use_lists_pop_method(input_list)
    {'last_element': 3, 'remaining_list': [2]}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `retrieve_middle_elements()` which returns the middle elements of a given list.

```python
def retrieve_middle_elements(x: list):
    """
    >>> retrieve_middle_elements([2, 3, 5])
    3
    >>> retrieve_middle_elements([2, 3, 5, 7])
    (3, 5)
    >>> retrieve_middle_elements([2, 3, 5, 7, 11])
    5
    >>> retrieve_middle_elements([2, 3, 5, 7, 11, 13])
    (5, 7)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `median()` which returns the median value of a given list.

Source: <https://en.wikipedia.org/wiki/Median>

```python
def median(x: list):
    """
    >>> median([2, 3, 5, 7, 11])
    5
    >>> median([2, 3, 5, 7, 11, 13])
    6.0
    >>> median([11, 13, 17, 2, 3, 5, 7])
    7
    >>> median([7, 11, 13, 17, 19, 2, 3, 5])
    9.0
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `sing_do_re_mi()` which returns the lyrics of "Do-Re-Mi".

Source: <https://youtu.be/Qy9cj-zwbVY>

```python
def sing_do_re_mi(note: str) -> str:
    """
    >>> sing_do_re_mi("Do")
    'a deer, a female deer.'
    >>> sing_do_re_mi("Re")
    'a drop of golden sun.'
    >>> sing_do_re_mi("Mi")
    'a name I call myself.'
    >>> sing_do_re_mi("Fa")
    'a long long way to run.'
    >>> sing_do_re_mi("So")
    'a needle pulling thread.'
    >>> sing_do_re_mi("La")
    'a note to follow so.'
    >>> sing_do_re_mi("Ti")
    'a drink with jam and bread.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```