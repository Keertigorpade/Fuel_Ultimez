def calculate_pizza_slices(people):
    large_slices = 8
    medium_slices = 6
    regular_slices = 4
    small_slices = 1


    large_pizzas = people // large_slices
    people %= large_slices

    medium_pizzas = people // medium_slices
    people %= medium_slices

    regular_pizzas = people // regular_slices
    people %= regular_slices

    small_pizzas = people // small_slices

    return large_pizzas, medium_pizzas, regular_pizzas, small_pizzas


# Test cases
print(calculate_pizza_slices(100))
print(calculate_pizza_slices(19))
print(calculate_pizza_slices(40))
